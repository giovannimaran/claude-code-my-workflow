---
paths:
  - "scripts/python/**/*.py"
  - "explorations/**/*.py"
---

# Python Code Conventions

**Reproducibility is the default, not a feature.** A script should be runnable from a clean shell with no manual intervention, from the repository root, and produce the same outputs every time.

> This rule mirrors [`r-code-conventions.md`](r-code-conventions.md) and [`stata-code-conventions.md`](stata-code-conventions.md) for the Python-first pipeline (the primary workflow for this project: data cleaning, network construction, RCA, BRIM community detection, descriptive analysis, figures). The numerical-discipline and figure rules apply across all three languages.

## 1. Reproducibility scaffolding

Every pipeline script starts with the same shape:

```python
"""
NN_descriptive_name.py
Purpose:   [one-sentence description]
Inputs:    [path(s) relative to repo root]
Outputs:   [path(s) relative to repo root]
Run order: Standalone | After NN_prior.py
"""
from __future__ import annotations

import logging
from pathlib import Path

import numpy as np
import pandas as pd

# --- Reproducibility ---------------------------------------------------------
SEED = 20260603                       # YYYYMMDD; set ONCE, at the top
rng = np.random.default_rng(SEED)     # prefer Generator over legacy np.random.seed

# --- Paths (always relative to repo root) ------------------------------------
ROOT = Path(__file__).resolve().parents[2]   # scripts/python/NN.py → repo root
DATA = ROOT / "data"
OUT = ROOT / "scripts" / "python" / "_outputs"
OUT.mkdir(parents=True, exist_ok=True)

logging.basicConfig(level=logging.INFO, format="%(asctime)s %(levelname)s %(message)s")
log = logging.getLogger(__name__)
```

Why each line:

- **`SEED` set once** — every random op draws from the same `rng`. Do not re-seed mid-script. If you use `random`, `scikit-learn`, `networkx`, or `igraph` RNGs, seed each explicitly from `SEED` (see §6).
- **`Path(__file__).resolve().parents[2]`** — never hard-code `/Users/giovannimaran/...`. Paths resolve relative to the file so the pipeline runs on any machine.
- **`OUT.mkdir(parents=True, exist_ok=True)`** — output directory is created idempotently.
- **`logging` not `print`** — timestamped, leveled, and suppressible. Use `print` only for genuine CLI output.

## 2. Numbered pipeline

Scripts live in `scripts/python/` and are numbered for run order:

```
scripts/python/
├── 00_run_all.py        # imports + runs 01..06 in order; the one-command reproduction
├── 01_load.py           # ingest raw microdata → parquet
├── 02_clean.py          # firm-product-destination panel; dedup, type coercion
├── 03_rca.py            # RCA / Balassa index, firm-product link definition
├── 04_network.py        # bipartite firm-product graph construction
├── 05_community.py      # BRIM-style community / block detection
├── 06_describe.py       # descriptive stats + publication figures
└── lib/                 # shared helpers (importable; not numbered)
    ├── __init__.py
    ├── io.py            # load/save helpers, path constants
    ├── rca.py           # RCA computation
    └── networks.py      # graph + community-detection functions
```

`python scripts/python/00_run_all.py` from the repo root reproduces every output the paper cites. Shared logic goes in `lib/` and is imported — never copy-paste a function across numbered scripts.

## 3. Outputs convention

All generated outputs land in `scripts/python/_outputs/` (gitignored):

```
scripts/python/_outputs/
├── panel.parquet              # cleaned firm-product-destination panel
├── rca_links.parquet          # RCA-based firm-product links
├── communities.parquet        # node → block assignment
├── descriptives.csv           # summary stats
├── tab_*.tex                  # tables for direct \input{} in paper
├── fig_*.pdf  / fig_*.png     # vector (paper) + raster (slides)
└── sessionInfo.txt            # python + key package versions (pip freeze subset)
```

- **Parquet over CSV** for intermediate data (typed, compressed, fast). CSV only for small human-readable summaries.
- **`sessionInfo.txt` is mandatory** — capture `python --version` + pinned versions of pandas/numpy/networkx/scipy at the end of `00_run_all.py`.
- Tables for the paper are emitted as `.tex` and pulled via `\input{}` — never hand-format a number that came from code (mirrors the Stata `esttab` discipline).

## 4. Code style

- **PEP 8**, enforced with `ruff` (or `black` + `flake8`). Line length 100.
- **Type hints on every function signature.** `def rca(df: pd.DataFrame, *, threshold: float = 1.0) -> pd.DataFrame:`
- **One-line docstring** for any non-obvious function; full docstring (Args/Returns) for anything in `lib/`.
- **`snake_case`** functions and variables; verb-noun for functions (`compute_rca`, `build_bipartite`).
- **No magic numbers** — RCA thresholds, year ranges, HS-digit levels are named constants at module top or function defaults.
- **Vectorize** — avoid `iterrows()` on the microdata; use groupby/merge/numpy. The Chinese export data is large.

## 5. Domain conventions

