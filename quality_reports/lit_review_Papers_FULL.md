# Full-Read Literature Review — `Papers/` folder

**Project:** Firm-Level Export Diversification and Capability Reconfiguration (University of Trento)
**Method:** Each paper read in full from the PDF, then synthesised at finding level (Main contribution / Data & method / Key findings / Relevance to project). No finding is recorded unless the PDF was actually read this session (repo anti-hallucination rule).
**Tracker:** `quality_reports/lit_review_Papers_full_PLAN.md`
**Companion syntheses already on disk:** `destefano2025_synthesis.md`, `teti2024_tariff_synthesis.md`.

---

## Batch 1 — Firm-level EFC core

### Sub-batch 1a — Firm-level fitness / complexity-metric cluster *(read 2026-06-03)*

This cluster establishes the central methodological problem the project must confront: **the standard country-level Economic Fitness & Complexity (EFC) toolkit does not transfer cleanly to firm-level export data.** All three papers come from the Pietronero/Saracco/Squartini/Zaccaria complexity-physics school and use Italian or Colombian firm-export microdata classified in the Harmonized System.

---

#### Laudati, Mariani, Pietronero & Zaccaria (2023) — *The different structure of economic ecosystems at the scales of companies and countries*
*J. Phys. Complex. 4, 025011 (main text 12 pp + supplement 9 pp, both read in full).*

**Main contribution.** Shows that the *structure* of the bipartite export network is qualitatively different at the country vs. the firm scale, and that this difference breaks the standard Fitness-Complexity (FC) ranking algorithm at the firm level. Country-product networks are **globally nested**; firm-product networks are **in-block nested** (modular, with nestedness only *within* sector blocks).

**Data & method.** Unique ISTAT dataset of Italian firms' exports, 1993–2017 (879,280 firms; after keeping firms active the whole interval, **18,349 firms × 1,233 products**), compared against a UN-COMTRADE country dataset (161 countries × 1,242 products), both HS-1992 at 4 digits (~1,200 products). RCA ≥ 1 binarisation (Balassa). Methods: FC algorithm; Barber bipartite modularity via **BRIM** (and BRIM², BiLouvain); **in-block nestedness** quality function I vs. global nestedness N (Solé-Ribalta/Mariani/Tessone framework); BiCM null model for significance; AMI to compare detected partitions against HS sections/chapters; logPRODY as an external monetary sophistication benchmark.

**Key findings.**
- FC product-complexity ranking correlates with logPRODY for countries (ρ = 0.642) but **anti-correlates for firms (ρ = −0.224)**. Fitness vs. export-volume: ρ = 0.887 (countries) vs. only 0.378 (firms). Fitness vs. diversification: ρ = 0.969 (countries) vs. 0.565 (firms). → FC mis-estimates product value and firm competitiveness when applied to the whole firm-product network.
- Both networks are "modular" by Q (country Q = 0.218, firm Q = 0.512, both p < 0.01 under BiCM), but the firm blocks are clean (>70% of links inside blocks, AMI vs. HS ~270% higher than countries) while country blocks are noisy (~50% of links) and heterogeneous.
- In-block nestedness ratio I*/N ≈ **12.0 for firms** (>80 blocks) vs. **≈1.02 for countries** (2 blocks, the larger holding 97.6% of nodes). Conclusion: nestedness is **global for countries, local for firms.**
- Country modularity is an artefact of diversification, not specialisation (supplement §IIIB: blocks track Fitness/Complexity/ubiquity gradients, huge within-block heterogeneity; HSSec/HSChap modularity near zero for countries).

**Relevance.** This is arguably the **anchor paper** for the project's methods chapter. It (i) justifies abandoning whole-network FC for firms, (ii) motivates detecting *local ecosystems* (firm + competitors + contested products) as the right unit, (iii) supplies the exact algorithmic stack (RCA → BRIM/IBN → BiCM validation → AMI vs. HS) the project's Python pipeline (`03_rca`→`05_community`) is already structured around, and (iv) provides Italian-ISTAT scale benchmarks to sanity-check our own panel. The author's margin notes on the PDF (use logPRODY as benchmark/robustness; question whether pseudo-NODF could measure nestedness; BRIM vs. BiLouvain/IBN robustness) are live design questions for our own chapter.

---

#### Bruno, Saracco, Squartini & Dueñas (2018) — *Colombian Export Capabilities: Building the Firms-Products Network*
*Entropy 20, 785 (17 pp, read in full).*

**Main contribution.** First (self-described "pioneering") full entropy-based network analysis of a national **firm-product** export network, showing it is strongly **modular/block-structured** — in sharp contrast to the triangular/nested World Trade Web (WTW) — and that the FC algorithm therefore loses predictive power at the firm level. Effectively the empirical precursor to Laudati 2023's in-block-nestedness result.

**Data & method.** Colombian customs (DIAN/DANE) manufacturing exports 2010–2014; bipartite firm-product binary network (HS-2007/2012 at 6 digits; ~3,100 products, ~4,800–5,100 firms/yr, ~2,240 persistent firms). Benchmark: BACI WTW (~140 countries, ~1,131 products). Methods: RCA filtering; **BiCM** entropy null model; statistically **validated monopartite projections** (Saracco et al. co-occurrence method, Poisson-Binomial p-values + **FDR** correction); Barber bipartite modularity + Louvain on projections; **NODF** nestedness with z-scores; degree/strength distributions.

**Key findings.**
- Firm-product matrix is sparse (density ~10⁻³) vs. WTW (0.09–0.13); RCA validates ~90% of firm links but only ~20% of WTW links → little national-scale competition.
- FC reordering reveals a triangular shape, but Barber community detection reveals a **block-diagonal structure underneath** — the FC algorithm *hides* the specialisation/block signal present in firm data. No such block structure appears in the WTW.
- Nestedness z-score steadily ≈ **−11** across 2010–2014: the firm network is **significantly less nested than the BiCM null** (the opposite of the WTW). Degree-fitness Spearman: ~0.40 firms vs. ~0.90 countries; product degree-complexity ~0.65 vs. ~0.73.
- Validated product-projection communities are stable over years and map onto interpretable, homogeneous sectors (clothes, textiles, food, electronics, metals, leather/footwear, etc.); inclusion ~0.85–0.92 vs. Barber bipartite blocks.
- Framing: **countries diversify (massive "species"), firms specialise** within a core set of capabilities — explicitly invoking Penrose/Teece capability theory and economies of scope.

**Relevance.** Provides the **methodological template and an independent (Colombian) replication** of the "firms are modular, not nested" result, plus a concrete, defensible projection+validation pipeline (BiCM → Poisson-Binomial → FDR) the project can adopt for building firm-firm or product-product relatedness networks. Useful as a second-country external-validity anchor alongside the Italian ISTAT evidence.

---

#### Bruno, Mazzilli, Patelli, Squartini & Saracco (2023) — *Inferring comparative advantage via entropy maximization*
*J. Phys. Complex. 4, 045011 (15 pp incl. appendices, read in full).*

**Main contribution.** Re-derives Balassa's **RCA from first principles** as the sparse-regime approximation of an entropy-based **Bipartite Weighted Configuration Model (BiWCM)**, shows RCA is **statistically biased** (its implicit parameters violate the maximum-likelihood condition — the benchmark is not "centered" on the data), and proposes a principled replacement: a proper **p-value-based statistical validation** ("statistically significant comparative advantage") instead of the RCA ≥ 1 thresholding rule.

**Data & method.** COMTRADE exports 2015, HS-2012 (169 countries × 5,206 products; country-level, not firm-level here). Introduces discrete and continuous BiWCM (geometric/exponential weight distributions; closed-form p-value e^{−(θ+η)w*}); "dressed-RCA" MERCAd/MERCAc models; FDR multiple-testing correction (α = 0.05); compares four binarisations (μ/α × MERCA/BiWCM) on link density, nestedness (sNODF), and resulting Fitness/Complexity rankings. Solvers shipped in the `NEMtropy` and `bicm` PyPI packages.

**Key findings.**
- RCA ≡ μ-MERCA = sparse-regime ⟨w⟩ of BiWCMd; but in practice trade is **far from the sparse regime**, so the RCA bias bites.
- **Fitness rankings are robust** to the validation choice (Spearman ρ > 0.8 across all four methods; RCA vs. BiWCM μ = 0.974). **Complexity rankings are not** (ρ as low as 0.48–0.73) — product complexity is the noisy, validation-sensitive quantity.
- BiWCM binarisation yields a **cleaner nested structure** (sNODF >10% higher than plain RCA); statistical (α) validation surfaces an excess of high-complexity products in high-fitness countries' baskets that plain RCA blurs.
- Country diversification survives regardless of validation strictness.

**Relevance.** Directly governs the project's **RCA step**. It tells us (i) our headline fitness-type results are likely safe under RCA, but **product-complexity claims need the BiWCM/p-value treatment for robustness**, (ii) there is an off-the-shelf, citable, reproducible Python implementation (`bicm`, `NEMtropy`) to swap in, and (iii) it gives a rigorous statistical-validation alternative to the ad hoc RCA ≥ 1 cut that referees in this literature increasingly expect. Note: this paper is country-level — applying BiWCM-style validation to *firm* weights is an open extension the project could legitimately claim.

