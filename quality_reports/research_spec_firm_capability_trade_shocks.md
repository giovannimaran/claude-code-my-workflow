# Research Specification: Firm-Level Capability Transformation under Trade Shocks

**Date:** 2026-06-03
**Researcher:** Giovanni Maran (University of Trento & Freie Universität Bozen)
**Paper type:** reduced-form (shift-share / Bartik exposure + two-way FE panel + event study)
**Status:** APPROVED scope (Decision 1 = A, fused causal paper; Decision 2 = temporal-coupled partition as clean benchmark — see ADR-0001)

> Synthesizes the researcher's own drafts `chapter1_Maran` (2026-02-02) and `Maran_Resproj1` (2026-01-27) with the supporting literature in `master_supporting_docs/supporting_papers/`. This is an *execution* spec, not a from-scratch design — the conceptual work is mature.

---

## Research Question

Does exogenous exposure to adverse trade-policy (tariff) shocks cause exporting firms to **reinforce their existing capability core** (within-core adjustment) or to **reorient toward activities outside their current capability set** (out-of-core adjustment) — and is this response amplified or constrained by the **strategic dependence** of the firm's regional production system?

Formally: the effect of an exogenous increase in tariffs faced by a firm's export basket on (i) **out-of-block diversification** `d_out`, (ii) **in-block diversification** `d_in`, and (iii) **`Share_core`** — the De Stefano (2025) in/out diversification measures. (Note: earlier drafts called these "Fitness_out/core"; the intended objects are De Stefano's diversification counts, not a fitness decomposition. EXPY enters as a product-sophistication control.)

## Motivation

Trade integration raised efficiency but also exposure to policy-driven disruption, making firm resilience and structural transformation central industrial-policy concerns. The existing trade-policy-shock literature (Topalova 2011; Pavcnik 2002; Amiti 2007; Bas 2017; Brandt 2017; Fajgelbaum 2020/2024) measures adjustment almost entirely through **performance** outcomes — exports, employment, productivity, survival. It is far less clear how shocks reshape the **underlying architecture of productive knowledge** — which products a firm retains, drops, or newly enters, and whether that reconfiguration deepens a coherent core or pushes into new capability bundles.

The economic-complexity literature (Hidalgo & Hausmann; the Fitness–Complexity line of Tacchella/Cristelli/Pugliese; De Stefano 2025 at the firm level) supplies tools to *measure* capability structure, but is predominantly **descriptive and macro/region-level**. A structural divergence motivates the bridge: country–product networks are *nested*, whereas **firm–product networks are block-modular** — firms cluster in coherent capability blocks. This paper exploits that divergence to adapt complexity tools to a firm-level causal setting.

The contribution sits in the gap between the two literatures: **no work links a predetermined trade-policy shock to firm-level capability reconfiguration (core vs. out-of-core fitness) within a block-modular firm–product export network**, nor conditions that response on regional strategic dependence (the EU "strategic-dependency" literature: EUC 2021; JRC 2025; Arjona 2023; Korniyenko 2017; Barbieri 2024). The core-vs-out-of-core tension is the firm-trade analogue of March's (1991) exploitation–exploration.

## Hypothesis