| Task | Library | Note |
|------|---------|------|
| Panel data | `pandas` | Use categorical dtype for firm_id / hs_code / destination to save memory |
| Large reads | `pyarrow` / `pandas.read_parquet` | Chunk raw ingestion if a single file exceeds memory |
| Bipartite networks | `networkx` (or `igraph` for speed) | Pin node ordering — see §6 |
| Community detection | `networkx` / custom BRIM | Modularity-based; document the null model |
| Stats | `scipy.stats`, `statsmodels` | Heavy econometrics goes to Stata, not Python |
| Figures | `matplotlib` (+ `seaborn`) | Publication discipline in §7 |

## 6. Numerical & RNG discipline

- **Seed every stochastic component from the same `SEED`.** Community detection (BRIM, Louvain), bootstrap, train/test splits all take an explicit seed. A pipeline with one un-seeded RNG is not reproducible.
- **`numpy.random.default_rng(SEED)`** is the modern interface — prefer it over the legacy global `np.random.seed`. If a library only accepts an int seed, pass `SEED` (or a derived int), not a fresh call.
- **Pin node/edge ordering** in networkx before any algorithm whose output depends on iteration order — `sorted(G.nodes())`. Graph iteration order is insertion-order in modern networkx but algorithm internals can still surface nondeterminism.
- **Float comparison** — never `==` on floats; use `np.isclose`. RCA thresholds: be explicit whether the cutoff is `>= 1` or `> 1`.
- **Missing values** — decide explicitly per column: drop, zero-fill, or propagate. Document the choice. `NaN` silently propagates through arithmetic and breaks group sums.

## 7. Figure discipline (publication-ready)

The user requires polished, publication-ready visuals. Every figure:

- Exported as **both** `fig_name.pdf` (vector, for the paper) **and** `fig_name.png` (`dpi=300`, for slides).
- Axis labels, tick labels, legend ≥ 10 pt. No default matplotlib title clutter; captions live in LaTeX.
- Colorblind-safe palette (e.g. `seaborn` `colorblind`, or viridis for sequential). No red/green contrasts as the sole signal.
- Tight layout (`fig.savefig(..., bbox_inches="tight")`), no whitespace borders.
- One figure = one `def make_fig_xxx() -> Figure` function in `06_describe.py` (or a `figures.py` in `lib/`), so figures regenerate deterministically.
- Save through a single helper that writes both formats:

```python
def save_fig(fig, name: str, out: Path = OUT) -> None:
    """Write a figure as vector PDF (paper) and 300-dpi PNG (slides)."""
    fig.savefig(out / f"{name}.pdf", bbox_inches="tight")
    fig.savefig(out / f"{name}.png", dpi=300, bbox_inches="tight")
```

## 8. Environment reproducibility

- Commit a `requirements.txt` (pip) or `environment.yml` (conda) with **pinned** versions. Regenerate on every dependency change.
- The pinned env + `sessionInfo.txt` is the Python analogue of Stata's `sessionInfo.txt` and R's `sessionInfo()`.
- Do not commit the virtualenv / conda env directory — gitignore it.

## 9. Common Python traps

| Trap | Fix |
|------|-----|
| `df["col"]` chained assignment (`SettingWithCopyWarning`) | Use `.loc[mask, "col"] = ...`; take explicit `.copy()` after a filter |
| Integer firm IDs read as float (NaN coercion) | Read with `dtype={"firm_id": "string"}` or `Int64` (nullable) |
| `groupby().sum()` silently dropping NaN groups | Set `dropna=False` when missing keys are meaningful |
| `merge` exploding rows on duplicate keys | Validate with `validate="1:1"` / `"m:1"` — fail loud on unexpected cardinality |
| numpy vs `random` vs library RNG all un-coordinated | Derive every seed from the single `SEED` constant (§6) |
| `read_csv` re-inferring dtypes differently per chunk | Pass explicit `dtype=`; for big files use parquet after first clean read |
| Mutating a DataFrame passed into a function | Treat inputs as immutable; return a new frame, or document in-place mutation |
| Float RCA cutoff ambiguity | Name the constant and the comparison operator; test the boundary case |

## Enforcement

- [`/data-analysis`](../skills/data-analysis/SKILL.md) is R-oriented; for Python pipelines, follow this rule directly and verify with `ruff check scripts/python`.
- [`/audit-reproducibility`](../skills/audit-reproducibility/SKILL.md) reads `.parquet` / `.csv` outputs alongside R `.rds` and Stata `.dta` for numeric-claim verification.
- A Python-specific code reviewer is on the v2.0 backlog; until then, request review explicitly.

## Cross-references

- [`r-code-conventions.md`](r-code-conventions.md) — analogous discipline for R.
- [`stata-code-conventions.md`](stata-code-conventions.md) — analogous discipline for Stata (the econometrics layer).
- [`replication-protocol.md`](replication-protocol.md) — tolerance contract across R / Stata / Python.
- [`exploration-folder-protocol.md`](exploration-folder-protocol.md) — where experimental Python work lives before graduating to `scripts/python/`.