---

**Cross-paper synthesis (sub-batch 1a).** A coherent through-line: (1) Balassa RCA is a biased sparse-regime null (Bruno 2023) — fix with entropy-based validation; (2) once you have a firm-product network, it is **modular/in-block-nested, not globally nested** (Bruno 2018 Colombia; Laudati 2023 Italy) — so (3) whole-network FC is invalid at the firm scale, and the right move is to identify **local nested ecosystems** (sector blocks via BRIM/IBN) and apply complexity tools *within* them. For the Trento project this is the methodological backbone: RCA(+BiWCM robustness) → bipartite network → community/in-block detection → within-block capability metrics. Italian ISTAT (Laudati) is the closest scale/data analogue to our own setting.

**Open threads flagged for later batches.** pseudo-NODF vs. NODF vs. I/N as the nestedness metric (Batch 3: Almeida-Neto, Mariani 2019, Solé-Ribalta 2018); FC convergence/stability (Pugliese 2016/2019, Servedio — Batch 1 remainder & Batch 2); capability-theory grounding of "firms specialise within a core" (Penrose, Teece, Dosi — Batch 4).

---

### Sub-batch 1b — Fitness-Complexity + firm diversification/coherence cluster *(read 2026-06-03)*

This trio moves from the **country-level FC engine** (Pugliese 2017 — what fitness *is* and what it predicts) to its **translation to the firm** via a relatedness/coherence measure (Pugliese 2019 on patents; Dosi 2022 on Indian products). The shared thread: a **capability-based view of the firm**, where coherent (related) diversification — not raw breadth — is what pays. Dosi 2022 is the closest template to the Trento project's own econometrics.

---

#### Pugliese, Chiarotti, Zaccaria & Pietronero (2017) — *Complex Economies Have a Lateral Escape from the Poverty Trap*
*PLoS ONE 12(1): e0168540 (18 pp, read in full).*

**Main contribution.** Adds **economic-complexity Fitness** as a *second dimension* to the classic (one-dimensional, GDP/capital-based) poverty-trap model. Shows that more complex/diversified economies face a **lower GDP-per-capita barrier** to start industrialization — a "lateral escape" — and packages this into a **Complex Index of Relative Development (CIRD)**, a geometric combination of Fitness and GDPpc.

**Data & method.** UN-COMTRADE export data (SITCv2 manufacturing, ~148 countries, HS 4-digit ~1,131 products) + Penn World Table 8.1, 1963–2000. Growth-accounting decomposition of GDPpc growth into input growth (capital, labour participation, human capital) vs. residual TFP; focus on **input growth** as the fingerprint of industrialization. Fitness-Complexity (FC) algorithm (Tacchella 2012) on the RCA-binarised country-product matrix. Non-parametric Gaussian-kernel (Nadaraya-Watson) estimation of input-growth vs. (GDPpc, Fitness).

**Key findings.**
- Pooling all countries, the input-growth-vs-GDPpc curve is muddy; **splitting by Fitness tertiles** reveals two regimes: high-Fitness countries take off at low GDPpc, low-Fitness countries face a much higher barrier.
- The 2-D (Fitness × GDPpc) kernel shows a clear diagonal "escape band"; **CIRD ≈ −2 is a sharp industrialization threshold** (inflection of input-growth).
- Country trajectories: South Korea/Thailand = "lateral escape" (build Fitness first, then GDPpc rises); **China = complementary case** (high Fitness early but extreme poverty kept it one-dimensionally trapped). Robust to a 1995–2010 database (SI).

**Relevance.** This is the **canonical statement of what Fitness predicts at the country level** and why the FC algorithm matters — the macro backdrop against which the firm-level project positions itself. The phase-transition framing (capabilities as latent heat) and the GDPpc↔Fitness complementarity are useful narrative devices. Less directly methodological for a firm panel, but essential for motivating "capabilities drive development" and for citing FC's predictive track record.

---

#### Pugliese, Napolitano, Zaccaria & Pietronero (2019) — *Coherent diversification in corporate technological portfolios*
*PLoS ONE 14(10): e0223403 (22 pp, read in full).*

**Main contribution.** Builds the bridge from country EFC to the **firm** by defining **Coherent Technological Diversification (CTD)** — an *intensive* diversification measure that rewards portfolios decomposable into large blocks of *related* technologies over equally broad but scattered ones — and shows it predicts firm labour productivity, dominating raw (extensive) Technological Diversification (TD).

**Data & method.** ~70,000 patenting firms, AMADEUS (Bureau van Dijk) balance sheets merged with EPO-PATSTAT triadic patent families, 2004–2013; ~7,000 IPC technology groups. Builds firm-technology bipartite matrix M → technology-relatedness matrix B via the **taxonomy-network/Zaccaria-Hidalgo proximity** (co-occurrence normalised by ubiquity); intra-firm coherence γ_ft = Σ B_tt' M_ft'; **CTD Γ_f = average coherence over the firm's technologies** (≈ average size of coherent knowledge blocks ≈ "technologies per production line"). Minimal-spanning-forest filtering for visualization; OLS of log labour productivity on CTD, TD, size.

**Key findings.**
- **CTD is positive and significant in every regression** (1% level), even controlling for size and TD; **TD loses all significance once CTD is included** (TD was just proxying CTD). 3-D plot: productivity rises horizontally with CTD but is flat/slightly negative vertically in TD.
- Striking structural result: the minimal-spanning-forest of B is **not** colour-sorted by IPC section — technologies co-occur because of the *products* they serve (a hidden layer), not technological similarity. This is the **opposite** of the country product-space, where similar products cluster.
- Practical use proposed: evaluating portfolios, recommending M&A partners.

**Relevance.** The **direct methodological ancestor** of the project's relatedness/coherence pipeline — same Hidalgo/Zaccaria proximity, applied to firms, with a clean intensive metric (CTD) and a regression design (coherence vs. performance, controlling for size/diversification) the project can replicate on export-product baskets. Confirms the recurring Batch-1 lesson: at firm scale, **block/coherence structure beats raw diversification**.

---

#### Dosi, Mathew & Pugliese (2022) — *What a firm produces matters: diversification, coherence and performances of Indian manufacturing firms*
*Research Policy 51, 104152 (15 pp, read in full).*

**Main contribution.** Brings the EFC relatedness toolkit into a **rigorous capability-theory econometric design** on a developing-country firm panel, correcting for the **endogeneity of the diversification decision**. Two results: (i) firms that *choose* to diversify gain (treatment-on-treated), but a random firm forced to diversify would not; (ii) **coherence of the product basket raises profitability** (not growth), with strong sector heterogeneity.

