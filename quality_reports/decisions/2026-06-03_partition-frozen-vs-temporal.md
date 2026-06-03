# ADR-0001: Block partition — temporal-coupled (clean benchmark) vs. frozen vs. independent-yearly

**Status:** ACCEPTED
**Date:** 2026-06-03 (revised same day after researcher refinement)
**Context:** `/interview-me` — research spec for "Firm-Level Capability Transformation under Trade Shocks" (Decision 2 of the scope interview)

## Problem

The outcome variables (`Fitness_core`, `Fitness_out`, `Share_core`, `d_core`, `d_out`) depend on a block partition of the firm–product bipartite network via the consistency indicator `δ_ip = 1{b(i)=b(p)}`. Running BRIM separately each year yields slightly different, **relabeled** partitions, so "a firm moved out of its core" is confounded with "the algorithm redrew the block boundary." The partition's time-handling must be fixed before any outcome is computed. **Requirement (researcher):** keep the core/out decomposition and diversification measures, but guarantee a measured out-of-core *jump* reflects real firm movement against a stable benchmark — NOT algorithmic relabeling.

## Options considered

### Option A: Frozen pooled partition
BRIM once on the pooled `M̄` → one fixed `b(i)`, `b(p)` for all years.
**Pro:** `δ_ip` predetermined; zero relabeling by construction; simplest to defend as exogenous.
**Con:** Assumes away genuine structural change over 2000–2015 (a window spanning WTO accession). If the capability map truly shifted, a frozen partition mismeasures early/late years and can mislabel real moves.

### Option B: Temporal / multilayer community detection with inter-layer coupling  ★ CHOSEN
Yearly partitions estimated jointly with a cross-time coupling term (multilayer modularity, Mucha et al. 2010 style; coupling ω) so block identities are **consistent across years** and evolve only when the data demand it. Algorithmic relabeling is suppressed by the coupling; genuine evolution is preserved.
**Pro:** Provides a *temporally-consistent, stable benchmark* → a measured jump is a real firm movement, not label churn. Honest about a 15-year window. Directly satisfies the researcher's requirement.
**Con:** Partition is now time-varying, so `δ_ipt` is no longer mechanically predetermined → must guard against the partition responding to the same shocks (see Consequences for the baseline-anchoring fix). Heavier to implement and tune (coupling ω is a researcher degree of freedom).

### Option C: Independent yearly partitions
BRIM each year, no coupling.
**Pro:** Simplest "dynamic" option.
**Con:** Maximal relabeling instability; longitudinal `δ_ip` essentially uninterpretable. The exact failure mode the requirement rules out.

## Decision

**Chose:** Option B — temporal/multilayer community detection with inter-layer coupling, used as a **clean measurement device** (not as an object of study).

**Rationale:** The researcher wants the decomposition + diversification measures AND a guarantee that an out-of-core jump is real. A frozen partition (A) buys cleanliness by assuming no structural change — too strong across WTO accession. Independent yearly partitions (C) reintroduce exactly the relabeling confound to be avoided. The temporal-coupled partition (B) threads the needle: the coupling term suppresses spurious algorithmic relabeling so block identities are trackable across years, while still permitting genuine evolution — so the jump is measured against a stable, temporally-consistent benchmark. NOTE: this is the *opposite motivation* from studying block reconfiguration as a contribution — the temporal network here is instrumentation for a clean measure, not the research object.

## Consequences

- `scripts/python/05_community.py` implements multilayer/temporal BRIM (or temporal modularity with coupling ω), producing a year-indexed but identity-consistent partition `b_t(i)`, `b_t(p)`.
- **Causal-design guard (important):** because the partition is now time-varying, define each firm's **home block at baseline** (pre-shock window) and measure post-shock whether its products fall in vs. out of that *baseline-anchored* block — so the benchmark for the causal `δ` stays predetermined even though block *definitions* are tracked temporally. Resolve the exact anchoring rule at implementation; document as an identification assumption.
- Tuning obligation: report sensitivity to the coupling parameter ω, and contrast against the frozen partition (Option A) and alternative algorithms (Louvain/Newman) + alternative link definition (BiWCM vs RCA>1) as robustness.
- Block reconfiguration over time (researcher's point (b)) remains a candidate **second paper**; here we only borrow the temporal machinery for measurement.

## Rejected alternatives — why not

- **Option A (frozen):** Buys cleanliness by assuming away structural change over a 15-year, accession-spanning window; retained only as a robustness check.
- **Option C (independent yearly):** Relabeling instability makes longitudinal `δ_ip` uninterpretable — the precise confound the researcher's requirement forbids.