Trade-policy shocks induce capability reallocation whose **direction is theoretically ambiguous**:
- **H1 (retrenchment):** adverse tariff shocks raise `Share_core` / `d_in` relative to `d_out` — firms retreat to the coherent core (relatedness / lock-in prediction). Per De Stefano, this is the *growth-negative* direction.
- **H1′ (exploration):** adverse shocks raise `d_out` / lower `Share_core` — firms adaptively search beyond the core (dynamic-capabilities prediction; De Stefano's *growth-positive* direction).
- **H2 (moderation):** the response is amplified (toward retrenchment, less room to upgrade) in regionally **more strategically dependent** systems — `β₂` on `TariffShock × ExpDep` is signed accordingly.

Expected magnitudes: modest on average, **heterogeneous** by exposure, firm size/age/ownership, and regional dependence.

## Empirical Strategy

**Method:** Bartik / shift-share tariff exposure with two-way (firm + year) fixed effects, progressively saturated, plus an event-study for dynamics and pre-trends.

**Outcome construction (the complexity machinery):**
1. Firm–product export matrix `X_t = {x_ipt}`; binarize via RCA: `M_ipt = 1{RCA_ipt > 1}` (Balassa). *Robustness: BiWCM entropy-maximizing null (Bruno 2023) instead of raw RCA>1.*
2. Bipartite graph `G = (I, P, E)`; partition by **BRIM** (Barber 2007) maximizing bipartite modularity `Q`.
3. **Temporal-coupled partition (Decision 2, ADR-0001):** estimate a **multilayer/temporal** partition with inter-layer coupling (ω) so block identities are *consistent across years* and the algorithm cannot relabel spuriously → year-indexed `b_t(i)`, `b_t(p)`. The coupling makes a measured out-of-core jump a *real* firm movement against a stable benchmark, not label churn. **Causal-design guard:** anchor each firm's *home block at baseline* (pre-shock) and measure post-shock products in/out of that baseline-anchored block, so the causal `δ` stays predetermined while block definitions track temporally. Robustness: contrast frozen pooled partition + sensitivity to ω. See `quality_reports/decisions/2026-06-03_partition-frozen-vs-temporal.md`.
4. **PRIMARY OUTCOMES** (De Stefano eq. 4): in-block `d_in_it = Σ_p M_ipt δ_ipt`, out-of-block `d_out_it = Σ_p M_ipt (1−δ_ipt)`, `Share_core_it = d_in/(d_in+d_out)`. (δ time-indexed under the temporal partition + baseline anchoring; see step 3.)
5. **Control:** `EXPY_it = Σ_p E_ipt·logPRODY_p / Σ_p E_ipt` (product sophistication). *Optional/secondary:* a fitness-based lens only if motivated — De Stefano Appendix C found country-level complexity unpredictive of firm growth, so it is NOT a primary outcome.

**Treatment:** `TariffShock_it = Σ_{p} s^X_{i,p,pre} · ln(1+Tariff_pt)` (chapter1 uses the product–destination form `Σ_{p,d} s_{i,p,d,0} Δln(1+τ_pdt)`). Pre-shock shares `s_{i,p,pre}` frozen over a baseline window → exposure predetermined.

**Moderator:** `ExpDep_i = Σ_p s^X_{i,p,pre} · Dep_{r(i),p,pre}`, where regional strategic dependence `Dep_{r,p,t}` is built from import-side concentration (HHI of origins), extra-EU reliance, and low-substitutability proxies (UN COMTRADE).

**Estimating equations:**
```
Y_it = α_i + γ_t + β₁ TariffShock_it + X'_{i0} θ + ε_it                              (baseline)
Y_it = α_i + γ_t + β₁ TariffShock_it + β₂ (TariffShock_it × ExpDep_i) + X'_{i0} θ + ε_it  (heterogeneity)
```
with `Y_it ∈ {d_out, d_in, Share_core}` (diversification counts logged à la De Stefano; EXPY as control covariate).

**Key identifying assumption:** conditional on FE and predetermined controls, firms with different baseline exposure would have followed **parallel trends** in capability outcomes absent the tariff changes.

**Saturation:** add Industry×Year (HS2×year / NACE×year) and Region×Year (NUTS2×year) FE → identification from within-region, within-sector differences in predetermined exposure.

**Robustness / validation checks:**
- Event-study leads/lags; test baseline exposure does not predict pre-period outcome changes; placebo "pseudo-shocks" in pre-period.
- Vary baseline window for `s_pre`; cap influence of dominant `(p,d)` cells; level vs. `Δln(1+τ)`.
- Policy-endogeneity: importer×year FE; drop lobbying-prone sectors; alternative tariff episodes.
- **Shift-share inference** (Adão 2022): exposure-robust SEs; cluster at firm + a shock-relevant level (destination / broad product group).
- Alternative link definition (BiWCM); alternative community algorithm (Louvain/Newman) as partition robustness; **temporal partition as a robustness check** (relaxes Decision 2).

## Data

- **Primary:** Chinese firm-level export microdata, 2000–2015, at firm × product (HS, HS6→HS4) × destination. Fields: firm ID, product value, HS code, destination country. *Not yet in repo; lands gitignored under `data/raw/`.*
- **Tariffs:** **Teodora Teti's global tariff dataset** (`Teti_2024.pdf` = CESifo WP 11590, 86pp — likely "30 Years of Trade Policy / ~5.7bn tariffs"; `Teti_2025.pdf` = CESifo WP 12179 follow-on). Replaces UNCTAD TRAINS — broader, harmonized, gap-filled bilateral coverage (HS product × importer × exporter × year). ⚠️ TO CONFIRM on full read (deferred — context limit): applied vs MFN, HS vintage, ad-valorem vs specific, and coverage of China + its destinations over 2000–2015.
- **Strategic dependence:** UN COMTRADE imports (origin concentration, extra-EU reliance, substitutability).
- **Setting note:** China 2000–2015 brackets **WTO accession (Dec 2001)** — Brandt 2017 is the natural shock/setting anchor; the design generalizes to other tariff episodes in the window.
- **Key variables:** treatment `TariffShock_it`; moderator `ExpDep_i`; outcomes `Fitness_core/out`, `Share_core`; controls `X_i0` (size, age, ownership incl. state-ownership).
- **Unit / sample:** firm-year panel of exporters observed across the window; N TBD on data ingest.

## Expected Results

Average effects modest; sign of the core-vs-out-of-core shift is the empirical question (H1 vs H1′). Strong prior that **heterogeneity dominates**: more dependent regions and smaller/younger firms retrench; larger/more-productive firms have more scope to explore (Zhu et al. 2017 path-breaking; Penrose/Teece dynamic capabilities). Event study should show flat pre-trends and post-shock divergence in `Share_core`.

## Contribution

First firm-level causal link from a predetermined trade-policy shock to **capability reconfiguration** — core vs. out-of-core fitness in a block-modular firm–product network — moving beyond exports/TFP outcomes, and conditioning the response on a novel regional **strategic-dependence** moderator. Bridges firm-trade (Melitz/Bernard multi-product exporters; sequential-exporting: Morales 2019, Albornoz 2012/2016, Conconi 2016) with firm-level economic complexity (De Stefano 2025).

## Open Questions

*(Resolved against De Stefano 2025 — full synthesis in `quality_reports/destefano2025_synthesis.md`.)*

- [x] **Destination dimension** — RESOLVED: De Stefano is pure firm–product (HS), no destination. Firm–product–destination *tensor* = second-stage extension; destination enters this paper only via tariff/dependence weights.
- [x] **Outcome choice — RESOLVED (ii).** Lead with De-Stefano-faithful **in-block / out-of-block diversification** (`d_in`, `d_out`, `Share_core`) + EXPY control. Clarified: "Fitness_out/core" in earlier drafts was just terminology for these diversification counts — there was no separate fitness decomposition. Fitness-based lens demoted to optional/secondary (De Stefano Appendix C: complexity unpredictive of growth).
- [ ] **Temporal partition is a departure from De Stefano** (who froze the pooled partition). ADR-0001's temporal-coupled choice is novel — strengthens methods contribution but Giovanni must build/defend the coupling; no recipe inherited.
- [ ] **WTO-accession framing.** Foreground 2001 accession (Brandt 2017) vs. full 2000–2015 tariff variation.
- [ ] **Sample / firm-ID continuity.** De Stefano keeps only firms exporting *every* year (balanced) — too restrictive for entry/exit-heavy Chinese customs data; define a looser panel rule.
- [ ] Block reconfiguration over time (point (b)) — parked as second paper + temporal-partition robustness.

## Verification note (citations)

All author–year citations in this spec correspond to PDFs **physically present** in `master_supporting_docs/supporting_papers/{Papers,new_papers}/` (verified by filename). Specific *finding* attributions (e.g., what Topalova 2011 or De Stefano 2025 precisely show) are drawn from the researcher's own framing drafts and standard knowledge and are flagged **UNVERIFIED at the finding level** — to be confirmed on full read before any of this text migrates into the manuscript. Per-session policy: no verifier subagent spawned (citations are repo-grounded, not retrieved).
