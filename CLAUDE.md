# CLAUDE.MD -- Academic Project Development with Claude Code

**Project:** Firm-Level Export Diversification and Capability Reconfiguration
**Institution:** University of Trento
**Branch:** main

---

## Core Principles

- **Plan first** -- enter plan mode before non-trivial tasks; save plans to `quality_reports/plans/`
- **Verify after** -- compile/render and confirm output at the end of every task
- **Single source of truth** -- paper LaTeX is authoritative; slides are presentation derivatives
- **Quality gates** -- nothing ships below 80/100
- **[LEARN] tags** -- when corrected, save `[LEARN:category] wrong → right` to [MEMORY.md](MEMORY.md)

Cross-session context lives in [MEMORY.md](MEMORY.md); past plans, specs, and session logs are in [quality_reports/](quality_reports/).

---

## Tool Stack

| Tool | Role |
|------|------|
| Python | Primary: data cleaning, network construction, RCA, community detection, figures |
| Stata | Econometric analysis: FE regressions, robustness tables, DiD / event-study |
| R | Occasional: specific packages, alternative robustness, publication-quality figures |
| LaTeX | Manuscript (`paper/`) and presentations (`Slides/`) |

---

## Folder Structure

```
my-project/
├── CLAUDE.md
├── .claude/                     # Rules, skills, agents, hooks
├── Bibliography_base.bib        # Centralized bibliography
├── Figures/                     # Publication-ready figures
├── Preambles/header.tex         # LaTeX headers
├── Slides/                      # Beamer .tex for presentations
├── Quarto/                      # RevealJS .qmd derivatives
├── paper/                       # LaTeX empirical manuscript
├── data/                        # GITIGNORED: raw/, processed/, intermediate/
├── scripts/
│   ├── python/                  # Main pipeline (numbered 00–99)
│   ├── stata/                   # Econometric regressions, FE, robustness
│   └── R/                       # Occasional use
├── explorations/                # Research sandbox (see rules)
├── docs/                        # GitHub Pages (auto-generated)
├── quality_reports/             # Plans, session logs, merge reports
├── templates/
└── master_supporting_docs/      # Reference papers and supporting slides
```

---

## Commands

```bash
# Python pipeline (from repo root)
python scripts/python/00_run_all.py
python scripts/python/01_load.py       # ingest raw microdata
python scripts/python/02_clean.py      # firm-product-destination panel
python scripts/python/03_rca.py        # RCA-based product links
python scripts/python/04_network.py    # firm-product bipartite networks
python scripts/python/05_community.py  # BRIM community detection
python scripts/python/06_describe.py   # descriptive stats + figures

# Stata (from repo root)
stata -b do scripts/stata/99_run_all.do

# LaTeX (3-pass, XeLaTeX only)
cd Slides && TEXINPUTS=../Preambles:$TEXINPUTS xelatex -interaction=nonstopmode file.tex
BIBINPUTS=..:$BIBINPUTS bibtex file
TEXINPUTS=../Preambles:$TEXINPUTS xelatex -interaction=nonstopmode file.tex
TEXINPUTS=../Preambles:$TEXINPUTS xelatex -interaction=nonstopmode file.tex

# Deploy Quarto to GitHub Pages
./scripts/sync_to_docs.sh LectureN

# Quality score
python scripts/quality_score.py Quarto/file.qmd

# Palette sync (LaTeX ↔ SCSS)
./scripts/check-palette-sync.sh
```

---

## Quality Thresholds (advisory)

| Score | Checkpoint | Meaning |
|-------|------|---------|
| 80 | Commit | Good enough to save |
| 90 | PR | Ready for deployment |
| 95 | Excellence | Aspirational |

Enforced by `/commit` (halts + asks for override); not enforced by a git pre-commit hook.

---

## Skills Quick Reference

| Command | What It Does |
|---------|-------------|
| `/compile-latex [file]` | 3-pass XeLaTeX + bibtex |
| `/deploy [LectureN]` | Render Quarto + sync to docs/ |
| `/extract-tikz [LectureN]` | TikZ → PDF → SVG |
| `/new-diagram [snippet] [output.tex]` | Scaffold a TikZ diagram from gallery |
| `/proofread [file]` | Grammar/typo/overflow review |
| `/visual-audit [file]` | Slide layout audit |
| `/review-r [file]` | R code quality review |
| `/validate-bib` | Cross-reference citations |
| `/commit [msg]` | Stage, commit, PR, merge |
| `/lit-review [topic]` | Literature search + synthesis |
| `/research-ideation [topic]` | Research questions + strategies |
| `/interview-me [topic]` | Interactive research interview |
| `/review-paper [file]` | Manuscript review (single-pass / `--adversarial` / `--peer <journal>`) |
| `/respond-to-referees [report] [manuscript]` | R&R cross-reference + response draft |
| `/seven-pass-review` | Seven-pass adversarial manuscript review (parallel forked subagents) |
| `/verify-claims [file]` | Chain-of-Verification fact-check (forked verifier, fresh context) |
| `/data-analysis [dataset]` | End-to-end R analysis pipeline |
| `/stata-replication [paper-or-data]` | End-to-end Stata pipeline scaffold |
| `/audit-reproducibility [paper]` | Enforce replication tolerance thresholds on paper ↔ code |
| `/simulation-study [estimator+DGP]` | Reproducible Monte Carlo study |
| `/preregister [--style osf|aspredicted|aea-rct]` | Draft a preregistration document |
| `/humanize [file]` | Detect AI-voice tells in academic prose |
| `/checkpoint [topic]` | Save structured state snapshot |
| `/compress-session [slug]` | Distil session before auto-compaction |
| `/context-status` | Show session health + context usage |
| `/deep-audit` | Repository-wide consistency audit |
| `/r-package-check [pkg path]` | R package release gate |
| `/promote-memory [filter]` | Five-critic council on [LEARN] entries |

---

## Beamer Custom Environments

*TBD — update once the presentation theme is finalized.*

## Quarto CSS Classes

*TBD — update once the Quarto theme is finalized.*

---

## Current Project State

| Artifact | Path | Status |
| --- | --- | --- |
| Empirical paper | `paper/` | Not started — run `/interview-me` to formalize research spec |
| Presentation slides | `Slides/` | Reference PDF exists (`Empirical_presentation copia.pdf`) — source .tex TBD |
