# De Stefano et al. 2025 — synthesis & implications for the spec

**Paper:** "From macro to micro: Economic complexity indicators for firm growth." De Stefano, Mula, Mariani, Zaccaria. Preprint → Research Policy, arXiv:2507.21754v1 (29 Jul 2025). Read in full 2026-06-03.

## What the paper actually does

- **Data:** ISTAT Italian firm exports 1993–2017 (18,597 firms kept = those exporting ≥1 product *every* year), HS6 = 5,203 products; + ORBIS financials from 2013 (12,852 firms). Outcomes = **Growth** (4-yr log-growth of smoothed operating revenue) and **Profit per Employee**.
- **Three indicator classes:**
  1. **EXPY_f** = `Σ_p E_fp·logPRODY_p / Σ_p E_fp` (export-weighted avg product productivity). `logPRODY_p = Σ_c RCA_cp·lnGDP_c / Σ_c RCA_cp`, z-scored. Built from the **country**-product network + GDP — NOT firm-internal.
  2. **In-block / out-of-block diversification** (the headline construct): RCA-binarize `M_fp = 1{RCA_fp>1}`; **BRIM (Barber 2007)** on the *pooled* firm-product graph → 7 blocks (Q=0.501); `δ_fp = 1{block(f)=block(p)}`; `d_in = Σ_p M_fp δ_fp`, `d_out = Σ_p M_fp(1−δ_fp)`. **Identical to chapter1's d_core/d_out.**
  3. **Coherence** `C_f = Σ E_fp E_fp' B_pp' / Σ E_fp E_fp'` using **Sapling Similarity** B (Albora 2023a) — used as a control.
- **Regression = cross-sectional, NOT panel FE:** time-average to `Y_{f,t*+Δt} = βX_{f,t*} + γ·D^(s)_f + η`, t*=2015, Δt=4, 21 HS sector dummies, robust (HC1) SE. Associational/predictive, no causal identification.
- **Headline results:** out-of-block div **+** on Growth (β=0.016, p<0.001); in-block div **−** on Growth (β=−0.014, p=0.004); EXPY **+** on both; Coherence **+** on Profit/Employee only. Maps March (1991) **exploration (out) vs exploitation (in)**. BRIM blocks essential — HS-sector blocks give insignificant results (Table 2).

## Implications — resolves 3 open questions in the spec

1. **No "Fitness_core / Fitness_out" exists in De Stefano.** Their outcomes are EXPY + in/out **diversification counts** + Coherence. **Appendix C explicitly shows product COMPLEXITY (Tacchella fitness) is NOT associated with firm growth** — "firms' performance is largely independent of their exported products' complexity." So chapter1's `Fitness_core/out` is **Giovanni's own extension, and De Stefano is a cautionary data point against it.** → DESIGN QUESTION for Giovanni: keep the `Fitness_core/out` decomposition (novel, but country-level complexity didn't predict growth in De Stefano), or use De-Stefano-faithful outcomes (`d_in`/`d_out` diversification counts, `Share_core`, EXPY) as primary and treat fitness as secondary?
2. **Partition: De Stefano FROZE it** (Appendix B — pooled/time-averaged graph, firms present all years, RCA>1, because yearly BRIM "varies slightly over time, undesirable for longitudinal analysis"). → Giovanni's **temporal-coupled partition (ADR-0001) is a genuine methodological departure from the framework paper**, not a given. Strengthens the methods contribution but is on Giovanni to build/defend; De Stefano offers no temporal recipe.
3. **No destination dimension** — pure firm-product (HS). Confirms firm-product-**destination tensor = second-stage extension**; destination enters this paper only via tariff/dependence weights.

## Other transferable specifics

- 4-digit vs 6-digit communities: robust (they use HS4 blocks). EXPY weights export-vol vs RCA: robust.
- Sapling Similarity (Albora 2023a) is their coherence kernel — candidate control for Giovanni too.
- Sample rule "firms exporting every year" → balanced panel; relevant to spec open-Q on Chinese firm-ID continuity, but very restrictive on Chinese customs data (entry/exit heavy) — Giovanni may need a looser rule.
- Giovanni's causal panel-FE + shift-share tariff design is **more rigorous than De Stefano's cross-sectional associational design** — clear contribution delta: De Stefano = "does export structure *predict* growth"; Giovanni = "does an exogenous tariff shock *cause* core↔out reconfiguration."