**Data & method.** Prowess (CMIE) Indian manufacturing panel, 1995–2015; product-level sales at 6-digit (383 products). Performance = sales growth and *relative* profitability (vs. sector mean). Econometrics: OLS/FE baseline → **Probit "who diversifies"** → **Heckman treatment effect** → **Endogenous Switching Regression** (Maddala) yielding ATT/ATU. Relatedness B_ij = **min-normalised co-occurrence** (Hidalgo 2007 / Zaccaria 2014 proximity, here firm-level) — deliberately the *raw* co-occurrence (economic significance), **not** the statistically-validated Teece/Bottazzi-Pirino τ (Appendix B's coin-flip argument: significance ≠ strength). Coherence C_f = sales-weighted average B_ij over the firm's product pairs. Pavitt (1984) four-taxa sector split.

**Key findings.**
- Diversifiers are **non-random**: larger, older, R&D-intensive, complex processes. Naïve OLS shows multi-product firms *less* profitable; once selection is handled, **ATT ≈ +27% firm growth and +17% profitability** for actual diversifiers, while ATU (untreated forced to diversify) is null/negative.
- **Coherence raises profitability but not growth** (FE) — related products share capabilities → efficiency. Sector heterogeneity: coherence matters for **science-based** (knowledge relatedness) and, more puzzlingly, **supplier-dominated** sectors; not for scale-intensive/specialized.
- In India, ~93% of new products come from **incumbents**, not entrants → "climbing the ladder" via incumbent diversification. Echoes the Dosi et al. (2017) finding that firms "know less than they make" (more product- than technology-diversified).

**Relevance.** The **single most directly transferable paper for the Trento project's empirical chapter.** It supplies (i) the exact relatedness/coherence definitions to compute on a firm-product-export panel, (ii) the *correct* econometric handling of self-selection into diversification (Probit → Heckman → Endogenous Switching, ATT/ATU), (iii) the Pavitt sector-heterogeneity lens, and (iv) the key methodological choice — use **raw co-occurrence (strength)** not statistical-significance relatedness when the question is economic payoff, not "is this link random". Three-author overlap (Dosi/Pugliese) ties it straight back to 1b's other papers and to the capability theory of Batch 4.

---

**Cross-paper synthesis (sub-batch 1b).** The arc: Fitness predicts *country* takeoff (Pugliese 2017) → the same complexity logic, ported to firms, says **coherent (block-structured) diversification, not breadth, drives performance** — in technology space (Pugliese 2019, CTD → productivity) and in product space (Dosi 2022, coherence → profitability). Both firm papers reuse the **Hidalgo/Zaccaria proximity** to build a relatedness matrix B and then aggregate it into a firm-level coherence score — exactly the operation the Trento pipeline needs, but on export products. Two design rules emerge for our own work: (1) prefer an **intensive coherence measure** over raw diversification counts; (2) **instrument/correct for the endogenous diversification decision** (Dosi 2022's switching regression) rather than running naïve OLS. Together with 1a (firms are modular/in-block-nested, FC-as-is fails), Batch 1 now has both the *structural* diagnosis and the *performance* econometrics.

---

### Sub-batch 1c — Country/firm complexity, GVC specialization & subnational fitness

#### Bontadini, Mancini & Marvasi (2021) — *Regional integration, trade specialization and economic performance in GVCs*
*(country-level; read in full, 34 pp.)*

**Main contribution.** Asks whether **what a country produces inside global value chains** — measured through domestic value added (DVA) by technology/knowledge intensity — shapes its macro performance, especially through the crisis. Reframes the "what you export matters" thesis at the **DVA / value-chain** level rather than gross exports.

**Data & method.** Country-sector panel from the **OECD ICIO (Inter-Country Input-Output)** tables; DVA decomposed via the **Leontief inverse** to strip out foreign value added embedded in gross exports. Sectors grouped into **knowledge-intensive business services (KIBS), high-tech manufacturing (HTM), low-tech manufacturing (LTM), and natural resources (NR)**. RCA-style specialization indices computed on DVA shares. **System GMM** (Blundell-Bond) to handle dynamic panel / persistence of specialization and endogeneity.

**Key findings.**
- Specialization in **LTM and NR is negatively associated** with subsequent growth/performance; specialization in **HTM and KIBS is positively associated — but the positive effect is concentrated in the crisis window** (knowledge-intensive specialization gave resilience when demand collapsed).
- The composition of DVA, not the volume of gross exports, is what carries the performance signal — "**what a country produces matters**" survives the GVC/value-added correction.

**Relevance.** Supplies the **value-added / GVC framing** the project can layer on top of gross-export complexity: if Trento's firm panel can be linked to sector DVA intensities, the same KIBS/HTM/LTM/NR lens (and the System GMM dynamic-panel design) transfers directly. Reinforces the through-line that *the qualitative content of the basket* — not its size — predicts performance and resilience to shocks.

#### Operti, Pugliese, Andrade, Pietronero & Gabrielli (2018) — *Dynamics in the Fitness-Income plane: Brazilian states vs World countries*
*PLoS ONE 13(6): e0197616 (20 pp, read in full).*

**Main contribution.** Extends Economic Fitness from countries to **subnational entities** by introducing the **Exogenous Fitness** algorithm: instead of computing product Complexity from the within-country (state) matrix — which is biased by local sparsity — it **borrows the product Complexities Q_p from the world-country Fitness-Complexity fixed point** and uses them to score the states' export baskets. This is the key methodological fix for applying EFC at a scale where the bipartite matrix is too small/sparse for the endogenous algorithm to converge to meaningful *values*.

**Data & method.** Brazilian state exports 2000–2015 (DataViva, from Brazilian ministries); world trade from **BACI/COMTRADE**, HS-2007 4-digit. Step 1: run standard (endogenous) Fitness-Complexity on the world country×product matrix → obtain Q_p. Step 2: **Exogenous Fitness** F_s = Σ_p M_sp Q_p (normalized), using world Q_p on the state×product RCA matrix. Compared against (i) Endogenous Fitness and (ii) ECI (Dataviva). Predictability analyzed in the Fitness–Income plane via a **"measure of direction"** (average cosine of state trajectory vectors in log F – log GDPpc), adapting the Selective Predictability Scheme of Cristelli et al. (2015) to the small-N (27 states) regime where the original concentration/grid method fails.

**Key findings.**
- **Endogenous Fitness on states collapses**: because the state×product matrix has a large empty region (Msp=0 > Msp=1), all Fitness values but one tend to zero — the *ranking* is well-defined but the *values* are degenerate. Exogenous Fitness restores **stable, comparable quantitative values** while preserving the ranking (Spearman ρ_ExEn ≈ **0.97** between the two).
- **ECI is essentially uncorrelated with (Exogenous) Fitness** (ρ_ExECI ≈ **−0.14**) and produces qualitatively implausible rankings (rich high-HDI states like Santa Catarina/Paraná ranked near the bottom; poor Alagoas ranked 4th) → the authors argue Fitness is the more reliable subnational metric.
- The Fitness–Income plane splits into a **high-predictability ("laminar")** and a **low-predictability ("chaotic")** region, mirroring the world-country heterogeneous-dynamics result. Diversified, complex-product states (São Paulo) sit in the predictable, growing regime; resource/simple-product states are chaotic. BRIC decomposition (Table 1): Brazil's Fitness fall 2003–2013 is driven by **loss of export-basket breadth (−43%)**, not by complexity change (−6%); China gains on both margins (+32% basket, +18% complexity).

**Relevance.** Two transferable assets. (1) **The Exogenous-Fitness trick** is the natural answer to the convergence pathology that 1a flagged for firm-scale matrices: when the focal bipartite matrix is too sparse for the endogenous FC algorithm to yield stable *values*, import product Complexities from a larger, denser reference matrix (world trade) and project. For a firm-level study this means scoring firms with **country/world-derived product complexities** rather than re-estimating Q_p on the thin firm×product matrix. (2) The **Fitness-decomposition (ΔF into basket-change vs complexity-change terms)** and the predictability-regime framing give a ready vocabulary for describing how firms move after a trade shock. Co-authored by Pugliese — direct continuity with 1b.

#### Guan, Yan, Hu & Xiong (2020 / firm-complexity) — *Does product complexity matter for firms' total factor productivity?*
*(Chinese firm panel; read in full, 9 pp.)*

**Main contribution.** Tests, at the **firm** level, whether producing **more complex products** raises **total factor productivity (TFP)** — porting the country-level "complexity → growth" result down to the firm and giving it a TFP-mechanism reading (complex production embodies more/better capabilities).

**Data & method.** Chinese manufacturing firms ~2000–2006, **CASIF (Annual Survey of Industrial Firms)** matched to product output via **CCTS** customs/product classification. Product Complexity Index built with the **Hidalgo–Hausmann Method of Reflection (PCI)**; aggregated to a **firm complexity index (fci)** over the firm's product mix. TFP estimated with **Levinsohn–Petrin** (intermediate-input proxy for unobserved productivity). Endogeneity of complexity addressed with **2SLS / lagged instruments**. Controls for human capital, capital intensity, ownership, export status.

**Key findings.**
- Firm product complexity is **positively and significantly associated with TFP**; magnitude on the order of a **~7.5% (of an SD) productivity effect**, robust across OLS, LP, and IV.
- The effect is **mediated by human capital and intermediate-input quality** — complex production pays off where the firm has the skilled labour and input base to absorb it (a capability-complementarity reading).

**Relevance.** Closes the 1c loop from the firm side: where Bontadini works at country-DVA scale and Operti at state scale, Guan shows the **complexity→performance link holds on a microdata firm panel** using the *Method-of-Reflection* PCI (the ECI lineage, contrast with the Fitness lineage of 1a/Operti) and a standard **LP-TFP + IV** productivity design. For Trento it offers a concrete template: assign each firm a complexity score from its product basket, regress LP-estimated TFP on it with lagged-IV, and look for human-capital/input mediation.

**Cross-paper synthesis (sub-batch 1c).** All three say **the qualitative content of the basket beats its size**, but at three different scales and with two different complexity lineages. Methodologically the sub-batch resolves a tension 1a raised — the FC algorithm misbehaves on small/sparse matrices — via **Operti's Exogenous Fitness** (borrow product Complexities from a larger reference matrix), which is exactly the move a firm-level study needs when the firm×product matrix is too thin to estimate Q_p endogenously. The performance regressions complement each other: **Guan** (firm TFP via LP + Method-of-Reflection PCI), **Bontadini** (country DVA performance/resilience via System GMM, KIBS/HTM/LTM/NR), and Operti's **Fitness-decomposition** (basket-margin vs complexity-margin) — together a menu of estimators and a shared message that diversification *into complex, coherent content* is what carries the growth/productivity/resilience signal. Continuity with 1a/1b is tight: Pugliese co-authors Operti; the ECI (Method-of-Reflection) vs Fitness(-Complexity) contrast recurs; and the "what you produce matters" thesis now spans country → state → firm.

---

### Sub-batch 1d — Relatedness for strategic-product targeting & ML interpretability of RCA prediction

#### Bontadini & Meliciani (2025) — *Selective Industrial Policy for the EU Open Strategic Autonomy: the Role of Products' Relatedness*
*European Commission, Single Market Economics Papers, Working Paper 30 (42 pp incl. appendix, read in full).*

**Main contribution.** Operationalises the Hidalgo/Hausmann **relatedness–density / country-product distance** toolkit as a *policy-targeting* instrument: which strategic products (EU-dependent goods, sensitive-ecosystem goods, Net-Zero Industry Act goods, semiconductors) lie closest to each EU country's productive capabilities, and does that distance predict (i) trade-dependence dynamics and (ii) gain/loss of revealed comparative advantage. Introduces the **absolute vs. relative distance** distinction as the conceptual bridge between *absolute* and *comparative* advantage — with directly opposed policy implications (EU-coordination vs. national specialisation).

**Data & method.** BACI-CEPII bilateral trade, HS12 6-digit, 2012–2021; all EU countries + UK. Builds the **Hausmann et al. (2007) product-proximity matrix** Φ_kk' (co-export-with-RCA conditional probability, ubiquity-normalised) → **density relatedness** → **country-product distance** dist_ik = 1 − Relatedness. **Relative distance** = z-score of dist across all products within a country (RelDist = (dist − mean)/sd). Outcomes: a bounded **trade-dependence index** (net-balance of imports vs exports, rescaled to [0,1]) and the **Balassa RCA**. Product complexity via the **Method of Reflection** (Mariani et al. 2015). Econometrics: long-difference OLS of Δlog trade-dependence on initial distance + controls (labour cost, labour productivity, product complexity, **revealed technological advantage RTA** from REGPAT patents via Lybbert-Zolas crosswalk, export-diversification level & change); **linear probability models** for "RCA drop" (Balassa >1.2 → <1) and "RCA jump" (<0.8 → >1); 3-state RCA **transition matrices** by distance terciles.

**Key findings.**
- **Distance predicts loss, not gain.** Low-distance products that start with RCA retain it far more often (sensitive-ecosystem 66% vs 31% high-distance; semiconductors 78% vs 25%); products with no RCA almost never gain one regardless of distance. RCA-**drop** LPMs: distance consistently positive & significant. RCA-**jump** on *absolute* distance: no significant relationship — but on **relative** distance, jumps become consistently positive & significant.
- **Absolute vs. relative split the policy problem.** *Absolute* proximity → reduces EU trade dependence (good for EU-level coordination, concentrating effort in Germany/Italy who are closest to most strategic goods). *Relative* proximity → predicts where a country will actually develop new RCAs (countries veer to their own-easiest specialisation). Ranking reshuffles sharply between the two (Czechia 10th→3rd, Sweden 12th→4th; Spain 3rd→19th).
- For the broad EU-dependent / sensitive-ecosystem categories, **distance loses significance once export diversification is controlled** (distance largely *is* diversification there); it survives for the technologically narrower **NZIA goods and semiconductors**, where capabilities matter beyond breadth. Semiconductors are sharply skewed to high complexity; NZIA goods are closest to EU capabilities.
- **Strong persistence** of distance 2012–21 (mild convergence only via outliers) — read explicitly through the **Schumpeterian/evolutionary path-dependence** lens (Dosi 1982; Dosi et al. 1988; Dosi-Nelson 1994). Policy upshot: target **coherent capability ecosystems**, not isolated products, or new RCAs won't last.

**Relevance.** This is the **policy-facing twin** of the relatedness pipeline the project already has from 1b/1c — same Hausmann proximity, same density-relatedness/distance, here paired with **trade-dependence dynamics and RCA-transition outcomes**, plus the **absolute-vs-relative distance** move (a clean, transferable idea: normalise distance within the unit to separate "who is closest to the product" from "which product is closest to the unit"). The RCA-drop vs RCA-jump asymmetry (distance kills retention; *relative* distance drives acquisition) is a directly usable empirical template, and the path-dependence framing ties Batch 1 to the Dosi capability theory of Batch 4. Same first author as 1c's Bontadini_2021 — continuity.

#### Gnecco, Nutarelli & Riccaboni (2023) — *Matrix completion of world trade: an analysis of interpretability through Shapley values*
*The World Economy 46:2707–2731 (25 pp, read in full).*

**Main contribution.** Brings **interpretable machine learning** to economic complexity: takes the authors' earlier **matrix-completion (MC)** predictor of RCAs (Gnecco et al. 2022) and asks *which countries' export profiles actually drive the prediction of a given country's RCAs* — answered with **Shapley values** from cooperative game theory. Headline conceptual point: the right notion of "comparable country" for a prediction task is **asymmetric** (Shapley) and **task-supervised**, not the symmetric, unsupervised **cosine similarity** the literature defaults to.

**Data & method.** CEPII-BACI, 2018 (plus a 2002/2006 EU-enlargement appendix), HS-1992 4-digit (P=1,243 products), C=14 European countries (computational limit). RCA matrix → incidence/discretised matrix → **soft-impute MC** (nuclear-norm regularised, λ chosen on validation, evaluated on a held-out test set) reconstructs hidden RCA entries → thresholded into a binary RCA≥1 classifier. Each country j is the "null player"; the **characteristic function** v_j(S) = test-set classification accuracy for j using coalition S of other countries; **Shapley values φ_i(v_j)** (Monte-Carlo permutation estimate, Q'=50, 91,000 MC runs per country) rank countries by marginal contribution to predicting j. Compared against **cosine-similarity** rankings via **Kendall-τ**, and validated by re-running MC on the top-r vs bottom-r country subsets.

**Key findings.**
- **Shapley ≠ cosine.** Rankings diverge (low/mixed Kendall-τ across countries); cosine is symmetric (Germany~Poland both ways) but predictive usefulness is *not* — a developing country mimicking a developed one is informative, the reverse less so. Cosine's symmetry is therefore the wrong tool for "who should I learn from."
- **Shapley rankings are predictively better.** Using the top-r Shapley countries beats top-r cosine countries (~74% of cases) and beats bottom-r Shapley (~88%) for MC classification accuracy — i.e. the Shapley-selected "comparable countries" genuinely carry the prediction.
- Country-specific, asymmetric "comparable set" → a natural **recommender system** for export upgrading, especially for developing countries; the appendix shows Shapley rankings track the exogenous 2004 EU-enlargement shock (Germany, Spain shift) better than cosine.

**Relevance.** Two transferable assets, both methodological. (1) A **principled similarity metric**: when the project wants "firms comparable to firm j for predicting its next product," the lesson is to use a **task-supervised, asymmetric** measure (Shapley over a predictive model) rather than off-the-shelf cosine/co-occurrence symmetry — directly relevant to building a firm-level recommender or peer-group. (2) **Matrix completion as an RCA/product-prediction engine** (soft-impute, low-rank, validation-tuned) is an alternative to the Fitness/relatedness predictors of 1a–1c and could be applied to a sparse firm×product matrix (cf. Operti's sparsity problem in 1c) — with Shapley giving interpretability that the EFC algorithms lack. Caveat for our use: Shapley is computationally heavy (capped at 14 countries here); scaling to many firms needs the parallelisation/Kernel-SHAP/clustering routes the paper flags. Riccaboni (IMT Lucca) anchors this to the Italian EFC-ML network.

**Cross-paper synthesis (sub-batch 1d).** Both papers extend the relatedness/complexity machinery from *measurement* toward *decision support*, but on different fronts. **Bontadini-Meliciani** keep the classic Hausmann-proximity engine and turn it outward — to industrial-policy targeting — surfacing the **absolute-vs-relative distance** distinction and the **drop-vs-jump asymmetry** (distance governs whether you *keep* an RCA; relative distance governs whether you *gain* one). **Gnecco et al.** turn inward — to the *interpretability and similarity-metric* layer — arguing that the right "comparable unit" is asymmetric and task-defined (Shapley) rather than symmetric (cosine), and offering matrix completion as a prediction engine robust to sparse matrices. Together they bracket the project's relatedness pipeline: one says *which targets are reachable and durable given a unit's capability core* (and that policy should build coherent ecosystems, echoing 1a–1c's "coherence beats breadth"), the other says *how to pick the comparison set and predict the next move* in an interpretable, sparsity-tolerant way. Both run on BACI-CEPII — the same trade backbone the project's export panel will sit on.

---

### Sub-batch 1e — Two Caldarola reviews/papers: EC × sustainability transition; EC × structural change/labour

#### Caldarola, Mazzilli, Napolitano, Patelli & Sbardella (2024) — *Economic complexity and the sustainability transition: a review of data, methods, and literature*
*Journal of Physics: Complexity 5, 022001 (33 pp, read in full).*

**Main contribution.** A **methods-and-literature review** mapping how the EC toolbox has been applied to environmental sustainability, organised by three questions: (i) does EC relate to environmental outcomes? (ii) are green products/technologies different from non-green? (iii) how to assess a country/region's readiness for the green transition? Its lasting value for the project is the **consolidated, unified statement of EC methods** (data sources, RCA binarisation, complexity algorithms, relatedness) plus a clear catalogue of **known methodological pitfalls**.

**Data & methods canvassed.** Two data families: **patents** (PATSTAT vs REGPAT; green tagging via CPC Y02/Y04S, OECD ENV-TECH, IPC Green Inventory — with a careful appendix on their reclassification fragility) and **trade** (HS; the proliferating green-product lists — OECD 1999, WTO 2009/CLEG/APEC/PEGS — and the unsolved "what is a green product / final-use" problem). Methods unified under a common notation: Balassa **RCA → binary M matrix** (threshold 1; Bruno et al. 2023 refinements noted); **nestedness** (ecology origin); the **Method of Reflections → ECI/PCI** (eigenvector form) vs the **Fitness-Complexity (EFC) algorithm**; the **Green Complexity Index** (Mealy-Teytelboym: sum of green-product complexities) and **Green Technology Fitness**; relatedness via **Hidalgo proximity ϕ** (Eq. 5; explicitly *not* a true conditional probability) vs the **statistically-validated assist matrix B** (Zaccaria, time-lagged, BiCM-filtered) for cross-layer (tech→product) links.

**Key findings / take-aways for us.**
- **EC↔environment evidence is genuinely mixed**: linear-positive, linear-negative, and complexity-EKC (inverted-U) results all appear, driven by sample/method/measure differences. High-income countries show complexity↔lower emissions; emerging economies often the opposite (pollution-haven caveat).
- Crisp statements of two **EFC algorithm caveats the project must heed**: (a) ECI/PCI are *averages*, smoothing out the cumulative-capability signal that Fitness (a *sum*) preserves — Fitness > ECI for capturing diversification; (b) **Fitness and ECI are within-year relative measures** — their magnitudes are *not comparable across years*, so naïve longitudinal regressions are invalid. Fixes: use rankings, **Operti-style exogenous complexity** (project a reference year's product complexity onto each year's RCA — links straight to 1c), or the **Mazzilli "dummy country" scale-invariance trick**.
- Green products are **more complex** and intertwined with non-green production; **relatedness to (often non-green) existing capabilities** is the dominant driver of green diversification — even low-income regions with high green-relatedness can enter complex green tech.
- Repeated gap flagged: EC green work is country/region-level; **firm-level micro-dynamics are under-explored** — an explicit opening for the Trento project.

**Relevance.** This is the project's **single best methods reference for the whole EFC pipeline** — it disambiguates ECI vs EFC, proximity vs validated-assist-matrix relatedness, patent vs trade data, and (critically) tells you how *not* to misuse Fitness/ECI in a panel regression. The cross-time-comparability fixes (exogenous complexity / dummy trick) are directly actionable for any longitudinal firm-complexity regression. Same Fermi-Center author cluster (Sbardella/Patelli/Mazzilli/Napolitano) that recurs across Batch 1.

#### Caldarola, Mazzilli, Patelli & Sbardella (2024) — *Structural Change, Employment, and Inequality in Europe: an Economic Complexity Approach*
*arXiv:2410.07906 (working paper, 35 pp, read in full).*

**Main contribution.** Three genuine methodological innovations bundled into one applied paper, all directly transferable: (1) **first empirical application of the BiWCM** (Bipartite Weighted Configuration Model, Bruno et al. 2023) to build an *Inferred* Comparative Advantage matrix — an entropy-based, maximum-likelihood-valid replacement for biased Balassa RCA; (2) the **Mazzilli "dummy-country" trick** to make Fitness/Complexity comparable across years; (3) a new **Labour-Weighted Fitness (LWF)** measure with a Fabricant-style **within/between structural decomposition** that isolates a clean "structural change" component = labour moving *between* industries toward more complex ones.

**Data & method.** Eurostat **Structural Business Statistics**: industrial *employment* shares (not exports — deliberately, to capture non-tradeable services) at **NACE 4-digit (218 industries)**, 27 EU countries, 2010–2018; matched to ARDECO (employment growth, labour share = compensation/value-added) and ILO (wage-decile ratios). EFC algorithm (Tacchella 2012) on the BiWCM-validated employment matrix → industry Complexity Q and country Fitness. **LWF = Σ θ_i Q_i** (labour-share-weighted Q); ΔLWF decomposed into **within-term** (Σ θ_{t−k} ΔQ, rising sectoral complexity) and **between-term** (Σ Q Δθ, labour reallocation across sectors = the structural-change component). OLS with country + year FE; controls GDPpc, population, R&D/GDP, exports/GDP; robustness via leave-one-out (N=30) and a **Shannon-entropy placebo** (Labour-Weighted Entropy — which fails to predict, confirming complexity carries the signal).

**Key findings.**
- The employment specialisation matrix is **nested but with an "empty" top-left** — high-Fitness countries (DE, FR, IT, UK, ES) have *dropped* the least-complex labour-intensive industries; sample splits into mature vs industrialising (PL, CZ) economies.
- The **between (structural-change) component is the only term that predicts the outcomes** (within-term and ΔLWF are insignificant throughout): structural change → **lower employment growth** (complex industries are less labour-intensive), **lower 9th/1st and 5th/1st wage inequality** (driven by the *bottom* rising — low-paid jobs in dropped low-complexity sectors disappear, lifting the 1st decile), and a **higher labour share** (likely via higher wages in complex industries, not more jobs). Hence a **trade-off: industrial upgrading vs job creation**.
- Honest limitations: preliminary/descriptive (no causal ID yet — shift-share instrument planned), small N, SBS missing-data reconstructed by validated interpolation (appendix).

**Relevance.** This is the **most methodologically transferable paper in Batch 1 for the project's estimation layer.** Three reusable tools: **BiWCM/Inferred Comparative Advantage** (the principled replacement for Balassa RCA binarisation that 1a's Bruno_2023 introduced — here *used*); the **dummy-country scale-fix** (solving the cross-year comparability problem the sustainability review flagged); and the **within/between Fitness decomposition** (a template for separating "the firm's products got more complex" from "the firm reallocated toward complex products"). The labour-weighted reframing also shows EFC need not run on exports — a relevant degree of freedom if the Trento firm panel has employment or product-mix data. Same author cluster; cites the companion sustainability review (1e-i) and the Mazzilli/Bruno methods papers that anchor Batch 1's toolkit.

**Cross-paper synthesis (sub-batch 1e).** The two Caldarola pieces are the **methods backbone** of Batch 1. The *review* (1e-i) is the map: it inventories every EC ingredient (RCA, nestedness, ECI-vs-EFC, proximity-vs-assist-matrix relatedness, patent-vs-trade data) and — most usefully — names the **two failure modes** that will bite any complexity regression (ECI averaging-away cumulativeness; Fitness/ECI within-year-relativity). The *structural-change paper* (1e-ii) is the demonstration: it deploys the **fixes** for those failure modes (BiWCM unbiased specialisation; dummy-country cross-year comparability) and adds a **within/between decomposition** that operationalises "structural change" as a clean, regressable quantity. Together they close the loop opened across 1a–1d: where 1a diagnosed that RCA and the FC algorithm misbehave (sparse/biased), 1c offered Operti's exogenous-fitness patch, and 1e now supplies the *entropy-null-model* (BiWCM) and *scale-invariance* (dummy) machinery — plus the warning to never compare raw Fitness across years. For Trento, 1e is the "how to compute and regress complexity correctly" chapter; substantively it also reinforces the recurring theme — moving toward complex activities reshapes employment and inequality, not just growth.

---

## §1f — Relatedness, prediction & the green economy (Batch 1f)

*Papers read in full 2026-06-03/04: Albora et al. 2023a (Sapling Similarity), Albora et al. 2023b (Product Progression), Mealy & Teytelboym 2022 (green economy), Nomaler & Verspagen 2023 WP (related vs unrelated diversification).*

This sub-batch closes Batch 1. Where §1a–§1e built the **measurement** toolkit (RCA/Fitness misbehaviour on sparse matrices → exogenous fitness → BiWCM/entropy null models → dummy-country scale fix), §1f turns to the **relatedness/prediction** side: how to measure product–product relatedness without bias, how to *validate* relatedness claims out-of-sample, how to apply the apparatus to a policy-relevant product subset (green goods), and a sharp methodological warning that the workhorse "density" metric is mostly *not* relatedness at all.

### Albora, Rossi Mori & Zaccaria (2023a) — "Sapling Similarity"

- **Main contribution.** A new memory-based collaborative-filtering similarity metric — **Sapling Similarity** — that uniquely allows **negative values**, encoding *anti-correlation/dissimilarity* between items, built on decision-tree / Gini-impurity logic. Observing that a country has product A updates the probability it has B either up (positive similarity) or down (negative similarity). Standard metrics (cosine, Pearson, Jaccard, Tanimoto) are bounded ≥0 and structurally cannot represent repulsion. Proposes **SSCF** (Sapling Similarity Collaborative Filtering), a hybrid user-/item-based scheme with a single hyperparameter γ, incorporating network size N.
- **Data & method.** Tested on standard recommender-system benchmarks (including Amazon-Book) and on the bipartite country–product export network. Compared against LightGCN and NMF (model-based baselines).
- **Key findings.** SSCF outperforms classic memory-based similarities and model-based baselines — new state-of-the-art on Amazon-Book. Negative-value capacity matters economically: Zambia and Japan have strongly *anti-correlated* export baskets, a signal cosine-type metrics structurally cannot represent.
- **Relevance.** Direct upgrade to the relatedness machinery used in EFC. The Hidalgo proximity ϕ is bounded ≥0 and is not a true conditional probability (cf. §1b/§1d critique); Sapling's negative similarities allow more faithful capability distance measurement and better ML feature selection for firm-level diversification prediction.

### Albora, Pietronero, Tacchella & Zaccaria (2023b) — "Product Progression"

- **Main contribution.** Reframes relatedness-measure comparison around **falsifiability**: proposes out-of-sample **forecasting of product "activations"** (RCA 0→1) as the common benchmark all relatedness measures should be judged on. Stops the proliferation of mutually-incomparable relatedness definitions by giving them one scoreboard.
- **Data & method.** COMTRADE HS1992 6-digit, 169 countries × 5040 products, 1996–2018. Predicts new activations using **Random Forest and XGBoost** vs the strong **RCA-autocorrelation benchmark**, Product Space, EcoSpace, preferential attachment, network-validation. Critical design: **cross-validation excludes the predicted country** to force learning of genuine product interdependencies. Because activations are rare, evaluation uses **AUC-PR / F1 / mean Precision@k** rather than ROC-AUC (misleadingly high under class imbalance).
- **Key findings.** Random Forest beats all relatedness-based alternatives and the autocorrelation benchmark. Trees exploit **anti-relatedness / negative signals** (consistent with Sapling). Headline methodological lesson: relatedness measures must be judged by predictive performance under imbalance-aware metrics on held-out units.
- **Relevance.** Provides the project a **validation protocol**: any firm-level diversification prediction must be scored out-of-sample (held-out firms/products), evaluated with PR-based metrics, and benchmarked against an RCA-persistence baseline — not assessed by in-sample regression fit alone.

### Mealy & Teytelboym (2022, *Research Policy*) — "Economic complexity and the green economy"

- **Main contribution.** Applies the EC apparatus to the **green transition**. Builds (i) a consensus dataset of 293 green / 57 renewable-energy HS-6 products (pooling WTO/OECD/APEC lists, COMTRADE 1995–2014), and three new measures: (ii) **Green Complexity Index (GCI)** = *sum* of PCI over green products with RCA>1 (contrast ECI = *average* over all — the sum-vs-average distinction resurfaces from §1c/§1e); (iii) **Green Adjacent Possible (GAP)** = density × PCI scatter for not-yet-competitive green products; (iv) **Green Complexity Potential (GCP)** = GAP aggregated to a scalar: mean relatedness to green complex products not yet competitive in.
- **Data & method.** Eigenvector ECI/PCI (Hausmann et al. 2014), Hidalgo proximity ϕ and density. Validation via cross-country OLS regressions on time-averaged data (no country FE feasible — too little within variation; explicitly acknowledged). Robustness: GCI with Tacchella Fitness-based PCI gives nearly identical results, so GCI is robust to the ECI-vs-FC choice.
- **Key findings.** Green/renewable products are above-average in complexity (mean PCI ≈ 0.48–0.49 vs 0 baseline). Controlling for GDP/cap and ECI, GCI predicts more environmental patents, lower CO₂/cap, and stricter environmental policy. GCP (beginning-of-period, 1995–2000) predicts growth in GCI, green-export share and green-product count (2009–2014). Strong GCI–GCP correlation (Pearson r=0.92) ⇒ strong **path dependence** in green-capability accumulation. Green stimulus spending 2008–09 positively predicts green-export gains 2008–2011 (n=19, suggestive).
- **Relevance.** Template for applying EC toolkit to any policy-relevant product subset — the methods are "completely general." The sum-vs-average GCI/ECI contrast, GAP/GCP logic, and the no-within-FE constraint are all directly reusable for the project's firm-level application. The path-dependence result motivates the capability-reconfiguration framing.

### Nomaler & Verspagen (2023 WP, UNU-MERIT) — "Related or Unrelated Diversification: What is Smart Specialization?"

- **Main contribution.** A pointed **deconstruction of the density metric**. Shows that density — sold as a measure of *relatedness* between a country's current basket and candidate products — is overwhelmingly explained by two relatedness-free quantities: **diversity** (how many products the country makes) and **ubiquity** (how many countries make the product). Together they capture **~93% of the variance of density** (R²=0.9266; diversity alone 0.9164, ubiquity adds ~0.01). So most of what "density-based" smart-specialization advice rests on is *not* relatedness.
- **Data & method.** COMTRADE/WITS, HS-2012 4-digit, 155 countries, 2012 vs 2018. Decompose density by OLS into a predicted part (c + δ·diversity + υ·ubiquity ≡ "unrelated variety") and a **residual** ("related variety"). Feed both into **logit regressions predicting gains AND losses of RCA** (gained: RCA 0→1; lost: 1→0), pooled and per-country. Log-odds-ratio "success bonus" decomposed into ubiquity vs residual contributions.
- **Key findings.** (1) Both related and unrelated variety are significant for gains *and* losses, but predictive power is low (pseudo-R² ≈ 0.03–0.07). (2) **Related variety's relative weight rises with country diversity** — smart-specialization relatedness advice mainly applies to *already-diversified* countries; the median country (diversity 205; 89% below 300) diversifies primarily on *unrelated* variety (high-ubiquity products many others make). (3) **Losses matter and are asymmetric**: lost specializations often had *higher* complexity than gained ones — "smart" specialization must also *preserve* existing specializations, not only acquire new ones. (4) Loss probability ≈ 24% vs gain probability ≈ 3.8% (heavy class imbalance, same lesson as 2023b). (5) The critique extends to derived indicators: **ECOI captures ~50% of variance from diversity/ubiquity** — it too embeds unrelated variety.
- **Relevance.** A **caveat-and-correction** the project must internalize: density/relatedness numbers are confounded by diversity and ubiquity; isolate the *residual* relatedness before claiming a capability-relatedness story. The symmetric gain/loss treatment directly maps to firm-level reconfiguration (firms drop products too, often the complex ones), and dovetails with the project's interest in reconfiguration rather than pure expansion.

### Cross-paper synthesis (§1f)

**1. Relatedness needs better metrics, out-of-sample validation, and a confounding audit — in that order.** Sapling fixes the *metric* (admits negative/repulsive links ϕ cannot); Product Progression fixes the *validation* (held-out-country forecasting, PR-metrics, RCA-persistence benchmark); Nomaler-Verspagen fixes the *interpretation* (strip out diversity/ubiquity before claiming relatedness). Together: don't trust an in-sample, ϕ-based, density-driven relatedness story without all three corrections.

**2. Class imbalance is the silent killer.** Both 2023b (rare activations) and Nomaler-Verspagen (gains 3.8% vs losses 24%) flag that naive AUC-ROC overstates performance. Any firm-level diversification prediction in this project must report PR-based metrics (AUC-PR, F1, Precision@k) and balance the sample explicitly.

**3. Losses are first-class, and complexity can go down.** Nomaler-Verspagen's gain/loss asymmetry — lost specializations often had higher complexity than gained ones — is the most project-relevant finding of this sub-batch. Capability *reconfiguration* is not monotone upgrading. Mealy's path-dependence and Nomaler's "preserve, don't only acquire" advice both reframe diversification as a two-sided (entry + exit) process — exactly the firm-level question.

**4. The sum-vs-average and toolkit-transfer themes recur.** Mealy's GCI (sum of PCI over a subset) vs ECI (average over all) reprises the §1c/§1e Fitness-vs-ECI distinction; and the demonstrated portability of the apparatus to "any product subset" licenses the project's plan to apply EFC machinery to firm-level capability sub-domains.

---

**Batch 1 status: COMPLETE** (sub-batches 1a–1f, all 17 papers read in full). The methods backbone — measurement + null models + relatedness/prediction/validation — is now assembled. Next per priority order: **Batch 4** (capability theory & firm dynamics), starting sub-batch **4a** (Penrose 1959, Teece 1982).

---

## §4a — Capability theory & economies of scope: the foundations (Batch 4a)

*Papers read in full 2026-06-04: Penrose (1959) Ch. VII "The Economics of Diversification"; Teece (1982) "Towards an Economic Theory of the Multiproduct Firm."*

Batch 4 opens the capability-theory strand of the literature. Where Batch 1 built the *measurement* toolkit for complexity (ECI, Fitness, BiWCM, relatedness), Batch 4 supplies the *theoretical micro-foundations* for why firms hold capability bundles and why those bundles shape the direction of diversification. Penrose 1959 and Teece 1982 are the canonical pair: Penrose provides the resource/capability ontology; Teece translates it into a transactions-cost theory of why multiproduct organization rather than markets is the efficient governance mode for deploying those capabilities.

### Penrose (1959), Chapter VII — "The Economics of Diversification"

- **Main contribution.** Penrose's core claim — across the whole book, crystallized in Chapter VII — is that **the firm is a pool of productive resources**, and its final products at any moment are merely one of several possible configurations of those resources. This inverts the neoclassical view: instead of the firm being defined by its output and selecting inputs accordingly, the firm's *existing resource base* defines the feasible set of products it can profitably produce. The chapter works out the full theory of diversification that follows from this ontology.
- **Key concepts.**
  - **Areas of specialization**: each firm has a *production/technological base* (complementary machines, processes, skills, materials that are jointly used — a firm may have several) and *market areas* (customer groups reached by a single sales program). Diversification can occur within existing areas, into new markets from the same technological base, into new products for existing markets from a different technology, or — the hardest case — into new markets with a new technology.
  - **Excess productive services**: firms continuously generate unutilized productive services through learning-by-doing, routinization of management, and industrial research. These services are the proximate engine of diversification: the firm finds it profitable to deploy them in new products rather than letting them lie idle or returning resources to shareholders.
  - **Industrial research and the technological base**: R&D, originally a competitive necessity ("firms must keep up with creative destruction"), generates knowledge that often has generalized application beyond existing products. A firm whose technological base is broad and non-product-specific — e.g., "industrial chemistry" or "engineering for mass production" — has wide adjacent opportunities. The GM and General Mills case studies illustrate how capability relatedness, not conglomerate randomness, drives the direction of diversification.
  - **Competition as a constraint**: competition forces continued investment in each field a firm enters; this restricts the number of fields that can be simultaneously supported. The completely non-specialized firm is almost as vulnerable as the completely specialized one under rapid innovation. Result: firms specialize broadly in a few well-defined capability areas rather than infinitely diversifying.
  - **The "pool of resources" conclusion** (p. 150): "The final products being produced by a firm at any given time merely represent one of several ways in which the firm could be using its resources, an incident in the development of its basic potentialities." Firm strength lies in capability depth — "defences in depth" in a small number of special fields — not in the specific current product portfolio.
- **Methodological note.** Penrose's approach is qualitative and case-based (GM, General Mills corporate annual reports); she explicitly rejects count-of-products as a meaningful measure of diversification. This anticipates the EC literature's frustration with product-count diversity measures and supports the project's capability-relatedness framing.
- **Relevance.** The "firm as pool of resources" ontology is the direct theoretical ancestor of the EC literature's concept of productive capabilities. Penrose's *areas of specialization* (production base × market area) map cleanly onto the bipartite firm–product network the project aims to analyze: the structure of that network at a point in time reflects the capability base, and its evolution reflects capability reconfiguration. Her emphasis on losses (firm must *maintain* investment or withdraw) anticipates Nomaler-Verspagen's gain/loss asymmetry (§1f).

### Teece (1982) — "Towards an Economic Theory of the Multiproduct Firm"

- **Main contribution.** Teece argues that neither neoclassical economies of scope (Panzar-Willig), financial diversification (CAPM), nor managerial theories (Marris/Mueller) provide a satisfying account of why multiproduct organization, rather than market contracts, is the efficient structure for deploying shared capabilities. The paper provides that account by combining Penrose's resource logic with transactions cost economics (Williamson) and the Nelson-Winter evolutionary theory of the firm (tacit, routine-based organizational knowledge).
- **Data & method.** Theoretical paper. Historical consistency checked against Chandler's (1969, 1977) evidence on US corporate diversification; no econometric analysis.
- **Key findings.**
  1. **Why scope economies alone are insufficient**: In a zero-transactions-cost world, scope economies can be captured by market contracts that share common inputs across specialized firms — multiproduct organization is economically irrelevant. Multiproduct organization only emerges as the efficient solution when *market failure* makes contractual sharing of shared inputs costly or impossible.
  2. **Organizational knowledge is tacit and fungible**: Drawing on Polanyi (personal tacit knowledge) and Nelson-Winter (organizational memory stored in routines, "organizations remember by doing"), Teece argues that a firm's productive capability lies *upstream* from its end products — it lies in a generalizable capability that can find application in a variety of product configurations. Transfer of this capability across firm boundaries is difficult precisely *because* it is tacit: it requires transfer of individual team members plus organizational context.
  3. **Four classes of scope economies and governance implications**:
     - *Class I* (non-specialized indivisible physical capital): market solutions (leasing) generally superior — no compelling reason for diversification.
     - *Class II* (specialized indivisible physical capital): thin markets → bilateral monopoly → Klein-Crawford-Alchian quasi-rent hold-up → diversification (intrafirm trading) avoids these contracting hazards.
     - *Class III* (human capital / proprietary knowhow as common input): multiproduct organization required because (a) tacit knowledge cannot be fully articulated or disclosed to a buyer without destroying the basis for exchange (Arrow's "fundamental paradox of information"); (b) recurrent idiosyncratic exchanges of proprietary knowhow require "relational contracting" or, for the most idiosyncratic cases, unified (intrafirm) governance; (c) congestion in accessing the common input (over-extended scientists/managers) limits but does not eliminate the scope for diversification.
     - *Class IV* (external economies): Coase theorem fails when transactions costs are significant → common ownership to internalize the externality.
  4. **The make-vs-market decision**: A profit-seeking firm with excess resources confronts three options: (i) sell factor services in markets, (ii) diversify (multiproduct organization), (iii) return cash to shareholders. Option (ii) dominates when market failure makes option (i) costly — i.e., for Class II–IV assets. The theory is thus explicitly a transactions-cost *theory of the boundaries of the firm* applied to product scope.
  5. **Lateral vs. conglomerate diversification**: Strong efficiency rationale for related (lateral) diversification — shared technological and market capabilities reduce market-failure costs. Conglomerate diversification has much weaker efficiency rationale: only shared management capability, which generally has low transactions costs in markets; unless the conglomerate's internal capital market has genuine information advantages over external markets for *related* businesses.
  6. **Historical evidence**: Chandler's evidence shows Depression-era diversification was triggered by excess capacity (slack from demand collapse), not portfolio risk reduction or managerial empire-building — consistent with the excess-resources/market-failure framework.
- **Relevance.** Teece provides the *transactions-cost micro-foundation* for why firms hold and deploy capability bundles internally rather than through markets. This is critical for interpreting the project's firm-level data: when we observe a firm entering a new export product, the theory predicts this occurs when (a) the firm has excess capacity in a related capability base (Penrose), and (b) market mechanisms for deploying that capability are imperfect (Teece). This maps directly onto the EFC apparatus: EFC identifies *which* capabilities a firm possesses (from its export basket); Penrose-Teece explains *why* the firm bundles those capabilities internally and *how* the direction of new entry is governed by the existing bundle.

### Cross-paper synthesis (§4a)

**1. The canonical Penrose-Teece chain.** Penrose establishes the ontology (firm = pool of resources; products = current deployment of that pool; excess services = engine of growth). Teece operationalizes the mechanism (excess services are deployed internally when market transfer is impeded by transactions costs arising from tacit, non-contractible organizational knowledge). Together they form the theoretical backbone for capability-based theories of firm diversification.

**2. The direction of diversification is capability-determined, not product-determined.** Both papers insist that the relevant unit of analysis is the capability or technological base, not the product. This maps directly onto the EFC literature's central claim: what a firm currently exports reveals its capability endowment, and that endowment — not industry classification — determines the direction of future entry. The "pool of resources" metaphor is literally what the firm–product bipartite network represents.

**3. Tacit knowledge as the source of relatedness.** Teece's Class III analysis shows that the *reason* capabilities cluster within firms is that the knowledge underlying them is tacit and team-embodied. This provides a micro-foundation for why EFC relatedness measures (product proximity, density) have predictive power: related products share tacit capabilities that are sticky to the firm; unrelated products require capability acquisition from scratch (high entry cost). It also explains why conglomerate diversification (Class III costs are high for unrelated capabilities) is less common and less persistent than related diversification — exactly as Nomaler-Verspagen (§1f) and Penrose (the GM/General Mills cases) document.

**4. Losses, maintenance investment, and the "full line" constraint.** Penrose's competition section stresses that firms must *continue investing* in each field they enter to remain competitive, and that "pruning and retrenchment" is often needed after excessive acquisition. This is the supply-side counterpart to Nomaler-Verspagen's (§1f) empirical finding that specialization *losses* are as important as gains. For the project: capability reconfiguration is not just about entry into new export products; it is about the joint process of entry and exit, each governed by the firm's current capability base and competitive pressure.

**5. What Teece's theory does NOT provide.** Teece's framework is essentially static (it explains *why* diversification occurs, not *when* or *how fast*). It also does not provide a tractable empirical measure of "transactions cost for capability transfer." The EC toolkit in Batch 1 (Fitness, relatedness, density) can be read as empirical proxies that operationalize the capability-distance concept implicit in Penrose-Teece — but this mapping needs to be made explicit in the project's theoretical framework section.

---

## §4b — Evolutionary economics & technical change (Batch 4b)

*Papers read in full 2026-06-04: Dosi (1988) "Sources, Procedures, and Microeconomic Effects of Innovation"; Dosi (1995) "Learning, Market Selection and the Evolution of Industrial Structures."*

Batch 4b brings the evolutionary economics framework that completes the foundation layer. Where Penrose-Teece (§4a) explained *why* firms hold capability bundles and why those bundles are sticky to internal organization, Dosi 1988–1995 explains *how* the innovation process works at the firm level, why it varies across sectors, and how innovation activity drives observable industrial structures and dynamics.

### Dosi (1988) — "Sources, Procedures, and Microeconomic Effects of Innovation"

- **Main contribution.** A comprehensive survey and theoretical framework for innovation activity in market economies. Dosi argues that innovation is **not** a random, undifferentiated process; instead, it has structured sources (scientific/technical opportunities), characteristic procedures (formal R&D, informal learning, diffusion, adoption), and sector-specific regimes that shape both the rate and direction of innovative effort. The microeconomic effects ripple through cost structures, competitiveness, and ultimately industrial evolution.

- **Key concepts.**
  - **Four modes of technological advance**: (i) formalized, costly processes of search (R&D, reflected in measurable expenditure); (ii) informal diffusion (publications, conferences, labor turnover, tacit watching-and-learning); (iii) learning-by-doing and learning-by-using (endogenous knowledge generation during production); (iv) adoption of innovations developed elsewhere, embodied in capital equipment and intermediate inputs.
  - **Propensity to innovate**: the empirical outcome of both the *capabilities* firms possess and the *incentives* they face. Sectors differ systematically in how much they invest in innovation and what they get back in terms of innovation output.
  - **Sectoral specificity** in innovation modes: some sectors (e.g., chemicals, pharmaceuticals, electronics) rely heavily on formalized R&D; others (e.g., textiles, leather) rely on informal learning and adoption. This reflects the underlying technological regime — the state of scientific knowledge, the nature of opportunities, appropriability conditions (strength of IP protection), cumulative properties of knowledge (whether building on prior knowledge matters), and characteristics of the knowledge base (whether abstract/codified or concrete/tacit).
  - **Directions of technological change** are not purely market-driven: they also reflect the internal state of science, the character of the knowledge base, path dependencies (what you've learned before shapes what you can learn next), and the structure of incentives (which innovations will be profitable given market conditions and cost structures).

- **Empirical patterns and data.**
  - R&D intensity varies dramatically by sector: electric/electronics 12.7% of value added in USA, chemicals 6.5%, petroleum 3.0%, instrumentsVariable across countries (Japan 8.5% in electronics vs USA 12.7%).
  - Four modes are present in all sectors, but their relative importance differs: formal R&D is critical in chemicals and electronics; informal modes dominate in traditional sectors.
  - Innovation output (patents, new products) does not scale linearly with R&D input — some sectors get "more bang per buck" from R&D than others.

- **Relevance.** This paper provides the *toolkit* for understanding why firms have different propensities to innovate (a direct explanation for the "excess capacity" in Penrose): firms in high-opportunity sectors (like microelectronics, which Dosi emphasizes as the transformation technology of the 1980s) accumulate excess productive services much faster because the knowledge base is expanding. The four-modes framework also explains why relatedness in capabilities matters (§4a Teece): capabilities learned via mode (i) R&D are different in their fungibility from mode (iii) learning-by-doing.

### Dosi (1995) — "Learning, Market Selection and the Evolution of Industrial Structures"

- **Main contribution.** Dosi et al. develop an evolutionary model that connects the *micro-level* heterogeneity in firm innovation and growth to *macro-level* regularities in industrial structures. The key insight is that aggregate stability (e.g., Pareto firm-size distributions) can coexist with persistent firm-level asymmetries, high turbulence, and entry/exit, **if** industries are governed by **technological regimes** and **market regimes** that shape learning patterns and competitive selection. Equilibrium models fail; far-from-equilibrium evolution explains the data.

- **Key concepts.**
  - **Technological regimes**: sector-specific characteristics of the knowledge base that determine how firms learn, what capabilities are valuable, and what innovations are feasible. High-opportunity, high-cumulativity regimes (like semiconductors) have very different dynamics than low-opportunity, low-cumulativity regimes (like textiles).
  - **Market regimes**: the competitive rules of the game — how easily can new firms enter, how concentrated is the market, what are the scale economies, how intense is advertising or capital intensity as a barrier to entry.
  - **Sectoral specificities** in industrial dynamics: same-size firm in electronics and textiles will grow differently, face different survival probabilities, invest in different types of innovation. These differences are *not* noise; they reflect underlying regime characteristics.
  - **Persistent firm asymmetries**: firms with higher productivity, profitability, or innovation rates *persist* — they don't converge to the average. This is not inconsistent with stable aggregate size distributions because the *distribution itself* adjusts: some firms stay big, some never escape being small.
  - **Life-cycle patterns at the product level**: when a new product emerges (e.g., antibiotics, integrated circuits), there is an initial phase of entry and product innovation, followed by a shakeout where the number of competitors falls and effort shifts to process innovation. This pattern is *not* an equilibrium; it's a far-from-equilibrium evolutionary pattern.
  - **Puzzle resolution**: how can aggregate size distributions be stable (Pareto) while firm-level dynamics are chaotic (high entry/exit, turbulence)? Answer: the stable distribution emerges from heterogeneous firms subject to stochastic shocks, non-equilibrium selection by markets, and regime-specific learning rates — without requiring equilibrium or randomness across all firms.

- **Empirical patterns.**
  - High turbulence in industry fringes (small firms); relative stability in core (large firms).
  - Negative correlation between firm size and growth rate (violates Gibrat's Law) — but this varies by sector.
  - High rates of entry despite low survival probabilities; many entrants are not more efficient than incumbents.
  - Persistence of profitability differentials: firms do not converge to the same rate of return.
  - Sectoral variety: concentration, capital intensity, R&D intensity, and appropriability conditions all affect industrial structure and dynamics differently in different sectors.

- **Theoretical critique.**
  - *Neutral equilibria* (Simon-Gibrat type): cannot explain persistent firm asymmetries or sectoral variety in dynamics.
  - *Optimal control equilibria* (Lucas, Jovanovic): require too much rationality and information; miss the role of technological heterogeneity and learning.
  - *Equilibrium with selection*: incompatible with the observation of persistent asymmetries and high turbulence; markets don't select away differences fast enough.
  - **Proposed solution**: far-from-equilibrium evolution where heterogeneous firms learn at different rates, face random shocks, and are selected by markets, but the outcome (size distribution, entry rates, survival) is regime-specific, not universal.

- **Relevance.** This paper operationalizes the Penrose-Teece framework at the sectoral level. It explains why the "excess resources" that drive diversification (Penrose) are accumulated at different rates in different sectors (Dosi 1988 technological regimes), and why this translates into observable differences in firm growth rates, entry rates, and industrial concentration. It also provides the theoretical foundation for why related diversification (Teece) is more common than conglomerate diversification: firms in regimes with high cumulativity and rich opportunity sets (like electronics) have abundant related expansion opportunities, while firms in low-cumulativity regimes (like textiles) must either focus or diversify into unrelated fields, which is riskier.

### Cross-paper synthesis (§4b)

**1. The innovation→growth→structure chain.** Dosi 1988 documents that innovation differs by sector in its sources, procedures, and output (propensity to innovate). Dosi 1995 shows how these sectoral differences in innovation translate into observable differences in firm growth, entry/exit, concentration, and size distributions. Penrose-Teece (§4a) provides the micro-foundation: why firms innovate (to deploy excess resources) and why internal organization is the efficient structure for deploying fungible, tacit capabilities.

**2. Technological regimes as operationalization of "production base."** Penrose's concept of the firm's "production base" or "areas of specialization" maps directly onto Dosi's technological regimes: both describe the sector-specific constraints on what a firm can *learn* and *produce*. A firm in a high-cumulativity regime (like semiconductors) has many internal learning opportunities; a firm in a low-cumulativity regime (like textiles) has fewer. This explains the direction of diversification: firms follow the expansion opportunities available within their regime.

**3. Persistent asymmetries and capability stickiness.** Dosi 1995 documents that firm-level asymmetries persist; this is not a failure of market selection but a feature of non-equilibrium learning dynamics. Teece Class III (knowhow as common input) explains *why* they persist: tacit knowledge learned within one firm cannot be costlessly transferred to others, so a firm with better learning (more effective R&D, faster learning-by-doing) maintains an edge.

**4. The sectoral heterogeneity puzzle.** Neither Penrose nor Teece alone explains why firm-level dynamics differ so radically across sectors (electronics vs. textiles). Dosi 1988–1995 provides the answer: **technological regimes**. High-opportunity, high-appropriability regimes have fast innovation rates, rapid accumulation of excess resources, frequent entry, and high turbulence. Low-opportunity, low-appropriability regimes have slower learning, less excess capacity creation, lower entry, and more stable incumbent positions.

**5. What remains unexamined.** The Penrose-Teece-Dosi foundation explains firm-level strategies and industrial structures; it does not yet explain **export market dynamics** or the **capability trade-offs** that arise when firms must allocate effort between defending existing markets and entering new ones. This is where the EC literature (Batch 1) enters: by mapping firm capabilities onto *observable trade patterns*, we can directly test whether capability-based models of diversification hold at the export level.

