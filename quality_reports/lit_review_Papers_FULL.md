# Full-Read Literature Review — `Papers/` folder

**Project:** Firm-Level Export Diversification and Capability Reconfiguration (University of Trento)
**Method:** Each paper read in full from the PDF, then synthesised at finding level (Main contribution / Data & method / Key findings / Relevance to project). No finding is recorded unless the PDF was actually read this session (repo anti-hallucination rule).
**Tracker:** `quality_reports/lit_review_Papers_full_PLAN.md`
**Companion syntheses already on disk:** `destefano2025_synthesis.md`, `teti2024_tariff_synthesis.md`.

---

## §4c — Innovation accumulation, exploration/exploitation, technological learning (Batch 4c)

*Papers read in full 2026-06-04: Patel & Pavitt (1997) "The technological competencies of the world's largest firms"; March (1991) "Exploration and Exploitation in Organizational Learning"; Bell & Pavitt (1993) "Technological Accumulation and Industrial Growth."*

Batch 4c completes the capability-theory foundation layer (§4a Penrose-Teece, §4b Dosi) with three papers that address the empirical anatomy of firm-level technological profiles (Patel-Pavitt), the behavioral logic governing how firms allocate effort between deepening and branching (March), and the meso-level process by which technological capabilities accumulate — or fail to — in the first place (Bell-Pavitt). Together they provide the micro-foundations for interpreting *why* firm capability portfolios are the shape they are, and *how* they change over time.

---

### Patel & Pavitt (1997) — "The technological competencies of the world's largest firms: complex and path-dependent, but not much variety"
*Research Policy 26: 141–156*

- **Main contribution.** The first large-scale empirical characterisation of firm-level technological profiles using patent data. Using USPTO grants for 440+ of the world's largest firms over 1969–90, Patel and Pavitt document three key structural properties of technological competencies: (1) *multi-field breadth* — firms are active in far more technological fields than they produce; (2) *remarkable stability* — over 90% of firms have technological profiles that are statistically unchanged from 1969–74 to 1985–90; (3) *sector-determined differentiation* — firms in the same industry have strongly correlated profiles; firms across industries do not.

- **Data and method.** US Patent and Trademark Office grants 1969–90, consolidated to parent-company level (manual disambiguation). Sample: 440+ firms with ≥50 patents in 1981–90; distributed across 16 principal product groups. The technological characterisation uses two complementary measures: (i) *Patent Share (PS)*: firm's share of own patenting in each of 34 technical fields; (ii) *Revealed Technology Advantage (RTA)*: firm's share within a technical field divided by its aggregate share across all fields — the firm-level analog of RCA. A 2×2 PS/RTA space partitions technological activities into *core* (high PS, high RTA), *background* (high PS, low RTA), *niche* (low PS, high RTA), and *marginal* (low PS, low RTA).

- **Key findings.**
  1. **Multi-technology firms are universal.** Only 4% of large firms are active in 10 or fewer of the 34 technical fields; 44% are active in more than 20. Technological reach systematically exceeds product reach: orders of magnitude more firms are technologically active in instruments, computers, and non-electrical machinery than make those products as their primary business.
  2. **Stability.** Correlating PS and RTA profiles between 1969–74 and 1985–90, >90% of firms have profiles that are statistically similar at the 1% level. This holds across all sectors. Acquisitions and divestments barely move the needle: out of 41 cases examined, only 1 showed a statistically changed profile after M&A.
  3. **Sector-determined differentiation.** A firm is ~5× more likely to find a technologically similar peer *inside* its own sector than outside. Cross-sector profile correlations (in RTAs) are negative and significant in 95% of cases between the three major clusters (chemistry/pharma, electrical/computers, mechanical/transport). Chemical and electrical firms have *negatively correlated* profiles despite both being "high-tech."
  4. **Direction of search is heavily constrained by prior competencies.** Table 7: firms' share of patenting in fast-growing technological sub-classes (the most dynamic 1% of all sub-classes by absolute growth) in 1985–90 is strongly correlated with their total patenting distribution in 1969–84. Cross-field diagonal correlations are ~0.85–0.91; off-diagonals are consistently negative. Firms exploit emerging opportunities almost exclusively within their existing field structure.
  5. **Rate of search has managerial discretion.** OLS regressions (Table 8) for three measures of accumulation rate (patent intensity, change in patent share, share in fast-growing sub-classes) find industry and home-country indicators are jointly significant — but adjusted R² is only 0.20–0.44. Unexplained variance (56–80%) is attributed to firm-specific and managerial factors. Scherer and Huh (1992) find that the presence of graduate scientists/engineers in top management is positively associated with R&D volumes.
  6. **No evidence of competitive variety in technology.** Within sectors, firm technological profiles are converging toward similar structures, not diverging. The same underlying technological fields (e.g., materials, instrumentation, controls) are essential to a wide range of competing product configurations. This implies *technological imperatives*: automobile firms must know mechanics; electronics firms must know semiconductor physics. "You cannot focus too much — the products are too complex."

- **Theoretical implications.** The paper formally rejects the "distinctive core competence" view (Prahalad-Hamel 1990 say firms should focus on 5–6 core competencies) as an empirical artefact: firms *need* background and marginal competencies to evaluate suppliers, integrate knowledge streams, and spot emerging opportunities. This confirms the Penrose-Teece (§4a) argument that capability portfolios are internally structured, firm-specific, and not easily replicated — but adds the dimension that they must be *distributed* (multi-field), not "distinctive" (narrow). The RTA/PS framework is directly ancestral to the EFC methodology: EFC's capability-product bipartite network can be read as the firm-level analog of Patel-Pavitt's RTA matrix, mapping revealed technological advantage across product-space rather than patent-class space.

---

### March (1991) — "Exploration and Exploitation in Organizational Learning"
*Organization Science 2(1): 71–87*

- **Main contribution.** One of the most-cited papers in organizational theory. March formalises the tension between *exploitation* (refinement of existing competences: choice, efficiency, execution) and *exploration* (search for new possibilities: variation, risk-taking, experimentation). The paper's central argument is that adaptive processes are inherently biased toward exploitation because its returns are more certain, more proximate, and more tightly coupled to the learning system — and that this bias is potentially self-destructive in the long run.

- **Method.** Two formal simulation models. **Model 1 (mutual learning):** An organisation has a "code" (shared beliefs, procedures) and *n* = 50 individuals. In each period, individuals learn from the code (at rate p₁) and the code learns from individuals whose beliefs are superior to it (at rate p₂). Reality has 30 binary dimensions (values ±1). **Model 2 (competition for primacy):** Normal performance distributions are compared under bilateral and many-competitor settings. The probability of finishing first among N competitors depends on the ratio of variance to mean in a way that increases the value of variability as N grows.

- **Key findings.**
  1. **Exploitation dominance.** Adaptive systems improve exploitation more rapidly than exploration because: (a) exploitation has faster, more certain feedback; (b) increasing competence at exploitation raises its likelihood of reward, compounding the advantage via positive local feedback and path dependence; (c) social effects amplify the bias (network externalities, learning and imitation inhibit experimentation).
  2. **Slow socialization outperforms rapid socialization.** In Model 1 (closed system), slower individual learning from the code (lower p₁) leads to higher equilibrium knowledge in the organisational code — paradoxically. Rapid socialization forces premature convergence between individual and code beliefs, eliminating the diversity from which the code improves. Highest equilibrium knowledge: code learns rapidly (high p₂) from slowly socialized individuals (low p₁).
  3. **Heterogeneity dominates homogeneity.** A mixed population of fast and slow learners (heterogeneous p₁) consistently achieves higher equilibrium knowledge than a homogeneous population at the same average p₁. Slow learners maintain the diversity that the code needs; fast learners capture the gains once the code improves. The problem: individual incentives favour rapid learning (each individual does better by conforming quickly), so optimal collective diversity may be undersupplied by voluntary learning.
  4. **Moderate turnover sustains exploration.** When p₁ is high (rapid socialisation → fast convergence → exploration collapses), moderate turnover (p₃ ≈ 0.1) saves the code by injecting naive diversity. But note: the gains come from diversity, *not* from superior knowledge of recruits — recruits know less individually. Under turbulence (shifting reality), turnover prevents degeneracy: without turnover, the code and individuals converge to a fixed belief set and then wander as reality drifts; with turnover, a moderate renewal of diversity tracks the moving target.
  5. **Competition for primacy reverses the logic.** When N competitors is large and only first place pays, *variance* in performance dominates *mean*. For large N: any variance increase (even at the cost of mean reduction) is advantageous; organisations that improve reliability (reduce variance) may paradoxically worsen their competitive position in races for primacy. This creates countervailing pressure: competitive ecology forces exploration even when internal adaptive dynamics would eliminate it.
  6. **Folk wisdom.** Returns to fast learning are not all positive. Rapid socialisation benefits the socialized but harms the socializers (who lose the diversity that would improve the collective code). Maintaining "naive and ignorant" entrants may be essential for organisational knowledge improvement. Competitive victory does not go to the "properly educated."

- **Relevance.** March provides the micro-level behavioral theory that complements the macro-level patterns documented by Patel-Pavitt and the evolutionary-structural analysis of Dosi (§4b). For the firm-level export diversification project, March's framework suggests that: (a) firms hit by trade shocks face an exploration/exploitation dilemma — deepen existing export competencies (exploit) or branch into new products (explore); (b) the institutional environment (competitive intensity, speed of feedback from export markets, managerial diversity) governs which equilibrium is reached; (c) in an oligopolistic export market with many competitors, the variance advantage (exploration) may dominate, explaining why some firms diversify aggressively in response to trade shocks rather than doubling down. The exploration trap (too many undeveloped possibilities, no distinctive competence) and exploitation trap (stuck in a suboptimal stable equilibrium) map directly onto the two failure modes the project aims to identify: firms that scatter capabilities without direction vs. firms that fail to adapt at all.

---

### Bell & Pavitt (1993) — "Technological Accumulation and Industrial Growth: Contrasts Between Developed and Developing Countries"
*Industrial and Corporate Change 2(2): 157–210*

- **Main contribution.** A sweeping empirical and conceptual survey that re-frames how we understand technological learning in firms, industries, and countries. Bell and Pavitt's central intervention is to draw a sharp analytical distinction between two distinct stocks of resources — *production capacity* (PC) and *technological capabilities* (TC) — and to show that these stocks accumulate at different rates, through different mechanisms, and require different policies. The paper's primary application is explaining why developing-country industrialisation so often fails to produce dynamic efficiency gains: because investment in PC is not sufficient for accumulating TC, and many policy frameworks confuse the two.

- **Conceptual framework.** Figure 1 (the paper's organizing diagram) distinguishes:
  - **Production capacity**: equipment (capital-embodied technology), operating skills, organisational procedures — resources needed to produce at *given* efficiency levels and techniques.
  - **Technological capabilities (TC)**: knowledge, skills, experience, and institutional structures needed to *generate and manage change* in the technology used.
  - **Technological accumulation** = the process of building TC. This is *not* the same as building production capacity, though they are related.
  - Two types of technical change: lumpy investment in new facilities vs. continuous "trickle" of incremental improvement in existing facilities. Both require TC; neither happens automatically from production alone.

- **Key characteristics of TC accumulation in developed countries.**
  1. **Tacit and specific.** Most TC is non-codifiable and person (or institution) embodied. Firm-specific specificity means: a textile firm cannot easily become a computer firm; a computer firm cannot easily become a textile firm. As industrial technologies have become more complex, these specificities have tightened. Transfer of tacit TC is slow, costly, and person-embodied.
  2. **Multi-modal learning.** Formal R&D is NOT the core mechanism for TC accumulation — it is the tip of the iceberg, relevant mainly for large firms in science-based sectors. More fundamental are: design, production engineering, quality control, project management experience, continuous improvement activities. "Even research-intensive innovations require prototype construction and pilot plants; expenditure on development far outweighs expenditure on research."
  3. **Firm-centrality with inter-firm linkages.** The primary locus of TC accumulation is the firm, particularly in learning from specific experiences in developing and operating production systems. But firms are not isolated: user-producer networks, collaborative R&D, knowledge from advanced customers, and public research institutions all play roles — but only as *complements* to, not substitutes for, intra-firm TC accumulation.
  4. **Cumulativeness.** Learning is path-dependent: firms move along trajectories shaped by prior knowledge. Neither frequent step-jumps into totally new areas nor simultaneous learning across many dimensions are feasible. This generates the observable stability of firm technological profiles (Patel-Pavitt 1997 provides the empirical confirmation).
  5. **The technology import/local accumulation complementarity.** A major analytical contribution: technology imports and local TC accumulation are *complementary*, not substitutes. Japan's post-war experience is the exemplar: massive technology licensing complemented (not replaced) by equally massive domestic R&D and engineering investment. The complementarity takes several forms: importing creates learning opportunities; prior local accumulation improves absorptive capacity for imports; importing creates the knowledge base to improve what was imported.

- **The five-sector taxonomy (Pavitt 1984, extended).** Bell and Pavitt apply Pavitt's (1984) classic taxonomy to characterise heterogeneity in TC accumulation:
  | Category | Core sectors | Sources of TC | Main protection |
  |---|---|---|---|
  | Supplier-dominated | Textiles, agriculture | Suppliers, production learning | Non-technical |
  | Scale-intensive | Steel, autos, durables | Production engineering, design | Know-how, scale |
  | Information-intensive | Finance, retail | Systems engineering, software | Copyright |
  | Science-based | Chemicals, electronics | Corporate R&D, basic research | Patents, secrecy |
  | Specialized supplier | Capital goods, instruments | Design, advanced users | Design know-how |
  Each implies a different locus of TC learning and a different trajectory of diversification.

- **The developing country diagnosis.** Inter-country variation in dynamic efficiency (TFP growth, structural transformation) tracks closely with differences in TC accumulation intensity and structure. East Asian NICs (Korea, Taiwan) succeeded by: (i) building strong *intra-firm* TC (engineering, project management, continuous improvement) alongside production capacity; (ii) making technology imports serve as inputs to TC accumulation (not substitutes for it); (iii) creating complementary institutional infrastructure (education/training) *and* investing in intra-firm human capital creation. Latin America, Africa, India: accumulated production capacity but not the TC necessary to generate ongoing improvement — explaining why TFP growth was low or negative in many industries despite significant investment.

- **Two secular trends making TC accumulation harder for latecomers.**
  1. *Increasing specialization.* The knowledge base for changing technology is increasingly differentiated from the knowledge base for using technology. As the gap widens, "doing" production yields less and less learning about how to *change* technology. Explicit, deliberate investment in TC learning becomes necessary rather than automatic. This trend penalises latecomers who rely on learning-by-doing alone.
  2. *Increasing minimum efficient scale.* As optimal production scales rise, the *frequency* of investment projects (per unit of industrial expansion) falls — and it is at the time of investment projects that opportunities for engineering-type TC accumulation are greatest. Each project invests in project management, design, specification, etc. Fewer projects = fewer learning opportunities.

- **Policy conclusion.** Neither protection (import substitution) nor export orientation alone is sufficient to generate adequate TC accumulation, given: the non-appropriability of returns; the increasing specialization and scale trends; and the complexity of managing the process. Explicit, direct policy focus on TC accumulation — investment in intra-firm engineering capabilities, training, R&D institutions oriented toward absorption rather than frontier innovation — is necessary. The old List-vs-Smith debate misses at least half the story.

---

### Cross-paper synthesis (§4c)

**1. Revealed technology profiles as the empirical fingerprint of capability accumulation.** Patel-Pavitt's RTA matrix operationalizes in data what Penrose (§4a) called the "firm's productive base" and what Bell-Pavitt call "technological capabilities." A firm's US patent distribution across 34 technical fields is a noisy but tractable measure of its accumulated TC. The striking stability of these profiles (>90% of firms unchanged over 21 years) *empirically confirms* the cumulativeness, specificity, and path-dependence theorized by Bell-Pavitt and Dosi (§4b). For the project: the observation that export baskets are also highly persistent over time is not a data peculiarity — it is a direct consequence of these fundamental properties of TC accumulation.

**2. The multi-technology imperative vs. the EFC distinctiveness assumption.** Patel-Pavitt's finding that firms must hold *broad, distributed* technological portfolios (core + background + niche + marginal) creates a tension with EFC approaches that emphasize a firm's "distinctive" capability endowment (inferred from its current export basket). A firm with, say, 10 export products has a capability portfolio far wider than those 10 products imply. The Patel-Pavitt lesson: if we measure TC only through exported products (the EFC approach), we are seeing the "core" and perhaps "niche" quadrants — missing the background competencies that enable supply-chain coordination and the marginal competencies that constitute future entry options. This is a potential limitation of the firm-level EFC inference and warrants explicit discussion in the project.

**3. Exploration/exploitation as the behavioral engine of capability reconfiguration.** March provides the missing *decision-level* micro-foundation. Given a stable capability profile (Patel-Pavitt), what drives the *when* and *direction* of change? March: firms that face competitive pressure (many rivals) have stronger incentives to explore (expand variance) than to exploit (improve mean). Trade shocks alter the competitive landscape — new entrants from cheaper-cost countries erode existing exploitative returns, pushing affected firms toward the exploration end. But March's warning is critical: excessive exploration has costs (no distinctive competence), and the adaptive dynamics tend to *under-supply* exploration relative to the social optimum. Policy instruments that force exploration (e.g., export promotion subsidies for new products, R&D tax credits for TC-building) can correct this bias.

**4. Bell-Pavitt's TC/PC distinction as the project's key theoretical wedge.** The distinction between production capacity and technological capabilities is the theoretically grounded version of what the project is trying to measure. A trade shock may destroy production capacity in a sector (comparative advantage erodes, plants close) without necessarily destroying TC — the engineers, routines, and accumulated know-how may survive and be redirectable. Conversely, accumulating production capacity (via export growth) does not automatically build TC. The project's empirical question — do firms that face trade shocks *reconfigure* their capability portfolio, or do they simply contract? — is precisely a question about TC, not PC. This motivates looking at the *direction* of export diversification post-shock (TC redeployment) rather than just the level (PC destruction).

**5. Locus of TC accumulation: firm vs. system.** All three papers converge on the firm as the primary locus of TC accumulation, but with important qualifications. Patel-Pavitt: home country and industry account for 20–44% of the variance in accumulation rate; the rest is firm-specific. Bell-Pavitt: institutional infrastructure (public R&D, education/training) is a *complement*, not a substitute, for intra-firm TC. March: the organisational code (collective knowledge embedded in routines and procedures) is what persists and what needs to be managed. For the project: identifying the firm-level TC endowment (from export baskets) is appropriate as a first approximation, but the heterogeneity in TC accumulation rates across regions/countries (Bell-Pavitt) implies that country or regional fixed effects will be important in the regression design.

**6. What batch 4c adds to the project's empirical design.**
   - *Measurement*: Use Patel-Pavitt's PS/RTA logic to justify the choice of RCA-based EFC measures (both are revealed-advantage indices normalised to remove size effects).
   - *Persistence*: The extreme stability of firm technological profiles provides the null hypothesis: absent shocks, firm export baskets should be highly persistent. The treatment effect of a trade shock is identified against this baseline.
   - *Direction of diversification*: March's exploration/exploitation framework predicts that high-competitive-intensity contexts will push toward exploration (diversification into new products); Bell-Pavitt predicts that the direction of that diversification will be constrained by prior TC accumulation (path-dependent trajectories).
   - *Heterogeneity in response*: Bell-Pavitt's distinction between firms with strong vs. weak TC endowments predicts heterogeneous responses to the same trade shock: TC-rich firms reconfigure (redeploy capabilities into new products); TC-poor firms contract or exit.

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

---

## §4d — Industrial geography, knowledge districts, and limits to globalization (Batch 4d)

*Papers read in full 2026-06-04.*
*Storper (1992) "The Limits to Globalization: Technology Districts and International Trade," Economic Geography 68(1): 60–93.*
*Allen & Gale (2000) — see MISIDENTIFICATION NOTE below.*

**MISIDENTIFICATION NOTE: Allen_2000.** The batch plan labelled Allen_2000 as "industrial geography / knowledge" alongside Storper_1992. The paper at that path is **Franklin Allen & Douglas Gale (2000) "Financial Contagion,"** *Journal of Political Economy* 108(1): 1–33 — a Diamond-Dybvig-style model of bank runs propagating through interbank deposit networks. It has zero relevance to the firm-level capability/trade-shock project. It belongs with the Battiston/Upper papers (Batch 3d, already flagged as SIDE summer-school residue — DROP). Batch 4 checkbox for Allen_2000 should be read as: **READ, CONFIRMED IRRELEVANT — DROP.** The "Allen_2000" label in the plan was presumably a mistaken carry-over from SIDE network theory summer-school materials.

---

### Storper (1992) — "The Limits to Globalization: Technology Districts and International Trade"
*Economic Geography 68(1): 60–93*

- **Main contribution.** Storper argues that a significant and growing share of international trade cannot be explained by comparative advantage (relative factor costs) or new trade theory (scale economies), and must instead be attributed to *absolute* technological advantages grounded in localized, cumulative learning. The core concept is **product-based technological learning** (PBTL): the capacity of a production system to continuously reinvent, differentiate, and reconfigure products through sustained redeployment of specialized skills. Industries dominated by PBTL tend to agglomerate in distinctive subnational regions — **technology districts** — that function as the basic building blocks of the global economy. Globalization, in this view, is not a homogenizing force but a set of relationships among specialized territorial nodes.

- **Six propositions (the paper's architecture).**
  1. *Export specialization is real and increasing.* At the 5-digit SITC level, trade specialization patterns of advanced economies have diverged since the late 1970s, not converged. Countries hold absolute export advantage in relatively few products, and those specializations are sector-specific and historically durable.
  2. *Trade specialization has three distinct causes.* (a) Factor costs / comparative advantage; (b) economies of scale; (c) PBTL. For large swaths of advanced-country trade — supplier-dominated sectors (Italy: clothing, ceramics, jewellery) and high-technology sectors (US: aircraft, semiconductors, medical equipment) — PBTL is the primary mechanism.
  3. *Technologically dynamic industries avoid vertical integration.* Lock-in to a given technology is fatal in PBTL systems. These industries form networks of specialized firms — neither Coasean hierarchies nor spot markets, but durable relational arrangements with "relation-specific skills" (Asanuma 1989). The network minimizes lock-in while preserving external economies of scope.
  4. *Not all networks are PBTL networks.* Networks also arise from simple market uncertainty. The distinction requires examining the qualitative nature of inter-firm transactions, not just their formal structure.
  5. *Networks and agglomeration are positively related in PBTL industries.* Rapid technological change renders user-producer transactions qualitatively dense: interpreting new evidence and negotiating evolving standards requires face-to-face interaction and shared cognitive frameworks. Agglomeration in PBTL systems reflects "Schumpeterian efficiencies" rather than standard localization economies.
  6. *Technological learning rests on territorial conventions.* Conventions — shared rules, behavioral routines, and expectations — mobilize resources and coordinate interactions in ways that cannot be reduced to a list of discrete institutional inputs (universities, R&D labs, quality of life). They explain why the same formal setup produces different learning outcomes in different places.

- **Empirical evidence (France, Italy, United States, 1985 UNIDO data).**
  - *Export composition (Table 1):* Italy's exports are 42% supplier-dominated and only 9% science-based. US exports are 30% science-based. France is scale-intensive with moderate DIC presence. These positions reflect systematically different PBTL structures, not factor endowments.
  - *Top-50 sector PBTL decomposition (Tables 2–5):* Across the three countries, PBTL sectors are 45% of the count but 63% of export value — confirming the "developmental premium" on technologically dynamic specialization. Italy: 32 of 50 sectors, 82% of value in PBTL. US: 19 sectors but 63% of value, driven by aircraft, computers, instruments, armaments.
  - *Technology district geography (Table 7, US):* 50%+ of US employment in export-specialization industries is in 8 states. California location quotients > 2.0 in electronics, aerospace, instruments, medical equipment. Massachusetts/Connecticut: aircraft (LQ = 7.78), precision instruments (2.81), R&D labs (1.80). Italy: DIC goods overwhelmingly concentrated in Third Italy (Tuscany, Emilia-Romagna); these districts also dominate world trade in intermediate equipment (kilns, textile machinery) that serve their own PBTL final-product sectors.

- **Key theoretical moves.**
  1. **Absolute vs. comparative advantage.** Storper links PBTL to Dosi-Pavitt-Soete's concept of absolute advantages: productivity gaps so large they are insensitive to input-price changes. PBTL-based absolute advantages are not temporary disequilibria but self-renewing outcomes of learning dynamics — a direct conceptual predecessor to ECI-based "non-linearities" in country complexity.
  2. **Network as Penrosian firm.** The PBTL production network is described as "the external equivalent of a Penrosian firm." The network maintains multi-field capability breadth (required for PBTL) while avoiding individual firm lock-in — the same balance Penrose sees as the driver of intra-firm expansion. This is the key theoretical bridge between Batch 4 foundations and the EFC bipartite network models of Batch 1.
  3. **Conventions vs. transaction costs.** In Williamson's TC framework the *product* is constant and the efficient governance structure is solved for. In PBTL, the product is being redefined by the transaction itself: "needs and possibilities are defined simultaneously." This requires conventions (qualitative rules of engagement), not governance optimization. The distinction matters for understanding *why* capability networks are regionally sticky and difficult to relocate.
  4. **Collective lock-in as a mechanism of regional decline.** PBTL networks, like technologies, can become locked in. A system's conventions — which initially enable flexibility — resist radical reorientation when a paradigm shifts. This is the mechanism by which trade shocks can be devastating: if a shock disrupts the conventional fabric, the learning network may fragment even if no single firm fails. An irreversibility that standard firm-level panels will not detect.
  5. **Technology district as an analytical category.** Distinguished from Marshallian industrial districts on three dimensions: (i) dynamic economies of scale (rather than static localization); (ii) relational governance (neither markets nor hierarchies); (iii) PBTL-enabling conventions. Examples: Silicon Valley, Modena/Emilia-Romagna, Hollywood, Paris fashion. The category is more specific than "cluster" and more institutional than "agglomeration."

- **Limitations.**
  - Empirical evidence is country- and product-level (UNIDO 1985), not firm-level. The paper argues but does not demonstrate that specific firms within districts earn quasi-rents relative to firms outside.
  - "Conventions" remain theoretically underdeveloped and difficult to operationalize. Storper acknowledges this.
  - No causal identification. The mechanism (PBTL → agglomeration → quasi-rents) is argued via stylized facts, not estimated via treatment-control comparisons.
  - The prediction that PBTL sectors earn "quasi-rents" is plausible but the empirical decomposition (how much of Italy's trade surplus is PBTL vs. scale-based) relies on rough industry-level classifications, not econometric decomposition.

- **Relevance to the project.** Storper_1992 is one of the direct theoretical ancestors of the EFC/complexity program (Batch 1). Specific connections:
  1. *PBTL ≈ firm-level RCA in products.* The Balassa specialization index is the country-level ancestor of firm-level RCA (EFC) and patent RTA (Patel-Pavitt). EFC extends the logic to product-space relatedness: which capabilities enable transition from one PBTL specialization to another.
  2. *Technology districts ≈ bipartite capability-product networks.* Storper's regional production network — specialized firms co-producing PBTL outputs — is precisely what EFC maps at the firm-product level. The "secrets of industry in the air" (Marshall, cited by Storper) are the relational component that EFC's structural signatures approximate.
  3. *Quasi-rents from learning ≈ economic complexity premium.* Storper's PBTL quasi-rents correspond to the "fitness premium" in Cristelli et al.: products not easily imitated earn supernormal returns. Complexity metrics operationalize the replication difficulty.
  4. *Path dependence and lock-in ≈ hysteresis in export baskets.* Storper's collective lock-in explains why export specializations persist and why trade shocks can have permanent effects: they may dissolve the relational capital of the learning network, not merely damage individual firms. This is the mechanism to test in the capability/trade-shock design.
  5. *Direct methodological inspiration.* Storper's question — "what is the network structure that makes a PBTL system work?" — is what community-detection (Batch 3: BRIM, Blondel, Barber) attempts to answer algorithmically: identifying coherent firm-product capability clusters that may function as empirical proxies for technology districts at the firm level.

---

### Cross-paper note (§4d)

Only Storper_1992 is relevant to Batch 4. It completes the theoretical bridge between the Penrose-Teece-Dosi-Bell-March microeconomic foundations (§4a–4c) and the EFC/complexity empirical program (Batch 1). The key addition is the *geographic* and *relational* dimension of capability accumulation: capabilities reside not in individual firms but in the *network of relational exchanges* between co-located firms. A trade shock therefore does not only harm the targeted firm — it can disrupt the relational fabric of the district, destroying the learning externalities that sustained all firms in the network. Standard firm-level panel regressions will miss this mechanism unless the network structure is explicitly measured. This motivates the bipartite network / community-detection approach central to the research design.

Allen & Gale (2000) — confirmed DROP from this project. See misidentification note above.

---

## §4j — What Determines Productivity? (Batch 4j — solo)

*Paper read in full 2026-06-04: Syverson (2011) "What Determines Productivity?", Journal of Economic Literature 49(2): 326–365.*

This is the field-defining survey of the micro-level productivity literature for the Journal of Economic Literature. It organizes a decade of empirical work (2000–2011) around a single question: why do firms and plants differ so much in how efficiently they convert inputs into output? The answer is "many things, both internal and external." The paper is essential background for any empirical work using firm-level production data — it calibrates expectations about what productivity is, how large and persistent differences are, and which factors have been shown to matter.

---

### The empirical baseline: enormous, persistent productivity dispersion

The survey opens by documenting the magnitude of the phenomenon. Within 4-digit SIC manufacturing industries in the US, the average 90th–10th percentile difference in logged TFP is 0.651. This implies a TFP *ratio* of e^0.651 ≈ **1.92** — the plant at the 90th percentile produces nearly twice as much output with the same measured inputs as the 10th percentile plant. This is the *average* across industries; the standard deviation across 4-digit industries is 0.173, so many industries show much larger spreads. In China and India, Hsieh & Klenow (2009) find average 90–10 TFP ratios exceeding 5:1.

These differences are not transient. AR(1) coefficients on TFP are 0.6–0.8, implying considerable persistence. And the correlation between productivity and survival is one of the most robust findings in the literature — virtually invariant to country, time period, or industry.

---

### What productivity is and how it is measured (Section 2)

**Conceptual definition.** TFP is the output–input ratio net of observable input variation: Yt = At·F(Kt, Lt, Mt), where At is the factor-neutral shifter. TFP is, at heart, a residual — the variation in output unexplained by changes in observable inputs. Explaining it means "putting a face on the residual."

**Measurement issues.** Three recurring problems:
1. *Output measurement:* Most producer microdata contains revenues, not quantities. Revenue-based TFP conflates physical efficiency with price variation due to market power or idiosyncratic demand shocks. This is a fundamental identification issue the literature is only beginning to address.
2. *Input measurement:* Labor quality (wage bill vs. headcount), capital (book value, perpetual inventory, depreciation rates), materials (expenditures vs. quantities). Any unmeasured input variation shows up in TFP.
3. *Aggregating inputs into TFP:* Cost-share weights under perfect competition and CRS give Cobb-Douglas α's from revenue shares. Alternatively, estimate the production function directly — but this raises the simultaneous-equation bias (Marschak-Andrews 1944): more productive firms hire more inputs, making inputs correlated with the TFP error. The Olley-Pakes (1996), Levinsohn-Petrin (2003) approaches attempt to correct for this using intermediate inputs as a proxy.

Despite these concerns, TFP results are typically robust to measurement choices because the underlying variation in microdata is so large.

**Within-industry equilibrium dispersion (model sketch).** Profits for producer i: πi = R(Ai, Li, D) − wLi − f. Higher-productivity producers have larger optimal size, higher profits, and are more likely to survive. With free entry (expected value of productivity draw = sunk cost), the equilibrium productivity distribution is a truncation of the underlying draw distribution. This model: (1) supports non-degenerate productivity dispersion (high-productivity firms are limited in size by concave revenue functions); (2) predicts that aggregate productivity increases as the truncation threshold rises; (3) is the conceptual foundation for the Melitz (2003) trade model.

---

### Internal drivers of productivity (Section 3)

**3.1 Management practices / talent.** Bloom & Van Reenen (2007): surveyed 700+ medium-sized firms in US, UK, France, Germany. Scored 18 management practices in operations, monitoring, targets, and incentives. Higher management scores are significantly correlated with labor productivity, TFP, ROA, Tobin's Q, sales growth, and survival. Interquartile range of management scores → 3.2–7.5% productivity difference (10–23% of TFP's 32% interquartile range). Competition and non-primogeniture succession predict good management. IV estimates (using competition and inheritance law as instruments) remain significant, consistent with a causal effect. Extended to 6,000 firms in 17 countries: developing economies (China, India, Brazil) have large left tails of very poorly managed firms — the key heterogeneity, not uniform low productivity.

Bertrand & Schoar (2003): CEOs tracked across multiple firms show significant fixed effects on ROA; adding manager FE raises R² from 0.72 to 0.77. MBA managers have ~1% higher ROA. More aggressive investment/leverage strategies associated with better management.

**3.2 Input quality (labor and capital).** Labor quality: matched employer-employee datasets (Ilmakunnas et al., Fox & Smeets 2011) show labor quality reduces average 90-10 TFP ratio from 3.74 to 3.36 — only a modest reduction. Substantial productivity variation remains unexplained after controlling for education, experience, and tenure.

Capital quality: Sakellaris & Wilson (2004) estimate capital-embodied technological progress at 8–17% per year from investment vintage data. Van Biesebroeck (2003): lean manufacturing adoption (capital + complementary practices) drove labor productivity growth in auto assembly.

Intangible capital: reputation, know-how, loyal customer base — difficult to measure, likely important, still largely an open question.

**3.3 IT and R&D.** IT: Jorgenson, Ho & Stiroh document IT as driver of US productivity resurgence mid-1990s after 20 years of sluggish growth. van Ark, O'Mahony & Timmer show EU's slower growth explained largely by later and smaller IT investment. Bloom, Sadun & Van Reenen: US multinationals in Europe are more productive due to IT + HR practices complementarity.

R&D: Doraszelski & Jaumandreu (2009): R&D spending explains substantial productivity growth in Spanish firms, but roughly doubles the uncertainty in productivity evolution — R&D is risky. Aw, Roberts & Xu (2008): Taiwanese electronics exporters combine self-selection (already more productive before exporting) with an R&D blitz at export entry, driving further productivity growth. The export-R&D interaction reflects the ability to spread innovation gains over a larger market.

**3.4 Learning-by-doing.** Benkard (2000): L-1011 aircraft assembly — 40% knowledge depreciation per year; new model variant required relearning despite prior experience. Thornton & Thompson (2001): Liberty ships across multiple yards — own-design, own-yard experience dominates; cross-yard spillovers = 5–10% of own-yard effect. Levitt, List & Syverson (2011): cross-model learning within an auto plant is limited; but shift-to-shift learning transfers almost perfectly.

Kellogg (2009): oil drilling — accumulated joint producer–driller experience raises productivity beyond each firm's individual experience. Relationship-specific capital: lost if the firms split, creating incentives for relationship stability. This is the firm-level analog of Storper's (§4d) relational conventions.

**3.5 Product innovation.** Product innovation raises revenue productivity (quality-adjusted output per input) via higher prices. Bernard, Redding & Schott (2010): firm TFP is *positively* correlated with number of products produced, both cross-sectionally and within firms over time. Whether innovation drives both TFP and product scope, or whether TFP shocks lead firms to "strike while the iron is hot" and expand product variety, remains open. This is directly relevant to the export diversification question.

**3.6 Firm structure.** Vertical integration: Hortaçsu & Syverson (2011): vertically integrated plants are more productive, but mostly selection (high-productivity plants choose vertical structures). Surprisingly, upstream plants in vertical firms ship very little to downstream plants internally — only 1/3 ship anything internally. Integration facilitates *intangible* input transfers (managerial oversight, know-how) rather than goods flows. This validates the Penrose/Teece argument that capabilities (not goods) are the productive input.

Diversification: Maksimovic & Phillips (2002): conglomerate segments are not less productive — they have lower productivity relative to specialized segments because *specialized firms* select into industries where they have exceptional draws. Conglomerates are firms with good draws in multiple industries (but not exceptional in any). The diversification discount reflects selection, not value destruction. Schoar (2002): conglomerate plants have *higher* permanent productivity; the observed discount reflects temporary adjustment costs — managers over-concentrate on integrating new plants ("new toy" effect), causing existing plant productivity to fall while acquired plants improve.

---

### External drivers of productivity (Section 4)

**4.1 Spillovers.** Moretti (2004): local human capital (share of college-educated workers in metro area other industries) has a positive marginal product on plant productivity; spillovers are stronger among geographically and technologically nearby plants.

Bloom, Schankerman & Van Reenen (2007): R&D generates technological spillovers (positive) and market-stealing effects (negative). The two are separable using technological distance (patent co-occurrence) vs. product-market distance (sales correlations). Technological spillovers dominate — net positive externality.

Bartelsman, Haskel & Martin (2008): convergence toward domestic productivity frontier is faster than toward the global frontier. If a plant falls far behind the global frontier, domestic convergence may still pull it up — but convergence to a frontier too far away disappears entirely.

**4.2 Competition — intramarket.** Syverson (2004a): ready-mixed concrete — denser markets (more competition) have higher productivity lower bounds, higher averages, and less dispersion. This is the clearest evidence of Darwinian selection via competition shifting the productivity distribution upward.

Schmitz (2005): US iron ore — when Brazilian competition arrived ~1980, labor productivity doubled (from 2 to 4 tons/worker-hour) by 1985 through work-rule flexibility. Pure within-firm improvement from competitive pressure; entry and selection were not the primary mechanism here.

**4.3 Competition — trade.** Pavcnik (2002): Chilean trade liberalization 1979–86 → faster productivity growth in import-competing sectors via BOTH within-firm efficiency gains AND reallocation/selection (exit of less efficient firms). The two mechanisms are empirically separable.

Bloom, Draca & Van Reenen (2011): Chinese WTO accession → EU import competition via differential product-level tariff reductions. Low-tech European firms shrank and exited (selection). Other firms innovated — patent rates, R&D, IT adoption, and TFP growth all increased. Net: Chinese competition raised aggregate TFP in Europe through both channels.

**Key result: export productivity premium is mostly self-selection.** Despite the strong positive correlation between exporting and productivity, most studies find that exporters were already more productive *before* they began exporting. Exporting per se does not cause productivity growth in most settings. The pre-entry productivity advantage selects who can pay the sunk cost of export market entry (Melitz mechanism). Exceptions: Van Biesebroeck (2005) for sub-Saharan Africa (credit/contract constraint relaxation); De Loecker (2007) for Slovenia (with greater learning from exports to higher-income regions).

**4.4 Deregulation.** Bridgman, Qi & Schmitz (2009): US Sugar Act 1934–74 distorted incentives → yields fell from 310 to 240 lbs/ton; rebounded immediately after repeal. Regulation can destroy productivity through perverse incentives over multi-decade horizons.

**4.5 Flexible input markets.** Maksimovic & Phillips (2001): the market for manufacturing plants operates efficiently — plants sold come from sellers' *weaker* business lines; productivity rises after sale. The market reallocates assets toward more capable managers.

Hsieh & Klenow (2009): if revenue TFP were equated across plants (allocative efficiency), Chinese TFP would rise 30–50%, Indian TFP 40–60%. The existing dispersion reflects distortions preventing inputs from flowing toward high-productivity producers. This is the microeconomic foundation of the misallocation literature.

---

### Open questions (Section 5)

1. **Role of demand in "productivity":** Revenue TFP mixes supply efficiency with demand factors (market power, idiosyncratic demand shocks). High "productivity" may partly reflect favorable demand conditions. The supply-demand decomposition is a frontier research area.
2. **Relative quantitative importance of drivers:** Which factor has the highest R²? Does it vary by industry? No synthesis yet.
3. **Within vs. between firm contribution to aggregate productivity growth:** What sectoral features determine whether reallocation or within-firm improvement dominates?
4. **Misallocation in developing countries:** What specific distortions create the gaps? Hard to design policy without knowing.
5. **Rising variance in outcomes:** IT may be increasing the spread of productivity outcomes. This creates option value (exit truncates downside); employment protection legislation reduces this option value.
6. **Intangible capital:** Management know-how, organizational routines, reputation — major source of productivity persistence, very hard to measure.
7. **Management vs. managers:** Are good practices causal, or do they reflect the skills of the people implementing them?

---

### Cross-paper synthesis (§4j): Syverson in the context of Batch 4

Syverson's survey closes the loop on everything Batch 4 has built from Penrose (§4a) through Bottazzi-Secchi (§4e), Coad (§4f), Grazzi (§4g), and the diversification literature (§4h–4i). Key synthesis points:

**1. The residual nature of productivity validates the capability-based framework.** TFP is residual output variation after accounting for observable inputs. This is precisely the space in which Penrose's "productive services," Teece's "organizational capabilities," and Dosi's "technological competencies" live. What the Batch 4 capability-theory papers describe qualitatively — firms' internal know-how, routines, and learning — shows up empirically as the TFP residual. The productivity literature's inability to explain more than a fraction of TFP variance with observable factors is evidence that capabilities matter and are hard to measure.

**2. Selection, not learning, dominates the export-productivity link.** The most important empirical message for the project: the export premium in productivity reflects selection (high-productivity firms self-select into exporting) more than learning-by-exporting (which would causally raise productivity after entry). Coad's survey (§4f) established the same point about firm growth more broadly. Together: observational correlations between exporting, diversification, and firm productivity must be interpreted carefully — they reflect the sorting of capable firms into more demanding markets, not the markets building capabilities.

**3. Trade shocks work through both channels.** Pavcnik and Bloom-Draca-Van Reenen confirm that trade competition shocks affect aggregate productivity through BOTH within-firm improvement (competition sharpens incentives) AND selection (less productive firms exit). Any study of trade-shock effects on firm capabilities must therefore measure BOTH the intensive margin (productivity of surviving firms) and the extensive margin (selection/exit). Grazzi's (§4g) finding that exporters are more productive but not more profitable is consistent with this framework: competitive pressure from export markets may constrain margins even as it raises efficiency.

**4. The diversification discount is a capability-matching problem, not a productivity problem.** Maksimovic-Phillips (2002) and Schoar (2002) — cited by Syverson — show that conglomerate firms' plants have higher permanent productivity, and the discount reflects selection and adjustment costs. This is exactly the Matsusaka (§4h) capability-matching theory. The implication: observed correlations between export-basket diversification and productivity require careful decomposition between capability-quality effects and portfolio-composition effects.

**5. Vertical integration transfers intangible inputs (capabilities), not goods.** The Hortaçsu-Syverson finding that vertically integrated firms' upstream plants ship very little to downstream plants — integration is about managing intangible inputs, not goods flows — directly confirms Teece (1982) (§4a): the rationale for the multiproduct firm is the transfer of firm-specific capabilities across activities, not physical goods transactions. This validates using capability portfolios (not product flows) as the unit of analysis in the research design.

**6. For empirical design.** The Syverson survey's message to any researcher using firm-level production data:
- TFP dispersion is huge (90-10 ratio ≈ 2:1 in manufacturing). Firm-level regressions must control for productivity; failure to do so conflates capability quality with input-use patterns.
- Revenue-based TFP mixes efficiency with demand factors. If the research design involves firms with heterogeneous product quality (which EFC-type capability portfolios imply), revenue TFP may not be the right productivity measure.
- Self-selection is the dominant explanation for the export-productivity correlation. Causal identification of trade-shock effects on capabilities requires quasi-experimental variation (tariff changes, trade agreements) combined with pre-shock productivity controls.
- Both within-firm and selection mechanisms are operative in trade shocks. The research design must test both margins.

---

## §4i — Corporate coherence, relatedness, and within-country diversification (Batch 4i)

*Papers read in full 2026-06-04.*
*Delios, Xu & Beamish (2008) "Within-country product diversification and foreign subsidiary performance," Journal of International Business Studies 39: 706–724.*
*Piscitello (2000) "Relatedness and Coherence in Technological and Product Diversification of the World's Largest Firms," Structural Change and Economic Dynamics 11: 295–315.*
*Valvano & Vannoni (2003) "Diversification Strategies and Corporate Coherence: Evidence from Italian Leading Firms," Review of Industrial Organization 23: 25–41.*

These three papers operationalize the concept of *corporate coherence* — the degree to which a firm's diversified activities are related rather than random — and extend it in three complementary directions: multi-dimensional relatedness (Piscitello), empirical testing on Italian manufacturing firms (Valvano-Vannoni), and the institutional conditioning of diversification performance (Delios et al.). All three build directly on Teece, Rumelt, Dosi & Winter (1994), which introduced the survivor-principle method for measuring relatedness.

---

### The shared methodology: Teece et al. (1994) survivor-principle relatedness

All three papers use or extend the same core measurement approach. Relatedness between sectors i and j is computed as the t-statistic comparing observed joint activity frequency (Jij = number of firms active in both i and j) to the hypergeometric random-diversification baseline:

**tij = (Jij − μij) / σij**

where μij = ni·nj/K is the expected number of joint occurrences under random diversification across K firms. If firms in the real world more often combine i and j than chance predicts, the sectors are related — not because of a priori industry classification, but because of revealed capability complementarity. Firm-level coherence is then a weighted average of the relatedness values between the firm's primary industry and all other industries in which it is active.

This is the same logic as EFC's bipartite network: products co-produced by the same firms are "related" by revealed capability structure. The survivor-principle method is the product-space analog of the Fitness/Complexity algorithm.

---

### Piscitello (2000) — "Relatedness and Coherence in Technological and Product Diversification"
*Structural Change and Economic Dynamics 11: 295–315*

- **Data.** 248 large US, European, and Japanese firms (stratified from Fortune 500), 1977–1995. Product data: sales across 42 sectors; technological data: US patent grants across 56 technological fields (University of Reading patent dataset). Coherence computed at three points: 1977, 1986, 1995.

- **Multi-dimensional relatedness.** The paper's main conceptual contribution is disaggregating what drives RELATij into three dimensions:
  1. *Industry-specific:* vertical integration (VERTij: dummy for sequential stages in production chain, from I-O tables) and market similarity (MKTij: dummy for both sectors serving industrial markets).
  2. *Technology-specific:* R&D flow linkages (TECH-LINKij: dummy for high inter-sectoral R&D flows).
  3. *Firm-specific:* technological competence affinity — COMPETij, computed using the same hypergeometric method applied to the patent matrix: high COMPET means the two technological fields are more often combined by the same firm than chance predicts.

  OLS regression (Table 3, n=324 sector pairs): COMPET, VERT, and MKT are all significant at p<0.01. TECH-LINK is not significant (possibly measurement limitations). Adjusted R²≈0.36. The firm-specific (COMPET) dimension explains variance in product-sector relatedness that is orthogonal to industry and technology characteristics — confirming that what counts as "related" is partly idiosyncratic to individual firms' capability histories.

- **Dynamic coherence analysis.**
  - *Product coherence (WARP = weighted average relatedness in products):* Decreases substantially over 1977–1995: mean WARP falls from 11.12 (1977) to 10.79 (1986) to 5.09 (1995). Firms showing above-average coherence decline from 50% to 35% of the sample. Product diversification patterns became less coherent over this period.
  - *Technological coherence (WART = weighted average relatedness in technologies):* Stable throughout: mean WART ≈ 10–11 across all three periods. Firms above average coherence: 41% → 58% → 55%. Technological diversification remains coherent.
  - *Cross-correlations* (Table 5): Product coherence is path-dependent early (WARPt1–WARPt2: r=0.742) but discontinuous late (WARPt2–WARPt3: r=0.206). Technological coherence is strongly persistent in the recent period (WARTt2–WARTt3: r=0.758). Kolmogorov-Smirnov tests confirm: product coherence distributions are statistically equal across 1977–1986 but not 1986–1995; technological coherence distributions are equal across 1986–1995 but not 1977–1986.

- **Key finding.** Over the last two decades of the 20th century, large firms reduced their product coherence while maintaining their technological coherence. This reflects a strategic transition: firms began managing a broad product portfolio around a narrow but stable technology base. Technological diversification and product diversification are increasingly decoupled. Firms follow coherent technological paths even as they disperse across product markets — because technologies are the underlying capabilities that can be deployed across many products.

---

### Valvano & Vannoni (2003) — "Diversification Strategies and Corporate Coherence: Evidence from Italian Leading Firms"
*Review of Industrial Organization 23: 25–41*

- **Data.** Top-5 firms in each 3-digit Italian manufacturing sector, 1993 and 1996. 337 firms (229 diversified) in 1993; 355 firms (230 diversified) in 1996. Firms disaggregated by sales across industries. The paper is the only application of Teece et al.'s methodology to Italian manufacturing.

- **Relatedness determinants (Table III).** Regression of tij on vertical integration dummies (FVI, BVI), and sector similarity measures (SIMADV, SIMR&D, SIMADVR&D, plus ADV and R&D levels). Results, 1993 and 1996:
  - Vertical integration (FVI, BVI): positive and significant (p<0.01) in both years — firms combine upstream-downstream adjacent sectors.
  - Similar advertising intensity (SIMADV): positive (p<0.05) — consumer-facing sectors with similar branding requirements cluster together.
  - Similar R&D intensity (SIMR&D): positive (p<0.01) — science-based sectors cluster together.
  - Combined high advertising + high R&D (SIMADVR&D): positive (p<0.05 to p<0.10).
  - R&D level alone: negative (p<0.01) — a high-R&D sector paired with a traditional sector is among the least related pairs.
  - Adj. R² ≈ 0.14–0.15; F-statistics: 102.7 and 110.7.

- **Coherence levels and performance link (Table IV).** Average COHMAX: 5.38 (1993), 5.57 (1996). Three key pattern findings:
  1. Firms entering the top-5 leaders in 1996 (entrants) are *more* coherent than the 1996 average (COHMAX = 5.88 vs. 5.57).
  2. Firms exiting from top-5 in 1993–1996 are *less* coherent than the 1993 average (COHMAX = 5.05 vs. 5.38).
  3. This is direct evidence that coherent diversification is a competitive advantage: more coherent firms are more likely to gain or retain market leadership; less coherent firms are more likely to be outperformed.

- **Determinants of coherence (Tables V–VI).** OLS of COHMAX on firm characteristics:
  - Size: positive (p<0.01) — larger firms are more coherent, consistent with the idea that they can better exploit capabilities across related sectors.
  - Diversification: negative (p<0.05 in 1996) — more diversification → less coherence.
  - State-owned: negative (1993) — state firms less coherent, consistent with non-market selection.
  - DIFR&D (R&D gap between primary and secondary activities): negative (p<0.01) — diversifying into sectors with very different R&D requirements reduces coherence.
  - VERTIN (vertical integration share of sales): positive (p<0.05 or p<0.01) — deepening vertical integration increases coherence.

- **Coherence change (Table VII).** Regression of ΔCOHMAX93→96 on 1993 levels and changes:
  - Mean reversion: high initial coherence → coherence decreases.
  - SENSITIVE (sectors more affected by EU single market, with greater competitive exposure): positive and significant (p<0.10) for the full sample; higher and more significant for lowly coherent firms. The tightening of competition through European integration pushed firms (especially less coherent ones) to refocus their diversification toward related activities.
  - DDIVER (increase in diversification): negative (p<0.05) — expanding diversification breadth reduces coherence.
  - DVERTIN (increase in vertical integration): positive (p<0.01) — deepening vertical integration increases coherence.
  - ADV changes: positive (p<0.05) — increasing advertising intensity is associated with coherence gains.
  - DR&D (increase in R&D activities): negative (p<0.01) — entering new R&D-intensive sectors reduces coherence (disruptive exploration).

---

### Delios, Xu & Beamish (2008) — "Within-country product diversification and foreign subsidiary performance"
*Journal of International Business Studies 39: 706–724*

- **Main contribution.** Shifts the unit of analysis from corporate-level diversification to *within-country* product diversity — the entropy of products across all of a multinational's subsidiaries in a single host country. Shows that this measure has a performance effect that is moderated by (i) host-country institutional strength and (ii) corporate-level product diversity.

- **Data.** 12,992 foreign subsidiaries of 1,563 Japanese MNCs, 1988–2001. 54+ host countries with ≥30 subsidiaries each. Dependent variables: subsidiary exit (event history, exponential model, n=78,540 spells, 2,963 exits) and subsidiary sales growth (fixed-effects GLS, n=39,816 obs.).

- **Two hypotheses, both supported:**
  1. *H1 (Institutional moderation, Table 3 Model 4):* The positive effect of within-country diversity on subsidiary performance (lower exit) is greater in institutionally **weak** environments. Coefficient on Institutional Strength × Within-Country Product Diversity: positive and significant (p<0.001) in exit model — meaning higher institutional strength attenuates the survival benefit of diversity. Figure 1 confirms: at high within-country diversity, exit rates diverge sharply between weak-institution and strong-institution countries.
  2. *H2 (Corporate diversity moderation, Table 3 Model 5):* The positive effect of within-country diversity on performance is amplified when corporate-level product diversity is higher. In exit model: Corporate Product Diversity × Within-Country Product Diversity: negative and significant (p<0.01) — confirming lower exit when corporate diversity reinforces within-country diversity. In sales growth model (Table 4 Model 5): positive and significant (p<0.05). Figure 2 shows: high corporate diversity firms grow faster at high within-country diversity; low corporate diversity firms grow slower.

- **Mechanism: institutional voids.** In institutionally weak markets, product diversification fills voids that functional markets (capital markets, labor markets, information markets) would otherwise fill. Within-country diversified subsidiaries can: allocate capital internally (bypassing underdeveloped external finance); share management (bypassing expatriate placement costs); build brand credibility across multiple products (bypassing weak brand signaling institutions); negotiate with host governments from a stronger position.

- **Corporate diversity amplification.** A parent with high corporate product diversity has already developed and proven the organizational routines for managing a diverse portfolio. These routines can be deployed by its subsidiaries at lower marginal cost — a version of the capability-breadth argument from Penrose and Patel-Pavitt.

- **Limitations.** The within-country diversity measure is based on SIC-code counts across subsidiaries, not sales-weighted by product within each subsidiary. Related vs. unrelated within-country diversification is not distinguished. Endogeneity is partially addressed via Heckman and 2SLS checks.

---

### Cross-paper synthesis (§4i)

**1. Corporate coherence as the operative concept for "relatedness."** All three papers converge on the Teece-Rumelt-Dosi-Winter (1994) framework: firms do not diversify randomly; their portfolios reflect underlying capability complementarities. The survivor-principle measure of relatedness operationalizes this without imposing a priori industry classifications. The key insight is that what counts as "related" is determined by what firms actually do together — not by technological taxonomies.

**2. The survivor-principle ≡ the EFC bipartite network logic.** The hypergeometric relatedness measure (Jij vs. μij) is structurally identical to the EFC approach of measuring capability relatedness from firm × product co-occurrence matrices. Both identify related activities by their frequency of joint co-presence in the same firm. The COMPET measure in Piscitello (technological patent co-occurrence) is a direct antecedent to the product-space relatedness concept that EFC formalizes (Batch 2). The difference is that EFC uses revealed comparative advantage (RCA) with additional normalization, and the Tacchella fitness algorithm adds an asymmetric weighting. The conceptual foundations are the same.

**3. Technological coherence > product coherence in large firms.** Piscitello's finding that product coherence is declining while technological coherence is stable is a fundamental structural result. As firms' product portfolios diversify and converge globally (driven by competition and institutional pressures), their capability base — the underlying technologies — becomes the stable organizing principle. This directly explains why EFC-type capability metrics (which operate at the level of what firms can produce, not what they happen to produce) outperform product-space metrics in predicting firm diversification paths: the capability structure is more stable than the product portfolio structure.

**4. Competition → coherence (Valvano-Vannoni).** The SENSITIVE result — firms in EU-exposed industries become more coherent over time as competition increases — has a direct implication for the trade-shock project: trade liberalization shocks should, according to this logic, *increase* coherence among surviving firms by eliminating less coherent diversifiers. But the mechanism also implies that the shocks are permanently damaging for firms whose diversification happened to straddle dissimilar sectors (high DIFR&D) — those are the least coherent and most vulnerable.

**5. Institutional voids and export diversification (Delios et al.).** The finding that diversification is more valuable in institutionally weak environments has an important implication for the Italian context: in regions or time periods where institutional infrastructure (financial markets, contract enforcement, brand signaling) is weak, export diversification may serve functions that go beyond pure capability exploitation. Firms in Southern Italy or in the pre-1992 institutional setting may have diversified for institutional void reasons that the capability-matching framework would misclassify as incoherent. Any empirical analysis of Italian firm export diversification that ignores institutional heterogeneity may confound these two mechanisms.

**6. Vertical integration is coherence-preserving (Valvano-Vannoni).** Deeper vertical integration increases coherence; broader product diversification decreases it. This is precisely the pattern that the Penrose framework predicts: related diversification along the value chain (vertical) exploits existing capabilities; unrelated product diversification requires new capability development and risks incoherence. For export diversification, the analog is: firms that extend into new products along their existing supply chain (upstream raw material processing, downstream assembled goods) should show more coherent capability portfolios than those that diversify into geographically or technologically distant product categories.

---

## §4h — Corporate diversification, matching, and the diversification discount (Batch 4h)

*Papers read in full 2026-06-04.*
*Matsusaka (2001) "Corporate Diversification, Value Maximization, and Organizational Capabilities," Journal of Business 74(3): 409–431.*
*Bernardo & Chowdhry (2002) "Resources, Real Options, and Corporate Strategy," Journal of Financial Economics 63: 211–234.*
*Lang & Stulz (1994) "Tobin's q, Corporate Diversification, and Firm Performance," Journal of Political Economy 102(6): 1248–1280.*

These three papers constitute the core of the corporate finance literature on diversification value. Together they establish the empirical fact (Lang-Stulz), offer the canonical capability-matching theory (Matsusaka), and provide the real-options learning extension (Bernardo-Chowdhry). The sequencing here is non-chronological — Lang-Stulz (1994) is the empirical base; Matsusaka (2001) builds on it theoretically.

---

### Lang & Stulz (1994) — "Tobin's q, Corporate Diversification, and Firm Performance"
*Journal of Political Economy 102(6): 1248–1280 — the canonical diversification discount paper*

- **Main contribution.** The paper establishes the empirical "diversification discount": diversified US firms trade at systematically lower Tobin's q than specialized firms, throughout the late 1970s and all of the 1980s, for all diversification measures and after controlling for industry effects, size, R&D intensity, and access to financial markets.

- **Data.** Compustat Business Information files, 1978–1990. All US firms with >$100M average assets in the file (~1,400–1,450 per year). Tobin's q computed using the Lindenberg-Ross (1981) / Smirlock et al. (1984) algorithm (replacement cost of plant/equipment from acquisition schedules; book value of debt and preferred stock; market value of equity). Three diversification measures: (1) number of reported segments; (2) Herfindahl index from sales; (3) Herfindahl index from assets.

- **Key empirical findings.**

  1. *The diversification discount, unadjusted.* In 1984 (the representative middle year): single-segment firms: mean q = 1.53, median q = 1.01. Firms with 5+ segments: mean q = 0.66, median q = 0.58. The D(2) coefficient from OLS regressions is significant at the 1% level every year. The jump from 1 to 2 segments is where most of the discount appears; additional segments contribute small and mostly insignificant further drops. This result holds across all three diversification measures.

  2. *Persistence.* Firms with 5+ segments have mean and median q consistently below 1.0 every year from 1978 to 1990. They never perform even at the sample average. This is "difficult to reconcile with the view that diversification is a valuable intangible asset."

  3. *The chop-shop / industry-adjusted discount.* The canonical test: for each division, take the average q of same-3-digit-SIC single-segment firms as the "pure-play q"; construct the firm's hypothetical q as an asset-weighted average of division pure-play q's. The industry-adjusted discount (pure-play q minus actual q): 0.35 for 2-segment firms, 0.49 for 5-segment firms in 1984, all significant. Industry effects reduce the discount but do not eliminate it. Significant every year (Table 5).

  4. *Robustness.* Holds after controlling for log-assets, R&D/assets, and dividend-paying dummy (proxy for capital market access). Holds for market-to-book as an alternative dependent variable. Holds when excluding outlier q's above 5 (all of which are single-segment firms). Holds for constant-segment subsamples (firms that didn't change segment count in previous 5 years), though weaker.

  5. *Causality — the key question.* Firms that subsequently diversify have below-average segment-adjusted q's before diversifying (mean segment-adjusted q = −0.163, significant at median level). But their industry-adjusted q's are not significantly below average (mean industry-adjusted q = +0.078). Interpretation: **firms in low-q industries diversify seeking growth opportunities** — not bad firms within their industries. Diversification is a response to poor performance in existing industries, not a cause of poor performance. The discount "results at least partly from the low stand-alone q of the divisions of the diversified firms."

  6. *Firms that focus.* Firms with 5+ segments that reduce to 4- do NOT have notably poor accounting performance before refocusing. They show only weak evidence of subsequent performance improvement. The evidence that "diversification causes the discount" vs. "poor performers diversify" is inconclusive — both directions are present.

- **Theoretical interpretation offered.** The paper does not resolve the causality question empirically. It notes that the evidence is consistent with: (a) agency problems causing managers to over-diversify; (b) poor-performing firms diversifying in search of growth (the "defensive diversification" view, Weston-Mansinghka 1971); (c) conglomerates' internal capital markets being efficient (which would predict q > 1, but the data show q < 1 for 5+ segment firms — inconsistent with this view dominating). The paper cannot distinguish these.

---

### Matsusaka (2001) — "Corporate Diversification, Value Maximization, and Organizational Capabilities"
*Journal of Business 74(3): 409–431*

- **Main contribution.** A dynamic neoclassical model in which diversification is a value-maximizing search process driven by organizational capabilities. The model reconciles the seemingly contradictory evidence of (i) a diversification discount and (ii) positive announcement returns to diversification programs.

- **The model.** A firm possesses organizational capabilities T (management skills in marketing, distribution, product development, etc.) that are firm-specific and partially transferable across industries. Revenue in industry i = vi · g(t, x), where vi ∈ [0,1] is the "match quality" — unknown until the firm actually enters the industry. The firm faces three choices each period: specialize in current industry (strategy a), diversify by entering a new industry while maintaining the old (strategy b), or liquidate current business and restart (strategy g).

  *Proposition 1 (optimal strategy thresholds, eq. 2):* A firm follows:
  - Strategy **a** (specialize) when match quality v ≥ v₁ — existing business is good enough
  - Strategy **b** (diversify = search) when v₀ ≤ v < v₁ — existing business isn't great but not worth liquidating; better to search while keeping the old
  - Strategy **g** (liquidate and restart) when v < v₀ — existing business is too bad to maintain while searching

  *Proposition 2 (comparative statics):* Probability of being diversified increases in (i) spread of the match distribution F (higher volatility of potential returns → diversification more attractive as a real option) and (ii) discount rate δ (more patient firms search more before committing).

- **Reconciling the evidence.**
  1. *Diversification discount:* Diversified (b-strategy) firms trade at lower q than specialized (a-strategy) firms for two reasons: they have inferior matches and they bear the static cost of splitting T between businesses. The discount is caused by poor matches — it reflects the reason firms diversify, not the cost of diversification.
  2. *Positive event returns to diversification announcements (1960s):* A diversification announcement signals that the firm is following the b strategy, meaning its current match is not terrible (v ≥ v₀ — the firm chose not to liquidate). This is good news: the market learns that the existing business is profitable enough to justify maintaining it while searching. Only firms with v ≥ v₀ diversify rather than liquidate.
  3. *Mixed event returns in the 1980s:* An a-strategy firm announcing diversification signals that its existing match has deteriorated (it has moved from a to b region). This is bad news.

- **Empirical evidence: evolution of 1960s conglomerates.** 63 conglomerate corporations (Weston-Mansinghka 1971 sample) tracked from 1958 to 1988 vs. matched non-conglomerates. Key finding: **conglomerates deleted their primary industry substantially more than non-conglomerates** (Table 3). Over 10-year periods: ~25–40% of conglomerates deleted primary 2-digit SIC vs. ~10–15% of non-conglomerates. Over 30 years: ~30% deleted primary 2-digit. This pattern of exit from original core industries is consistent with matching/search dynamics — firms diversify, test matches, find a better one, and migrate to it.

- **The capability perspective.** Explicitly built on Penrose (1959) and Teece (1982): organizational capabilities are the source of competitive advantage, but their fit with any specific industry is uncertain. Diversification is not empire-building — it is the rational response of a firm with valuable but poorly matched capabilities. The firm should keep old businesses alive (as insurance) while experimenting, rather than liquidating and restarting (which squanders the search opportunity).

- **Policy implication.** "Defensive diversification" (diversifying to avoid decline in core business) can be shareholder-value-maximizing — it preserves the option value of organizational capabilities while searching for a better match. External pressure to refocus prematurely may destroy value if the firm has not yet found a good match.

---

### Bernardo & Chowdhry (2002) — "Resources, Real Options, and Corporate Strategy"
*Journal of Financial Economics 63: 211–234*

- **Main contribution.** A dynamic real-options model in which firms learn about their resources (capabilities) by undertaking investments and observing outcomes. The model predicts a specific life cycle (specialize → experiment → expand or focus) and provides a novel explanation of the diversification discount based on option value rather than agency costs or match quality.

- **The resource decomposition.** Net cash flow from project i = Ri = G + Si, where G = general resources (applicable to all projects) and Si = specific resources (applicable to project i only). Firms don't know the levels of G and Si separately — only their sum Ri. The key insight: to disentangle G from Si, the firm must try a "general project" (a portfolio of projects with negligible specific resources, so the cash flow converges to G by the LLN).

- **Life cycle (Propositions 1-2 in the discrete model).**
  1. Young firms begin with the **specialized project** (the one for which they believe they have specific resources). This is optimal even when the general project could convey more precise information about G, because the firm would only undertake the general project if the option value is positive, which requires the specialized project to be worth pursuing anyway (Lemma 1 proof).
  2. If specialized project result is intermediate (H+L, ambiguous about G vs. S): the firm **experiments with a general project** to disentangle G and S.
  3. After observing general project outcome:
     - If general resources high: **expand into multisegment business** (high G → many opportunities)
     - If general resources low: **scale up specialized business** (G low → leverage S)
  4. After failing the general project, a firm may **intensify investment** in the specialized business — the failure reveals G is low, confirming S is driving performance.

- **Continuous-time extension.** The critical values ZL (threshold below which the firm scales up specialized) and ZH (threshold above which it expands multisegment) both depend on resource uncertainty σ². As σ² decreases over time (the firm learns), the continuation region [ZL, ZH] shrinks — the firm must commit to either specialization or multisegment expansion. This generates several empirical predictions:

  1. **Young firms > mature firms, same expected resources** — young firms have more real option value (resource uncertainty is higher). This explains the diversification discount: single-segment firms are young-like (uncertain about which way to expand); multisegment firms have already exercised their expansion options.
  2. **Earlier expanders are more valuable** — expanding early (when σ² is still high) requires very high ZH, meaning the firm revealed very high G. Early multisegment expansion is a stronger positive signal than late expansion.
  3. **Earnings persistence (low noise σₑ) → higher value** — more signal per observation about G means faster learning → better investment decisions. Unlike standard real options models where volatility → higher value, here noise in the signal reduces value (it slows learning).
  4. **Asset return volatility decreases with firm age** — as σ² falls deterministically, D = σ²/σₑ falls, and return volatility DVZ/V falls.
  5. **Announcement effects are asymmetric** — value function is convex in Z; positive earnings surprises have larger stock price effects than negative surprises of equal magnitude. Firms more sensitive to earnings news (high VZ) are more likely to expand multisegment.

- **The model's explanation of the diversification discount.** Under this theory, the discount arises because diversified firms have *exercised* their growth options (they've expanded), while single-segment firms retain the unexpercised option to expand. Both types may have the same expected level of G, but the option value differs. This explanation implies no inefficiency: the discount is not evidence of agency problems or capability mismatch — it is the option value of single-segment status.

---

### Cross-paper synthesis (§4h)

**1. Three explanations of the same empirical fact.** Lang-Stulz (1994) documents a robust industry-adjusted diversification discount of 0.35–0.50 in Tobin's q, present every year 1978–1990. Matsusaka (2001) explains it as *capability-match signaling*: diversified firms are in a search phase (poor current matches), not at equilibrium. Bernardo-Chowdhry (2002) explains it as *unexpercised option value*: single-segment firms have more to learn (higher resource uncertainty), which translates into higher option value. These are complementary, not competing: a poorly-matched firm (Matsusaka's b-strategy) is also a firm still learning about its general capabilities (Bernardo-Chowdhry's experimentation phase).

**2. The causality is reversed.** All three papers point to the same conclusion: the discount does NOT reflect that diversification destroys value. Lang-Stulz: poor-performing (low-q) firms diversify in search of growth — the discount precedes diversification. Matsusaka: diversification is the *response* to a poor match, not the cause of the poor match. Bernardo-Chowdhry: single-segment firms are more valuable not because diversification is bad, but because they have unexpercised real options. The policy implication: premature enforcement of corporate focus (disciplining managers to divest) may destroy option value.

**3. Organizational capability as the common theoretical primitive.** All three papers work with the same fundamental concept: firm-specific, transferable capabilities (Penrose's excess resources) that fit some activities better than others. The Matsusaka match quality vi and the Bernardo-Chowdhry general/specific resource decomposition (G+Si) are formalizations of the Penrose/Teece capability concept. The main theoretical contribution of these papers to the research project: they operationalize capability quality as a *match* between capability and activity, not as an absolute level.

**4. Export diversification as the product-space analog.** The corporate diversification setting (firm × industry segments) translates directly to the export diversification setting (firm × export products). The "match quality" vi in Matsusaka's model is the analog of a firm's RCA in product i — how well the firm's capability portfolio fits the specific demands of product i. A firm actively diversifying its export basket (entering new product categories) is following Matsusaka's b-strategy: maintaining existing export lines while experimenting with new ones. The "general resources" G in Bernardo-Chowdhry correspond to firm capabilities that support many export products; "specific resources" Si correspond to product-specific advantages (proprietary technology, established relationships, regulatory certifications). Export diversification is how firms learn whether their capabilities are general (applicable to many products) or specific (tied to a narrow product group).

**5. Trade shocks and capability matching.** A trade shock (import competition, tariff changes) that damages a firm's performance in its existing export products corresponds to reducing the match quality vi for those products. The Matsusaka model predicts: if the shock is severe enough to move vi below v₀ in all existing product lines, the firm liquidates and restarts rather than searching within the current product basket. If the shock is moderate (v₀ ≤ vi < v₁ for some products), the firm should diversify — exit the hardest-hit products while searching for better matches. A trade shock that forces a firm from b-strategy to g-strategy (liquidation) permanently destroys the option value of organizational capabilities. This is the mechanism through which trade shocks can have lasting negative effects on capability portfolios.

**6. The diversification discount in export data.** The Lang-Stulz finding — that firms actively diversifying have lower q BEFORE diversifying — has a direct implication for export-basket research: firms entering new export product categories may appear to perform worse than non-diversifiers in cross-sectional snapshots, not because diversification hurts them, but because they are in a capability-matching phase. Any cross-sectional regression of export-scope breadth on firm performance that ignores this endogeneity will confound the search phase with the matched phase, systematically under-estimating the value of export capability diversification.

---

## §4g — Capabilities ladders and export-performance decoupling (Batch 4g)

*Papers read in full 2026-06-04.*
*Coad, Mathew & Pugliese (2021) "Positioning firms along the capabilities ladder," UNU-MERIT Working Paper 2021-031.*
*Grazzi (2012) "Export and Firm Performance: Evidence on Productivity and Profitability of Italian Companies," Journal of Industrial Competition and Trade 12: 413–444.*

---

### Coad, Mathew & Pugliese (2021) — "Positioning firms along the capabilities ladder"
*UNU-MERIT Working Paper 2021-031*

- **Main contribution.** The paper operationalizes the capability hierarchy — the notion that some firm capabilities are prerequisites for others — using balance-sheet expenditure data from ~40,000 Indian firms (PROWESS, 1988–2015). The methodology applies the Tacchella et al. (2012) fitness/complexity algorithm (originally designed for ECI/country-product matrices) to a firm × capability activity bipartite matrix. This yields simultaneous rankings of firms ("fitness" = position on the capabilities ladder) and activities ("complexity" = how few lower-rung firms can perform it). The result is a data-driven hierarchy of 47 capability dimensions and the firms that possess them.

- **Data.** PROWESS database (CMIE), 39,992 Indian firms, 348,422 firm-year observations, 1988–2015. Balance sheets and profit-and-loss accounts of both listed and unlisted firms. 47 activity variables (binary: does the firm spend anything in this area?) grouped into: (1) Production Capabilities; (2) Technological Adoption; (3) Innovation; (4) Basic Managerial & Organizational; (5) Internationalization; (6) Environment/Welfare; (7) IT & Communication. Merged with PATSTAT for patent data.

- **Methodology.** The Tacchella et al. algorithm iterates coupled non-linear equations until convergence, simultaneously computing firm fitness (Ff) and activity complexity (Qc). A capability is complex if firms lacking fitness are not observed performing it. Nestedness is validated against four progressively tighter null models (homogeneous probability; heterogeneous firm diversification; heterogeneous activity ubiquity; bilateral configuration model preserving both margins). The empirical NODF (Nestedness as Overlap and Decreasing Fill) of 0.710 exceeds all null model predictions — including the bilateral configuration model (mean NODF = 0.593, Z-score = 803) — confirming that nestedness is a genuine structural feature, not an artefact of firm diversification or activity ubiquity.

- **The capability ladder: structure.**
  - *Bottom three rungs:* borrowing (access to credit), land/building assets, outsourced professional employment. These are the minimum organizational prerequisites.
  - *Mid-level rungs:* internationalization activities (import/export of goods, foreign borrowings, overseas investment) and technological absorptive capacity (tech know-how fees, R&D spending, staff training).
  - *Upper rungs:* product development expenditure, patenting, M&A activity, environmental/welfare spending. These are less precisely ordered — nestedness is weaker at the top, meaning firms with adequate mid-level capabilities have more heterogeneous paths to advanced activities.
  - *Dynamic change (2001–2014):* ICT capabilities that were advanced (rare) in the early 2000s became lower-rung fundamentals by 2014 as ICT permeated basic operations. This is the capabilities-ladder analog of general-purpose technology diffusion.

- **Climbing the ladder: firm size and growth outcomes.**
  - *Size-capabilities relationship (Figure 7):* Positive and approximately linear for small firms (below log-sales ≈ 6, ~US$5M). Above this threshold, the relationship flattens — large firms occupy all rungs of the ladder without further size increases. Two distinct regimes: a size-constrained lower regime and a capabilities-determined upper regime.
  - *Growth and capabilities (Figure 8, Table 2):* Higher capability ladder position is associated with higher average sales growth, controlling for size and age. Fixed-effects regression (Eq. 1): capability coefficient = 0.123 (manufacturing), 0.264 (ICT), 0.197 (all firms), all highly significant (p < 0.01). This is the first panel regression result linking a quantified capability score to firm growth across sectors and years in a developing economy.
  - *Survival and capabilities (Figure 9):* Survival probability after 7 years is highest for firms at step I.B (basic productive capabilities without R&D or exporting). Moving to higher rungs (R&D, patenting, exporting) is associated with *lower* survival probability for small firms — consistent with higher risk from advanced activities and higher fixed costs. But for larger firms, survival peaks at step II (internationalization + absorptive capacity) rather than the very top rungs. The explanation: higher rungs involve riskier activities; some "non-survival" is actually lucrative M&A exits.
  - *Profitability and capabilities (Table B.1):* Capabilities do NOT predict profitability — coefficient is -0.0033 (SE = 0.0038), not significant. Growth and survival respond to capabilities; the bottom line does not. This is another instance of the Grazzi (2012) finding (§4g below): performance measures decouple along different dimensions.

- **Pavitt taxonomy decomposition (Figure 6):** Within manufacturing, Science-Based and Specialized Supplier firms (Pavitt's high-tech categories) sit significantly higher on the capabilities ladder than Supplier-Dominated firms. ICT service firms sit at the top. This validates using Pavitt-sector classifications as a rough proxy for capability intensity in sector-level analyses.

- **Policy implications.** Capability-conditional policy support (e.g., export assistance conditional on having a website; R&D grants conditional on patent applications) is suggested as more targeted. But Grazzi et al. (2021) is cited for a caution: some firms may prematurely climb the ladder (e.g., enter export markets before being ready) to become eligible for policy support — misallocation toward ill-prepared firms.

- **Limitations.** (1) Binary capability measure ignores quality heterogeneity (a small firm spending €100 on R&D gets the same score as one spending €100M). (2) Input-based not output-based: inefficient firms may spend on R&D without generating value. (3) Findings are from Indian firms — generalizability to European manufacturing needs verification.

- **Relevance to the project.** This is one of the most directly relevant papers in the batch for the research design:
  1. *Methodology directly applicable:* The Tacchella fitness/complexity algorithm on a firm × capability bipartite matrix is essentially what the EFC programme does for firm × product matrices. This paper bridges EFC network methods to strategic management theory.
  2. *Capabilities ladder ≡ capability hierarchy of export products:* The finding that capabilities are nested (lower rungs are prerequisites for higher rungs) directly maps onto the product-relatedness hierarchy in EFC: firms must master simpler product-capability combinations before accessing complex ones.
  3. *Growth without profitability:* The finding that capabilities predict growth but not profitability reinforces Grazzi (2012): the link between competitive position and profit margins is severed by market competition. Identifying the capability effect on trade outcomes should focus on scope and diversification of the export basket, not firm profit rates.
  4. *Survival as an additional outcome margin:* The U-shaped survival-capability relationship is a direct warning for the trade-shock design: a trade shock that forces firms down the capability ladder may increase exit probability (survival margin) more than it reduces growth rates (growth margin). Both margins must be tested.

---

### Grazzi (2012) — "Export and Firm Performance: Evidence on Productivity and Profitability of Italian Companies"
*Journal of Industrial Competition and Trade 12: 413–444*

- **Main contribution.** Using the Italian manufacturing census (Micro.3, ISTAT) linked to comprehensive trade data (COE), Grazzi documents a robust productivity premium for Italian exporters — consistent with the global literature — but shows that this premium does **not** translate into a comparable profitability premium. Exporting firms are more productive but not systematically more profitable. Growth rates of exporting firms also do not consistently exceed those of non-exporters. This creates a puzzle for theoretical models that treat productivity and profitability as proportional, and for the selection-via-differential-growth mechanism of evolutionary theory.

- **Data.** ISTAT Micro.3 database: Italian manufacturing firms, all sectors NACE 15–37, 1989–2004. Census of firms >100 employees plus rotating sample for firms 20–99 employees plus financial statement data from limited liability firms (from 1998). ~130,000 firms in all sectors; ~60,000 in manufacturing. Covers ~50–60% of Italian manufacturing value added. Linked to COE (complete census of cross-border transactions by Italian firms). Two sub-periods: 1991–1995 (pre-euro) and 2000–2004 (post-euro).

- **Descriptive evidence.**
  - Export participation is high and rising: in most sectors, 60–90% of firms with ≥20 employees export by 2004. In machinery (NACE 29) and chemicals (NACE 24), ~90% export. Export status is highly persistent: P(export in t+1 | export in t) ≈ 0.90, stable across both sub-periods.
  - Sector concentration of exports is very stable over time: NACE 29 (Machinery) accounts for ~20% of total manufacturing exports throughout 1989–2004. Motor vehicles (34) and chemicals (24) together account for another ~20%.

- **Non-parametric tests (Fligner-Policello).** Applied to distributions of size, labor productivity, TFP, ROS (return on sales), and growth rates for exporters vs. non-exporters, across 22 NACE sectors and selected years:
  - *Size and productivity:* Exporters stochastically dominate non-exporters in size and both labor productivity and TFP in almost all sectors and years. Positive and significant FP statistics are the rule, across sectors and sub-periods.
  - *Profitability (ROS):* No consistent pattern. The majority of sector-year cells are not significant. Some sectors show negative FP statistics (non-exporters have *higher* ROS). The export premium in profitability is absent or occasionally reversed.
  - *Growth rates:* Similarly inconclusive. Negative significant statistics appear (non-exporters grow faster in some sectors/years). No systematic export growth premium.

- **Regression analysis (Pooled OLS, Eq. 3).** Controlling for size, patenting activity, and regional dummies, estimated sector-by-sector for both sub-periods:
  - *Labor productivity (Table 6):* Export coefficient is positive and significant in most sectors and both sub-periods, with magnitudes of roughly 0.1–0.4 log points. The euro introduction did not substantially change the coefficients.
  - *TFP (Table 7):* Similar picture — consistent positive export premium in productivity.
  - *Profitability (Table 8):* Only sporadically positive and significant. Many sectors show non-significant or negative export coefficients. The result is robust to stricter definitions of exporter (>20% export intensity threshold, Tables 9–11), and to distinguishing systematic exporters (≥3 years out of 5) from occasional exporters. Systematic exporters are *more productive* than occasional exporters, but no systematic profitability advantage of systematic over occasional is detected.
  - *Patenting:* Positive on productivity in most sectors; rarely significant on profitability; not significant on growth.

- **The puzzle.** Three facts co-exist: (1) productivity and profitability are positively correlated within each group; (2) exporters have a strong productivity premium; (3) exporters have no profitability premium. The missing link is international competition itself: larger/exporting firms face fiercer competition that compresses margins even as their productivity advantage allows them to survive. Smaller, non-exporting firms serve domestic niches sheltered from international competition — their lower productivity is offset by higher price-cost margins in protected market segments.

- **Comparison to theory.** Melitz (2003) and Melitz-Ottaviano (2008) predict that more productive firms earn higher mark-ups; a trade liberalization shock lowers all mark-ups but preserves the ranking. Grazzi's evidence falsifies the ranking-preservation claim: the productivity ranking does not translate into a profitability ranking. The theoretical models assume a direct productivity→profitability link; the data suggest these are partly decoupled, especially once international competitive pressure is factored in.

- **Italy-specific context.** The persistence of a very wide support for the productivity distribution — even after the euro introduction — suggests that Italian manufacturing selection pressure was weaker than Melitz-type models predict. Less productive domestic-oriented firms survived in large numbers throughout the period, serving protected segments. This is consistent with Coad's (2009) finding that selection via differential growth is weak in Italy specifically.

- **Relevance to the project.**
  1. *Export premium in productivity, not profitability:* For the capability/trade-shock research design, the relevant outcome is the composition and scope of the export basket, not firm profits. Profit margins may not move even if capabilities are damaged — the signal will be in export diversification patterns.
  2. *Persistent export status (high sunk costs):* The high persistence of export status (P ≈ 0.90) means trade shocks that force firms to exit export markets are consequential and sticky — hysteresis in export participation is real. This is the mechanism that makes capability damage from trade shocks durable.
  3. *Decoupling of performance dimensions:* The Grazzi finding (exporters = more productive ≠ more profitable ≠ faster growing) is a direct empirical counterpart to Coad (2009)'s theoretical claim. For the project's empirical design: using growth rates or profits as the outcome variable will likely underpower the test. Export scope diversity and capability portfolio breadth are better outcome candidates.
  4. *Italian manufacturing data:* The Micro.3 / COE dataset described here is the direct ancestor of the firm-level Italian manufacturing datasets used in Bottazzi-Secchi (§4e), Grazzi_2012, and the Pugliese et al. / EFC papers (Batch 1). Understanding its structure is important for any future extension of the EFC Italian data work.

---

### Cross-paper synthesis (§4g)

**The common thread: performance dimensions decouple.** Both papers in Batch 4g independently establish the same structural finding — that firm-level competitive advantage, measured along one dimension (capabilities in Coad-Mathew-Pugliese; productivity in Grazzi), does not automatically translate into advantage along other dimensions (profitability and growth). This is not a methodological artifact; it is a structural feature of competitive markets where firms face different competitive pressures depending on their market orientation (domestic vs. export) and capability depth.

**Capabilities predict growth, not profits.** Coad-Mathew-Pugliese show that a higher capabilities-ladder position predicts higher sales growth but not profitability. Grazzi shows that exporting (a proxy for being further up the capability ladder) predicts productivity but not profitability. Together, these papers establish that the capability-to-profitability channel is severed by market competition. The policy and research implication: measuring the effect of trade shocks on firm capabilities should use scope, diversification, and growth outcomes — not profit rates or margins.

**Capabilities as pre-conditions for export.** The Coad-Mathew-Pugliese ladder shows that internationalization activities (export goods, import raw materials, foreign borrowings) sit at the mid-level rungs — above basic production/management capabilities but below patenting and product development. This is directly consistent with the EFC finding (Batch 1) that firms enter export markets sequentially, following capability relatedness. A trade shock that strips away internationalization capability from a mid-rung firm would push it back to lower-rung activities — a backward step on the ladder with long-run capability implications.

**Hysteresis and sunk costs.** Grazzi's finding that export status is highly persistent (P = 0.90 annual transition probability) is the empirical correlate of Melitz's sunk cost of export market entry. Combined with the Coad-Mathew-Pugliese finding that capability positions are themselves sticky, this means: firms do not move freely up and down the ladder in response to shocks. A trade shock severe enough to force exit from the export market is not easily reversed — the firm exits, loses the mid-rung capability signal, and will need to re-pay sunk costs to re-enter. This is the capability-based mechanism for the persistent negative effects of import competition shocks documented in the trade literature (Autor, Dorn, Hanson 2013; Teti 2024 from §destefano_synthesis).

---

## §4f — Firm Growth: A Survey (Batch 4f)

*Paper read in full 2026-06-04: Coad (2009 [working paper 2007]) "Firm Growth: A Survey," Max Planck Institute of Economics, Evolutionary Economics Group, Working Paper #0703.*

This is a 73-page multidisciplinary survey — economics, management, and sociology — covering empirical stylized facts, theoretical frameworks, growth strategies, and size-differentiated dynamics. It synthesizes and frames the Bottazzi-Secchi programme (§4e) and the Penrose-Dosi tradition (§4a–4c) in their broader empirical context, while adding critical new claims about what determinants of growth actually predict.

---

### Empirical regularities (Section 2)

**Size distributions.** Log-normal shape at the aggregate level is a robust first approximation (Gibrat 1931, Hart-Prais 1956). At disaggregated levels the distribution becomes more complex — potentially multimodal (as in pharma, §4e) and sector-specific in its skewness and kurtosis. The smooth aggregate log-normal is a statistical artefact of pooling heterogeneous sectors, not a deep economic regularity.

**Growth rate distributions.** Laplace / tent-shaped density is robust to disaggregation: survives at sector level (Bottazzi-Secchi 2003, §4e), across indicators (sales, employment, value added), and across countries (French, Italian, Danish manufacturing). Laplace is a better summary statistic of the growth distribution than the Gaussian. Fat tails mean extreme growth events (both positive and negative) are more frequent than normality would predict — and contribute disproportionately to the evolution of industries.

Cyclical variation: growth rate variance is **countercyclical** (more dispersed during recessions); kurtosis is **pro-cyclical** (more peaked, less fat-tailed during recessions). The central mass of the distribution shifts more than the tails in response to aggregate shocks.

**Gibrat's Law — four testable dimensions:**

1. *Mean growth independent of size.* Mixed verdict: for large, surviving firms above the minimum efficient scale (MES), β ≈ 1 (Gibrat's Law holds). For small or young firms, β < 1 — mean reversion, i.e. smaller firms grow slightly faster. Caves (1998) and Sutton (1997): best empirical conclusion is "Gibrat's Law holds above a size threshold." Sample selection bias (small firms have higher exit rates) can push β downward; after correction the negative size-growth relationship shrinks.

2. *Variance of growth decreasing with size.* β ≈ -0.20 in US and pharma (Bottazzi-Secchi, §4e). Not universal: absent in Italian manufacturing; weaker in France (β ≈ -0.07). Entirely explained by diversification scope (N ~ S^0.35), not by correlated sub-unit growth.

3. *Autocorrelation of growth rates.* Completely inconclusive literature: some studies find positive, some negative, some none. The key resolution (Bottazzi et al. 2002, Coad 2006b): autocorrelation is **firm-specific and heterogeneous** — averaging masks it. Small firms → negative autocorrelation (erratic, boom-bust); large firms → slight positive autocorrelation (smooth, momentum). The autocorrelation coefficient depends on lagged growth rate: firms with extreme past growth tend to mean-revert sharply, while near-zero-growth firms show no autocorrelation.

4. *Independence from other determinants.* Largely confirmed at the mean — growth is predominantly stochastic. R² values from comprehensive regressions are 2–10% (Table 2 in Coad 2009), occasionally reaching ~30% with very rich controls. The bulk of variance in growth rates is within-firm over time, not between firms at any given moment.

**Other determinants of growth:**

- *Age:* Robust negative effect — younger firms grow faster. Age and size are closely related but age has an independent negative effect on both the mean and variance of growth rates.
- *Innovation:* **The key paradox of the literature.** Innovation is theoretically central and managerially emphasized, but empirical OLS regressions show weak and inconsistent effects on average firm growth. The resolution (Coad-Rao): innovation matters *enormously* for the fast-growth tail, not for the median firm. Quantile regressions at the 90th+ percentile of the growth distribution reveal strong effects of innovativeness; OLS at the mean yields near-zero coefficients. Innovation increases the probability of being a high-growth firm, not the average growth rate.
- *Financial performance (profits):* Not a predictor of growth. Coefficient is often statistically significant but economically negligible. Firm growth and firm profitability are essentially independent processes. Coad (2005): "it may be more useful to consider a firm's profit rate and its subsequent growth rate as entirely independent."
- *Productivity:* Not a predictor of growth either. Baily et al. (1996) find that ~1/3 of productivity growth comes from growing plants, ~1/3 from downsizing plants, ~1/3 from entry/exit. No robust positive relationship between plant-level TFP and growth. This directly undermines the evolutionary "growth of the fitter" principle as applied to differential growth (as opposed to differential exit).

---

### Theoretical assessment (Section 3)

**Neoclassical (optimal size).** Rejected as a description of growth dynamics. Firms do not demonstrably converge to an industry-specific optimal size. Size distributions are too wide, too persistent, and too heterogeneous within sectors to be consistent with optimization toward a common target. Coad's verdict: "better to un-learn [optimal size] quickly."

**Penrose (1959).** Most empirically consistent theoretical framework for growth of large firms. Key mechanism: learning-by-doing releases managerial resources over time → excess capacity of management → pressure to deploy in new growth projects → "economies of growth." Growth is not a means to an optimal size but an end in itself, a constructive application of surplus productive services. Important Penrose effect: above an "optimal growth rate" (Slater 1980), fast growth generates higher operating costs through coordination strain. Related: dynamic capabilities (Teece et al. 1997) as the firm's ability to reconfigure its resource portfolio in fast-changing markets.

**Marris / Managerialism.** Managers attach utility to firm size, not just profits. Growth-maximization subject to a profit constraint → over-diversification relative to shareholders' interests. Largely supported as an explanation for conglomerate diversification (Section 4.2.2). The "conglomerate discount" (diversification destroys shareholder value) provides indirect empirical support: managers diversify beyond the value-maximizing level.

**Evolutionary economics (replicator dynamics / "growth of the fitter").** Key prediction: more profitable or productive firms should grow faster — replicator dynamics should reallocate market share toward "fitter" firms. **Empirically rejected for differential growth.** Neither profitability nor productivity is a robust predictor of growth rates. Selection works via exit of the least fit (survival of the fitter), but not via differential growth among survivors. This is a significant welfare implication: selective reallocation toward more productive firms is much weaker than evolutionary theory predicts.

**Population ecology.** Industry-specific niche carrying capacity explains population dynamics (entry, exit, density dependence). Limited explanatory power at the firm level — individual growth rates vary enormously within the same niche, and niche-level factors add little to the R² of firm-level growth regressions.

---

### Growth strategies (Section 4)

**Is growth intentional?** Both: some firms actively plan growth (Penrose's intentional growth, neoclassical q-theory); many firms experience growth passively as "organizational drift" (Parkinson's Law, Gibrat's stochastic process). Practical conclusion: bounded rationality in growth — not purely random, not perfectly forward-looking.

**Growth by replication.** Requires tacit knowledge transfer — very difficult. Intel's "Copy EXACTLY!" strategy is the extreme case: reproduce every detail of a successful production process, including barometric pressure and hose lengths, because the complexity of semiconductor manufacturing means small deviations cascade into large failures. The general lesson: replication is harder than theory implies because firms don't fully know why their own routines work.

**Growth by diversification.** Related > unrelated (Penrose, Ansoff). Unrelated (conglomerate) diversification destroys value (conglomerate discount, ~1960s wave of acquisitions followed by 1980s "return to corporate specialization"). Related diversification is positive when the new activity leverages existing resources. Corporate refocusing (trimming unrelated activities) is associated with improved performance. The literature's verdict: optimal diversification level is above zero but well below pure conglomerate.

**Growth by acquisition.** Usually destroys value. Managerial motives (empire-building, hubris) dominate shareholder motives in acquisition decisions. Acquiring firms pay 10-30% premium for target, then pay integration costs. "More unsuccessful acquisitions than successful ones" (Harvey-Jones).

---

### Small vs. large firms; stages of growth (Section 5)

- **Small firms:** entry rates high, ~20-40% fail in first two years, only 40-50% survive beyond year 7. Enter at ~40-60% of incumbent MES. Must grow rapidly to close cost gap; growth and survival are intertwined. Growth is erratic (negative autocorrelation, especially for fast-growing small firms). Only a minority of entrants are true innovators; most are "followers" escaping unemployment.
- **Large firms:** growth and survival are decoupled. Growth is smoother (positive autocorrelation). Large firms resemble investment trusts with semi-autonomous divisions. They can grow above MES without reducing survival probability.
- **Stages of growth** (Greiner 1972, Churchill-Lewis 1983, Garnsey 1998): firms pass through sequential stages accompanied by crises — leadership, autonomy, control, coordination, collaboration. Empirical support is weak but not absent; the sequences are probabilistic, not deterministic.

---

### Cross-paper synthesis (§4f)

**1. Stochastic dominance as the central empirical regularity.** Coad's survey makes this unavoidable: the R² of firm growth regressions is 2–10%. This is not a failure of the empirical literature — it is a finding. Firm growth is predominantly stochastic at the individual firm level. For the project, this means: (a) trade shocks will explain only a fraction of the variance in firm-level capability change; (b) identifying causal effects requires carefully designed quasi-experimental variation (DiD, IV), not OLS with controls; (c) standard errors on all growth rate regressions should be expected to be large relative to point estimates.

**2. "Survival of the fitter" without "growth of the fitter."** The most striking empirical claim in the survey: selection via differential growth does not work. Productive and profitable firms do not grow faster — they exit less. This challenges the evolutionary story that market competition reallocates resources toward better firms. For the capability/trade-shock project: if pre-shock capability advantages don't translate into faster growth, then a trade shock that reduces capability may not show up clearly in growth outcomes — it may show up in exit probabilities instead. The research design needs to test both margins.

**3. Innovation matters at the tail, not the mean.** This is a direct methodological recommendation for the project: use quantile regression (or flexible distributional approaches) to assess the effect of capability portfolios and trade shocks on growth. The effect of capabilities on becoming a fast-growth exporter is likely concentrated in the upper tail of the growth distribution and will be missed by OLS.

**4. Penrose as the best theoretical framework — but stochastic.** The Penrose theory of growth (excess resources → capability accumulation → diversification) is the most empirically consistent framework in Coad's assessment, but it must be understood as generating tendencies not determinisms. The "Penrose effect" (above an optimal growth rate, growth is costly) implies diminishing returns to rapid capability reconfiguration — firms that diversify too fast bear coordination costs.

**5. Diversification strategy: the related/unrelated axis.** The empirical verdict is that related diversification is superior to unrelated diversification. This is the empirical counterpart to the Teece coherence argument (§4a) and the Patel-Pavitt RTA finding (§4c) that technological profiles are organized around a core capability field. The EFC literature (Batch 1) operationalizes this as the "density" of a firm's position in the product-capability network — high density = related diversification; low density = unrelated exposure.

**6. Position of §4f in the reading sequence.** The Coad survey sits at the end of Batch 4's theoretical-empirical foundations block (Penrose → Teece → Dosi → Bell/March/Patel → Storper → Bottazzi-Secchi → Coad) and performs a critical function: it calibrates expectations about what cross-sectional regressions of firm growth can deliver. After this foundation layer, the project's empirical identification challenge is clear: given that growth is predominantly stochastic and standard determinants explain only 5-10% of variance, the research design must exploit credible quasi-experimental variation (tariff shocks) and must focus on the right outcome variable (capability portfolio composition and export scope, not just growth rate) using flexible distributional methods.

---

## §4e — Firm growth distributions: the Bottazzi-Secchi programme (Batch 4e) — Firm growth distributions: the Bottazzi-Secchi programme (Batch 4e)

*Papers read in full 2026-06-04.*
*Bottazzi & Secchi (2003) "Common Properties and Sectoral Specificities in the Dynamics of U.S. Manufacturing Companies," Review of Industrial Organization 23: 217–232.*
*Bottazzi & Secchi (2005) "Growth and Diversification Patterns of the Worldwide Pharmaceutical Industry," Review of Industrial Organization 26: 195–216.*
*Bottazzi & Secchi (2006) "Gibrat's Law and Diversification," Industrial and Corporate Change 15(5): 847–875.*

These three papers constitute a coherent and progressive empirical-theoretical programme. Each article builds on the previous one, moving from documenting cross-sectoral stylized facts (2003), to exploring them in high-resolution disaggregated data (2005), to providing a full mechanistic explanation and a validated stochastic model (2006). They are treated as a single unit below.

---

### The empirical core: stylized facts on firm growth (Bottazzi & Secchi 2003)

- **Data.** COMPUSTAT US manufacturing, 1982–2001; balanced panel of 1,025 firms (1993–2001) and unbalanced panel of >3,000 firms. 15 2-digit SIC sectors (SIC 20–39 with >21 firms each).

- **Four sector-invariant findings.** The paper's central contribution is identifying statistical properties that survive disaggregation from aggregate US manufacturing to individual 2-digit sectors (Table III):

  1. **Stationarity of size distribution.** The firm size distribution (log-normal shape) is stable over time in all sectors. The moments of log-size are essentially constant across the 1993–2001 window.
  2. **Unit root in growth process.** AR(1) coefficient on log-size: φ = 0.9576 (SE = 0.005). Sectoral estimates: all significant and in [0.88, 0.99]. The growth process is a geometric Brownian motion — size today is the best predictor of size tomorrow (Gibrat's Law validated for the mean). This is robust at both aggregate and sectoral levels.
  3. **Variance-size power law.** The standard deviation of growth rates scales with firm size as σ(g|S) ~ S^β, with β ≈ -0.19 (aggregate) and sector-by-sector range of -0.138 to -0.217. Larger firms have less volatile growth — a "second-order" violation of Gibrat's Law that is itself invariant across sectors (Table II).
  4. **Laplace growth rate density.** After rescaling growth rates by the variance-size relation, the empirical density of normalized growth rates ĝ is well described by the Subbotin distribution with b ≈ 1.0 (Laplace / symmetric exponential), not b = 2 (Gaussian). This holds in each sector separately (all sectors: b ∈ [0.80, 1.21]). The tent shape — fat tails with sharp peak — signals that most firms grow approximately as before, but a nontrivial fraction exhibit very large positive or negative shocks.

- **Two sector-specific (non-invariant) findings.** Shape of the size distribution (log-normal aggregate vs. skewed, bimodal, or asymmetric in individual sectors) and the AR structure in growth rates (some sectors show positive autocorrelation, some negative, some none) are both sector-specific. The sectoral AR structure is plausibly driven by macroeconomic cycles, sector-level price dynamics, or demand shifts — not generic firm behavior.

- **Interpretive claim.** The invariant properties (unit root, variance-size scaling, Laplace density) arise from a fundamental, sector-transcendent economic process. The 2003 companion paper (Bottazzi & Secchi 2003a, cited as Economics Letters) shows the tent shape emerges from a positive-feedback mechanism in growth. A separate paper (Bottazzi 2001) derives the variance-size relation as a diversification effect. The 2006 paper closes the loop.

---

### Disaggregated evidence: pharmaceutical industry (Bottazzi & Secchi 2005)

- **Data.** Pharmaceutical Industry Database (PHID), 198 top worldwide pharmaceutical firms, 7,654 drug products aggregated into 517 four-digit ACS (Anatomical Classification System) submarkets, seven western markets (US, UK, France, Germany, Spain, Italy, Canada), 1987–1997. Balanced panel; "super-firms" constructed to absorb M&A (all mergers treated as merged from period start).

- **Replication results.** All four sector-invariant findings from 2003 replicate:
  - Unit root: φ = 0.956 (consistent)
  - Variance-size: β = -0.209 (consistent)
  - Growth density: b ≈ 0.97 after rescaling (Laplace, consistent)

- **Pharma-specific deviation.** Growth rates show weak positive AR(2) autocorrelation (φ₁ = 0.097, φ₂ = 0.106, both significant), not found in US manufacturing. Interpreted as mild self-reinforcing competitive advantage or disadvantage in the pharmaceutical context.

- **Bimodal size distribution.** Firm size distribution is persistently bimodal: a "core" of ~20 dominant incumbents (Roche, Merck, Novartis, Pfizer, Glaxo Wellcome, etc.) and a large lower tier. This bimodality is statistically significant (Silverman–Hall–York multimodality test: rejected unimodality at p < 0.05 in 7 of 11 years). A firm in the lower tier would need sustained 20% annual growth for 20 years to reach the upper tier — structurally rare.

- **Novel diversification analysis.** The paper exploits four-digit ACS sub-market data to study diversification patterns:
  1. **Size-scope scaling.** The number of active sub-markets N scales with firm size S as log(N) = α + 0.385 log(S) (SE = 0.024). Larger firms operate in more sub-markets.
  2. **Diversification symmetry is size-invariant.** How firms distribute their sales across their active sub-markets (the Δ index: 0 = perfectly symmetric, 1 = fully concentrated in one) is essentially independent of firm size. The slope is -0.025 (SE = 0.004) — statistically significant but economically negligible (a tenfold size increase changes Δ by <3%).
  3. **Cross-submarket growth independence.** The cross-correlation of growth rates across a firm's active sub-markets has mean r ≈ 0.006 and SD ≈ 0.057 — statistically indistinguishable from zero for all firms. Growth in different product categories is driven by independent processes. This is the key finding enabling the 2006 explanation.

---

### The mechanism: scope economy to diversification (Bottazzi & Secchi 2006)

- **The explanandum.** The variance-size scaling β ≈ -0.21 is softer than the Central Limit Theorem prediction of β = -0.5 (which would apply if a firm were simply a portfolio of N independent, equal-sized sub-businesses). Why is diversification not a more effective risk reducer?

- **The decomposition.** Writing aggregate firm growth as a weighted sum of sub-market growth rates (eq. 10), and exploiting cross-submarket independence, the variance of aggregate growth decomposes into a sum of sub-market variances weighted by sub-market shares (eq. 12). The variance-size relation therefore has exactly three possible sources:
  1. Sub-market growth rates depend on firm size (scale economies/diseconomies in competitive performance) → *not found* (Figure 4–5 confirm no relation between sub-market growth mean or variance and firm size)
  2. Distribution of sales across sub-markets (Δ index) depends on firm size → *not found* (Δ is size-independent, as in 2005)
  3. Number of active sub-markets N depends on firm size → *confirmed* (N ~ S^0.35)

  The variance-size exponent then follows from the CLT: β = -λ/2 = -0.35/2 = -0.175, which agrees with the observed β ≈ -0.21. **The entire variance-size violation of Gibrat's Law is explained by the diversification structure of the firm, with no additional assumptions about internal firm organization or cross-unit correlations.**

- **Why is β ≈ -0.21 and not -0.50?** Because N ~ S^0.35, not N ~ S^1. Firms do not expand sub-market scope proportionally to size — they expand at a sub-linear rate (exponent 0.35 < 1). Thus diversification is a real but imperfect portfolio: larger firms are less volatile, but they would need to be 10× larger to halve their volatility (not 4× as the CLT would imply with linear scope scaling).

- **Three stochastic models of diversification dynamics** (validated against empirical mean-variance-of-N relationship):
  1. **Model I: Linear Poisson.** Each unit of growth independently triggers a constant-rate chance of entering a new sub-market. Predicts N grows linearly with S → inconsistent with super-linear empirical scaling.
  2. **Model II: Non-linear Poisson (scale economy).** Arrival rate of diversification events increases with firm size. Can reproduce mean-N vs. S but predicts variance of N grows linearly with mean-N → inconsistent with data (Figure 10 shows a clearly super-linear mean-variance relationship).
  3. **Model III: Yule process (scope economy).** Each currently active sub-market is a potential seed for a new sub-market entry (branching process, Figure 9). The arrival rate of diversification events is proportional to the current number of active sub-markets: P(enter new sub-market | size increases by δ) = n·λ·δ. This generates: (a) exponential growth of mean-N with S (consistent with observed log-linear scaling); (b) quadratic relation between variance and mean of N (consistent with Figure 10); (c) distribution of N consistent with observed empirical distribution (Figure 11, λ = 0.35, n₀ = 5).

- **Theoretical interpretation.** The Yule branching process is explicitly grounded in Penrosian and evolutionary economics: "the ability to diversify into new sub-markets increases with the number of sub-markets already penetrated" — a direct formalization of capability accumulation. Each existing competency is a potential seed for further expansion. This is scope economy, not scale economy: entry probability does not depend on size per se but on the *diversity* of existing capabilities. The result: "competencies are accumulated by a firm at a pace that is less than proportional to its growth rate" — diversification is capability-constrained, not resource-constrained.

---

### Cross-paper synthesis (§4e)

**1. The Bottazzi-Secchi empirical programme as a foundation.** These three papers together establish the empirical baseline for any firm-level growth analysis relevant to the project. Four facts must hold in any microdata (firm × product × time): Laplace-distributed growth rates, unit-root size dynamics, variance-size scaling (β ≈ -0.2), and super-linear scope-size scaling (N ~ S^0.35). Any model or regression that assumes Gaussian errors or that treats variance as size-independent will be misspecified.

**2. Diversification as the key micro-mechanism.** The 2006 paper provides the cleanest possible empirical argument: the variance-size relation is *entirely* a diversification effect. Nothing else (scale economies, correlated sub-unit dynamics, internal organization) is needed. This directly supports the project's focus on firm-level diversification as the operative mechanism connecting capability accumulation to competitive performance.

**3. The Yule branching model ≈ cumulative capability accumulation.** Model III (Yule) is the stochastic dynamic analog of the static Patel-Pavitt RTA profiles (§4c): both capture that a firm's current capability portfolio constrains and seeds its future portfolio. The transition from static (Patel-Pavitt: snapshot of capability breadth) to dynamic (Yule: evolution of capability breadth over time as a branching process) is the key conceptual step for modeling how firms accumulate and reconfigure capabilities in response to trade shocks.

**4. Cross-submarket independence as an identifying assumption.** The finding that sub-market growth rates are near-zero correlated within firms — that firm-level diversification is across genuinely independent competitive processes — is a strong identifying assumption. In the capability/trade-shock context: if a trade shock hits sub-market j for firm i, there is no automatic spillover to sub-market j' for the same firm. This means shocks are idiosyncratic at the product level, and the aggregate effect on a firm depends on its diversification structure (how many active products, how sales are distributed). Firms with more product diversity are mechanically more insulated — a testable hypothesis.

**5. Bimodal size distribution in pharmaceuticals.** The pharma-specific finding of bimodality (core vs. periphery) generalizes to the question of whether firm-level EFC scores display a similar dual structure: a small group of firms that persistently hold highly diversified, central positions in the capability network, and a larger group with narrow specializations. The Guan_2020 and Bontadini_2021 papers (Batch 1) find precisely this.

**6. What remains.** The Bottazzi-Secchi programme ignores relatedness — it treats all sub-market entries as equivalent, whether the new sub-market is adjacent or distant in product space. The EFC literature (Batch 1) and the complexity/relatedness literature (Batch 2) add the spatial structure: not all N active sub-markets are equally valuable, and entry into related vs. unrelated sub-markets has different implications for capability accumulation. The Yule branching model predicts the *number* of active sub-markets but not their *location* in product space. Extending the Yule model to a product-space branching model (where entry probability depends on relatededness) is a natural direction — and arguably the core of what EFC does empirically.

---

## §2a — Product sophistication and the capabilities network (Batch 2a)

*Papers read in full 2026-06-04: Hausmann, Hwang & Rodrik (2007) "What you export matters"; Hausmann & Hidalgo (2011) "The network structure of economic output."*

Batch 2a opens the complexity/fitness-foundations layer. These two papers are the direct intellectual ancestors of the EFC framework and of the project's core empirical machinery: PRODY/EXPY are the macroeconomic precursors of firm-level EFC scores; the bipartite capabilities model in Hausmann-Hidalgo 2011 is the formal substrate on which BRIM community detection and the firm × product matrix operate. Understanding both at the level of their formal arguments — not just their conclusions — is essential for situating the project's contribution.

---

### Hausmann, Hwang & Rodrik (2007) — "What you export matters"
*Journal of Economic Growth 12(1): 1–25*

- **Main contribution.** A theory and empirical test of the claim that not all goods are equal: the *income level associated with a country's exports* predicts subsequent economic growth above and beyond the usual growth correlates. The paper introduces two indices — PRODY (income level associated with a product) and EXPY (income level associated with a country's export basket) — and shows that high-EXPY countries grow systematically faster. The mechanism is "cost discovery": entrepreneurial investment in new activities generates knowledge spillovers for imitators (returns to the pioneer are socialized), leading to sub-optimal entry in new activities and a structural role for industrial policy.

- **Theory.** A two-sector general-equilibrium model: a traditional sector (single homogeneous good, diminishing marginal product of labour) and a modern sector producing a continuum of goods indexed by productivity θ ∈ [0,h], where h proxies human capital (it determines what goods are "discoverable"). Projects are of fixed cost b (in labour) and θ is drawn from Uniform[0,h] ex ante — unknown until the investment is sunk. Once θ is discovered, it becomes common knowledge; emulators operate at fraction α of incumbent productivity. The equilibrium number of modern-sector entrants m* is determined by zero-profit condition (ZP) and labour market clearing (LL) — both upward sloping in (m,w)-space. Key result: expected productivity in the modern sector scales as h·[1 + αm/(m+1)]²/2, so *information spillovers generate increasing returns at the sector level without technological externalities*. Larger labour endowment L increases m* and — paradoxically — raises wages in long-run equilibrium, because modern-sector productivity rises with m.

- **Data and method.** COMTRADE HS6 (1992–2003, 113 countries, 5,023 products) and World Trade Flows SITC4 (1962–2000, 97 countries, 700+ products). PRODY for product k is constructed as:
  > PRODY_k = Σ_j [(x_jk/X_j) / Σ_j(x_jk/X_j)] · Y_j
  using RCA-based export-value-share weights so that large countries do not dominate (Bangladesh outweighs the US in garment PRODY because garments are a larger share of Bangladesh's basket). EXPY for country i is the export-value-share-weighted average of PRODY across its products. Growth regressions use OLS, IV (instruments: log population, log land area — plausibly exogenous to growth through channels other than EXPY), country fixed effects, and Blundell-Bond GMM.

- **Key findings.**
  1. **PRODY range is vast.** Within the HS6 classification, PRODY spans from ~$750 (vanilla beans, cloves — primary exports of poor Sub-Saharan countries) to ~$47,000 (flat rolled steel coated with aluminium — dominant export of Luxembourg). The variance in product income levels is enormous.
  2. **EXPY strongly predicts growth.** Cross-section: estimated coefficient on log EXPY ranges 0.032–0.082 depending on specification; 10% increase in EXPY → 0.3–0.8 pp higher growth. IV estimates exceed OLS. Panel with country fixed effects (1962–2000): coefficient 0.014–0.019; 10% increase in EXPY → 0.14–0.19 pp growth, identifying off within-country variation in export sophistication over time.
  3. **Effect concentrated in middle-income countries.** Fixed-effects estimates are zero for OECD (low within-country variance in EXPY) and low-income countries (measurement error in trade statistics). MIDLW sub-sample gives FE coefficients 0.035–0.037, double the full-sample estimate.
  4. **China and India are positive outliers.** China's EXPY exceeds Brazil, Argentina, Chile — all 3–4× richer in per-capita terms. India's EXPY (2003) exceeds Argentina. This is consistent with both countries' subsequent high growth and their deliberate industrial policy favouring sophisticated manufacturing.
  5. **EXPY is not explained by institutions.** Rule of Law index enters insignificantly once GDP per capita is controlled (Table 7, col. 3). EXPY has residual variation unexplained by GDP, human capital, population and land area — this residual is the "idiosyncratic" component of specialisation.
  6. **Mechanism confirmation.** Countries with high initial EXPY experience faster subsequent export growth (Fig. 9), consistent with elastic world demand for sophisticated goods and with the cost-discovery process.

- **Relevance to project.** EXPY is included as a control variable in the project's regressions (product-sophistication control, per research spec). This paper establishes what EXPY measures and why it matters. More fundamentally, the cost-discovery mechanism is the country-level analogue of what we model at the firm level: firms that invest in new product capabilities face cost uncertainty, and capability accumulation (analogous to cost discovery) has spillover effects mediated through the network. The paper's key prediction — that *what* a country/firm exports matters beyond quantity or total value — is the organizing principle of EFC and of the project's RQ.

---

### Hausmann & Hidalgo (2011) — "The network structure of economic output"
*Journal of Economic Growth 16(3): 309–342*

- **Main contribution.** A network analysis of the bipartite country × product matrix (M_cp) that establishes four empirical stylized facts about its structure, proposes a capabilities model that explains three of the four, and derives from the model the existence of a *quiescence trap* — a poverty trap grounded in the complementarity of capabilities rather than in capital or institutions. The paper is the formal underpinning of Economic Complexity: it shows that the triangular (not block-diagonal) structure of M_cp implies that diversification and ubiquity are inversely and *structurally* related, in a way that standard trade theories do not predict.

- **Data and method.** Two trade datasets: (1) Feenstra et al. SITC4 rev.2 (1962–2000, 129 countries, 772 products); (2) BACI/CEPII HS6 (232 countries, 5,109 products, year 2005). Robustness check: Chilean municipality × industry matrix (347 municipalities, 700 industries including non-tradables). RCA binarised at threshold R* ∈ {0.5, 1.0} to form M_cp. Key objects:
  - kc,0 = diversification of country c (number of products with RCA > R*)
  - kp,0 = ubiquity of product p (number of countries with RCA > R*)
  - kc,1 = average ubiquity of c's products
  - kp,1 = average diversification of p's exporters
  - φ_pp' = min conditional co-export probability (proximity between products p and p')

- **Four stylized facts.**
  1. *Diversification and ubiquity are inversely related.* M_cp is triangular: poorly diversified countries export high-ubiquity (many-country) products; highly diversified countries export low-ubiquity (few-country) products. kc,0 − kc,1 diagram has strong negative slope. Validated with four null models at p < 0.001, and replicated on Chilean municipal data.
  2. *Product ubiquity is non-normally distributed.* Better fit by log-normal or Weibull than normal. Departure from normality is statistically significant.
  3. *Country diversification is non-normally distributed.* Log-normal / Weibull fit. The heterogeneity in diversification (variance relative to mean) is much larger than for ubiquity — a key asymmetry.
  4. *Co-export proximity is non-normally distributed.* Weibull distribution is the consistent best fit.

- **Capabilities model (binomial model).**
  Countries and products are described by binary vectors in capability space (Na capabilities). Country c has capability a independently with prob r; product p requires capability a independently with prob q. The country-product link M_cp = 1 iff the full set of capabilities required by p is a subset of those present in c (Leontief / subset operator). This is a Leontief production function in binary/capability form: no substitution between required inputs, but the identity of inputs is unrestricted. The model has three parameters (r, q, Na) reduced to two (r, Na) by matching network density η = r^(q·Na) to data.

  Mean-field predictions (derived analytically via the binomial theorem):
  > kc,0 = Np · [q·(kc,0^a/Na) + 1 − q]^Na          (diversification as function of capabilities)
  > kp,0 = Nc · r^(kp,0^a)                              (ubiquity falls with capability requirements)
  > kc,1 = Nc · [r·q^(kc,0/Np)^(1/Na) + (1−q)(1−r)]^Na  (average ubiquity falls with diversification)

  Calibration: best fit at Na ≈ 65–80, r ≈ 0.80–0.89. The model fits stylized facts 1, 2, and 4 but *cannot* reproduce the full heterogeneity in stylized fact 3 (diversification distribution) unless each country is allowed its own rc — which is interpreted as direct evidence of large heterogeneity in capability endowments across countries.

- **The quiescence trap.**
  The key theoretical result: diversification is a *convex* function of capabilities. Second derivative d²kc,0/d(kc,0^a)² > 0 for all Na > 1, regardless of the structure of C_ca and P_pa (proved for any Leontief-type operator with uncorrelated capability endowments). Interpretation: a country with few capabilities gets near-zero marginal product from any single additional capability, because products require *all* of the requisite inputs — one missing capability = zero output. A country with many capabilities gets large marginal product from any additional capability, because it can combine the new input with the many existing combinations already present. The returns to capability accumulation are increasing in the existing capability stock. Calibration with Na ≈ 65–80 places the world in a strong quiescence trap regime: Fig. 11 shows the capability-diversity relation is highly convex at the calibrated parameters, consistent with the observed bimodal world income distribution.

  This trap differs from the Rosenstein-Rodan / Murphy-Shleifer-Vishny big push (complementarities among few industries with scale economies): in the capability world, there are *dozens* of capabilities and 2^Na potential combinations, making targeted provision of any single missing capability unlikely to resolve the trap. The trap is endogenous to the complexity of the global economy, not just to aggregate investment levels.

- **Comparison with prior theory.**
  - Classical HO / Ricardo: explains specialization, makes no prediction on diversification levels or diversity-ubiquity relationship.
  - New trade theory (Dixit-Stiglitz): symmetric goods, no predictions on which goods are made where.
  - Melitz (2003): firm heterogeneity explains firm-level trade participation, but matrix would be block-diagonal not triangular.
  - Kremer (1993) O-ring: matrix should be block-diagonal (countries specialize in either complex or simple products); data is triangular. O-ring rejected.
  - Weitzman (1998) recombinant growth: related conceptually, but no predictions on country-product network structure or diversity-ubiquity relationship.

- **Relevance to project.** This paper establishes the formal scaffolding on which all EFC work rests. The M_cp matrix in this paper = our firm-product bipartite matrix M_ipt (with countries → firms, products → exported HS products, RCA → firm-level RCA). The four stylized facts should also hold (approximately) in the firm-product bipartite network for Chinese exporters — this is an implicit robustness check for our data construction. The capabilities model formalises the latent structure that BRIM community detection is recovering: each block (community) in the bipartite network corresponds to a latent capability cluster. The Leontief complementarity assumption is the formal statement of why blocks are coherent: firms that share capabilities co-specialize in the same product cluster, and products in the same block require a similar capability bundle. Most importantly, the quiescence trap is our theoretical motivation for the asymmetric response to trade shocks: firms with few capabilities (peripheral in the network, exporting few and highly ubiquitous products) face near-zero gains from exploring new product directions — they are capability-constrained. Firms with many capabilities (central in the network, exporting many low-ubiquity products) can recombine existing capabilities into new combinations after a shock. This is the micro-mechanism we are identifying with the Bartik tariff exposure.

---

### Cross-paper synthesis (§2a)

**1. EXPY is a country-level EFC score.** EXPY assigns each country a productivity level based on what it exports, using RCA weights. This is structurally identical to the EFC country complexity index (which assigns income-predictive capability scores by iterating on the bipartite network). The 2007 paper establishes the rationale; the 2009 Hidalgo-Hausmann PNAS paper (Batch 2c) will refine the measure to pure network iteration. For the project: EXPY enters as a product-sophistication control in the firm-level regressions precisely because we need to separate "firm exports sophisticated products" from "firm is more capable after controlling for sophistication." EXPY is the right-hand-side version of what EFC measures on the left.

**2. The bipartite network is the methodological backbone.** Hausmann-Hidalgo 2011 demonstrates that the bipartite country-product matrix is *not* a random allocation but has deeply non-random structure (triangular, power-law distributions, Weibull co-export proximity) that is explained by a latent capability architecture. Translating this from country-product to firm-product (our M_ipt) is the central methodological step in the EFC literature (De Stefano 2025, Batch 1). The data moment that validates our network construction is whether the firm-product bipartite matrix for Chinese exporters also exhibits the triangular shape and non-normal distributions established here.

**3. Capabilities are not directly observable; network structure identifies them.** Both papers treat capabilities as latent. The 2007 paper avoids defining them; the 2011 paper formalises this agnosticism (binary vectors with probability r per capability, no assumption about their nature) and shows that capability diversity can be *inferred* from the network structure without knowing what capabilities are. This validates the use of BRIM community detection as a measurement device: block structure in the bipartite network = latent capability clusters, identified without needing to observe capabilities directly.

**4. The quiescence trap grounds our heterogeneous treatment effects.** The central empirical prediction from Hausmann-Hidalgo 2011 is that returns to capability accumulation are convex: low-capability entities gain little from any single new input; high-capability entities gain a lot. At the firm level, this predicts that tariff shocks (which destroy or displace capabilities at the product level) have asymmetric effects by prior capability stock. A shock that destroys one product for a peripheral firm (few capabilities) has near-zero effect on its ability to reconfigure: it was already capability-constrained. A shock that destroys one product for a central firm (many capabilities) has a larger relative effect but also leaves the firm with more recombination options. This asymmetry — central firms reconfigure within-core; peripheral firms exit or remain stuck — is the heterogeneous treatment effect we are testing.

**5. Cost discovery ↔ capability accumulation.** The 2007 mechanism (cost discovery generates knowledge spillovers, leading to sub-optimal entry) is the country-level version of Penrose's "excess productive services" (§4a) and Dosi's "technological regime" (§4b). All three describe the same phenomenon at different levels of aggregation: the productive knowledge required to enter a new activity is (i) uncertain ex ante, (ii) learnable through experience, and (iii) partially public — generating externalities that under-incentivize capability investment at the social level. For the project, this means the tariff shock is not just a demand shock (fewer destination markets, lower prices) but a capability-disruption shock: the entrepreneur who was engaged in cost discovery for products in the affected destination-product cells loses the returns on that discovery, reducing the productivity of the remaining capability portfolio.

**6. Where these papers end and the project begins.** Both papers operate at the country level. The key insight that does *not* appear in either paper — and is the project's contribution — is that the bipartite structure can be taken to the firm level, the treatment can be exogenous (Bartik tariff shock), and the outcome can be block-consistent diversification (d_in vs d_out) rather than aggregate growth. The quiescence trap prediction is theoretically clean but has never been tested causally at the firm level with an identified shock. The project does exactly this.

---

## §2b — The Fitness-Complexity algorithm and the predictability of growth (Batch 2b)

*Papers read in full 2026-06-04: Cristelli, Gabrielli, Tacchella, Caldarelli & Pietronero (2013) "Measuring the Intangibles"; Cristelli, Tacchella, Cader, Roster & Pietronero (2017) "On the Predictability of Growth."*

Batch 2b completes the measurement foundations for Fitness/EFC. Cristelli 2013 formally introduces and defends the non-linear Fitness-Complexity (FC) algorithm that replaces Hidalgo-Hausmann's Method of Reflections (MR), and is the measure used throughout the EFC literature (including De Stefano 2025, Batch 1). Cristelli 2017 applies Fitness to growth forecasting at the country level and introduces the concept of *selective predictability* — heterogeneous growth regimes that map directly onto the project's heterogeneous treatment-effect predictions.

---

### Cristelli, Gabrielli, Tacchella, Caldarelli & Pietronero (2013) — "Measuring the Intangibles: A Metrics for the Economic Complexity of Countries and Products"
*PLoS ONE 8(8): e70726*

- **Main contribution.** Proposes and validates the Fitness-Complexity (FC) algorithm as a mathematically and economically superior replacement for the Hidalgo-Hausmann Method of Reflections (MR). The core argument is that the triangular structure of M_cp implies that: (1) country fitness should sum (not average) product complexities, so that diversification is a direct competitive advantage; and (2) product complexity must be bounded by the fitness of its *least* fit exporter — not the average — because a product exported by a poor country cannot be a complex product, regardless of how diversified a country exporting it is.

- **Data.** BACI HS4 (1131 products, ~200 countries, 1995–2010). Binary M_cp with RCA threshold = 1. Unweighted (binary) and weighted versions analyzed.

- **The FC algorithm.** The iterative non-linear map is defined by two equations per iteration:
  > F̃_c^(n) = Σ_p M_cp · Q_p^(n−1)           [sum of complexity-weighted exports]
  > Q̃_p^(n) = 1 / Σ_c [M_cp / F_c^(n−1)]      [harmonic mean of exporters' fitness]
  > Normalized: F_c^(n) = F̃_c^(n) / ⟨F̃^(n)⟩; Q_p^(n) = Q̃_p^(n) / ⟨Q̃^(n)⟩

  The algorithm converges to a unique, globally attracting non-trivial fixed point for any M_cp consistent with the triangular structure of real trade data — proved numerically for >300 random triangular matrices of varying sizes. Convergence is exponential (Euclidean distance ∝ e^{−γn}, γ ≈ 0.28 for Nc=150). Starting conditions do not affect the fixed point.

- **Fitness measures intensivity vs. extensivity.** The binary (unweighted) FC gives *intensive fitness* — analogous to GDP per capita (diversification per se, not volumes). The weighted version gives *extensive fitness* — analogous to total GDP (China ranks 1st extensive vs. 2nd intensive; Italy ranks 3rd intensive vs. 5th extensive). For the project, intensive fitness (binary M) is the relevant measure because we care about the capability structure of the firm, not export volumes.

- **Key critique of Method of Reflections (MR).** MR defines k_c^(n+1) and k_p^(n+1) as arithmetic *averages* of neighbors' values. This has three fatal problems:
  1. *Dimensionality flip*: k_c^0 = diversification (extensive), k_c^2 = average complexity (intensive), k_c^4 = average of average (even more averaged) — the economic meaning of the iterated variable changes at every order.
  2. *Trivial fixed point*: MR is the transposed of an ergodic Markov transition operator; iterating to convergence gives k_c^(2n) → constant for all c. The authors subtract the mean before analysis — but this means the "index" they report is the second eigenvector of a Markov matrix, not a self-consistent fixed point.
  3. *Diversification ignored*: A country with 500 products at average complexity k̄ scores identically to a country with 1 product at complexity k̄ in MR. Directly contradicts the capabilities framework: diversification *is* the competitive advantage.

- **Economic results — BRIC.** China and India have strongly increasing intensive fitness 1995–2010 (China: 13th → 2nd). Brazil and Russia have *declining* fitness despite rising GDP — commodity-price driven growth with no capability accumulation. MR ranks China 33rd (just above Romania), India far below Qatar — economically implausible. FC correctly identifies China's spectacular industrial upgrading.

- **Economic results — PIIGS.** All PIIGS have high or rising intensive fitness — Italy is consistently top 3 (>500 products with RCA>1, most diversified European exporter). But PIIGS have financial fragility. Resolution: developed countries have "saturated" their capability phase space; for them, growth is driven by politics, finance, and non-capability factors, not further capability accumulation. This two-regime observation (capability-driven growth for emerging countries; finance/policy-driven for developed) foreshadows the predictability story in Cristelli 2017.

- **Product complexity.** The non-linear harmonic mean formula makes Q_p very sensitive to entry by low-fitness exporters. Product complexity falls when a new low-fitness country begins exporting it. This creates higher volatility for Q_p than for F_c (the sum of products stabilizes; any single product's complexity fluctuates). Implication: trend analysis of product complexity is meaningful; single-year snapshots are noisy.

- **Relevance to project.** The FC algorithm IS the Fitness measure underlying EFC (De Stefano 2025, Batch 1; Pugliese 2017/2019, Batch 1). Understanding why FC beats MR is critical for the validity of the entire EFC framework: it is not an arbitrary algorithmic choice, but the mathematically necessary implementation of the Leontief complementarity assumption (Hausmann-Hidalgo 2011). The non-linearity of the complexity measure means that product complexity = 0 whenever any capability is missing from the exporting country's set — exactly the Leontief condition. For the project, the FC algorithm applied at the *firm* level produces firm-fitness scores. These are the capability measures that determine a firm's block membership in BRIM and its position on the capability ladder — central firms export many low-ubiquity products, peripheral firms export few high-ubiquity products.

---

### Cristelli, Tacchella, Cader, Roster & Pietronero (2017) — "On the Predictability of Growth"
*World Bank Policy Research Working Paper 8117*

- **Main contribution.** Introduces the Selective Predictability Scheme (SPS): a non-parametric growth forecasting method using the Fitness-GDPpc plane as a 2D phase space. Historical comparator countries (those that were in the past in the same neighborhood of the Fitness-GDPpc plane) provide the trajectory estimates for a country's future growth. The paper's main discovery is that growth predictability is *heterogeneous*: countries in the right-upper region of the Fitness-GDPpc plane (high Fitness, moderate-to-high GDP) follow *laminar* (predictable, coherent) trajectories; countries in the lower-left (low Fitness) follow *chaotic* (unpredictable, divergent) trajectories.

- **Data.** BACI HS4 (1995–2014, ~140 countries after filter). Fitness from Tacchella et al. (2012)/Cristelli et al. (2013). GDPpc PPP (World Bank). IMF World Economic Outlook 5-year projections (2007–2015). Benchmark models: last-period growth (Model 1), AR(1) (Model 2), AR(1) + trend (Model 3).

- **The Fitness-GDPpc plane.** Country trajectories in log(Fitness) × log(GDPpc) space reveal a structured flow field. The local 1-year average displacement field (averaged over a grid in the plane) shows: (1) in the right part of the plane (high Fitness countries), arrows point consistently rightward and upward — laminar flow; (2) in the left part (low Fitness), arrows are incoherent — chaotic flow. Kenya and Uganda in 2017 are at the position of Vietnam in the early 1990s; South Korea in the 1970s. The phase space enables time-independent comparisons of economic states.

- **SPS methodology (three-step kernel regression).**
  1. *Comparator selection*: For country c at time t0, find all past observations (c', t) with Euclidean distance ‖(log F_{c',t}, log Y_{c',t}) − (log F_{c,t0}, log Y_{c,t0})‖ < r, where c' ≠ c and t < t0. Default r = 0.6 (robustness verified for r ∈ [0.3, 0.9]).
  2. *Trajectory averaging*: Project the average D-period-ahead displacement of comparators' trajectories onto the reference country.
  3. *Predictability P*: ratio of initial dispersion of comparators to their dispersion D periods later: P = σ_initial / σ_final. P > 1: trajectories converge (predictable); P < 1: trajectories diverge (chaotic). Threshold ln(P) ≈ −0.25 (median of the Fitness-marginalised distribution) ≡ ln(Fitness) ≈ −1 separates laminar from chaotic regime.

- **Key results — SPS vs IMF.**
  | | PC | MAE | RMSE |
  |---|---|---|---|
  | SPS (all) | 0.30 | 2.01 | 2.64 |
  | SPS + trend (all) | 0.37 | 1.97 | 2.60 |
  | IMF (all) | 0.42 | 2.03 | 3.05 |
  
  IMF has 10% higher directional correlation (PC); SPS is 1–15% more accurate in magnitude (MAE, RMSE). A single-parameter, parameter-free global model matches country-specific IMF models on a 5-year horizon.

- **Key results — P vs UnP regimes.**
  - ~60% of events are in the predictable (P) regime; ~40% unpredictable (UnP).
  - In the P regime: SPS MAE = 1.81 vs. IMF MAE = 1.87 → SPS matches or outperforms IMF.
  - In the UnP regime: SPS MAE = 2.26 vs. IMF MAE = 2.22 → both worsen substantially.
  - IMF P accuracy is 19% better on MAE and 33% better on RMSE than IMF UnP accuracy. The predictability dimension works equally well as a segmentation criterion for IMF projections — confirming that P captures a real feature of economies, not an artefact of the SPS method.
  
- **Growth improves at longer horizons.** At 9-year horizon, SPS MAE is ~25% lower and RMSE ~30% lower than at 5-year horizon. This is the opposite of what most econometric models find. Explanation: short-term growth is dominated by business-cycle shocks (which SPS doesn't model); long-term growth is dominated by the structural capability-accumulation trajectory, which Fitness captures.

- **Case studies: Thailand vs Ghana.** Both have similar predicted growth (5.4% vs 5.15% CAGR 2014–2019). Thailand is in the laminar regime (P = 1.1); Ghana is in the chaotic regime (P = 0.5). Thailand's 53 comparators (Brazil 1995, Indonesia 2000, Bulgaria, Romania, …) follow coherent trajectories in the Fitness-GDPpc plane. Ghana's comparators are heterogeneous, strongly dependent on natural resources (10% of GDP from natural resources, vs 1.9% for Thailand's comparators). The predictability score reflects this structural difference.

- **Economic interpretation of regimes.** Countries in the laminar regime have high enough Fitness that their development trajectories are "on rails": their capability endowment constrains the set of feasible new activities, and any new capability is immediately put to productive use (cf. quiescence trap from Hausmann-Hidalgo 2011). Countries in the chaotic regime are capability-poor and their trajectories are dominated by commodity prices, geopolitics, and other exogenous shocks that capability accumulation does not govern.

- **Relevance to project.** Three distinct contributions:
  1. *Fitness as a validated growth predictor.* SPS validates that Fitness (the FC algorithm) is not just a theoretical construct — it predicts GDP growth with accuracy comparable to IMF models, using a single parameter and one global dataset. This validates using firm-level EFC/Fitness as the primary capability measure in the project.
  2. *Laminar/chaotic = heterogeneous treatment effects.* The laminar/chaotic distinction at the country level maps directly onto firm-level heterogeneity in treatment response. Firms with high Fitness (many capabilities, central network position) should show laminar, systematic responses to tariff shocks: they adjust within well-defined capability corridors (within-core diversification). Firms with low Fitness (few capabilities, peripheral network position) show chaotic responses: their adjustment depends on which specific products are hit, whether they can access complementary inputs, and other idiosyncratic factors unrelated to their capability structure. This is the heterogeneous treatment-effect story: central firms reconfigure systematically; peripheral firms cannot.
  3. *The Fitness-GDPpc plane as a firm-level analog.* At the country level, development regimes emerge in the Fitness-GDPpc plane. At the firm level, the analog is the Fitness-revenue plane: firms with high Fitness and moderate revenue should show the most systematic responses to shocks. The event-study heterogeneity analysis (by pre-shock EFC quantile) directly tests whether firm-level laminar/chaotic dynamics exist.

---

### Cross-paper synthesis (§2b)

**1. FC algorithm is the correct operationalization of the Leontief complementarity.** Cristelli 2013 shows that the non-linear harmonic-mean complexity formula is the mathematically necessary consequence of the triangular structure of M_cp and the Leontief complementarity assumption: product complexity is bounded by the *minimum* fitness among exporters. Any linear measure (including MR) violates this because it allows high-fitness exporters to compensate for low-fitness ones — as if a product could be "partially" produced in the absence of one required capability. The FC algorithm, by using the harmonic mean, implements the Leontief condition formally: zero fitness contribution from one exporter collapses the complexity of the product toward zero.

**2. Predictability is the dynamic consequence of the quiescence trap.** The static quiescence trap (Hausmann-Hidalgo 2011) predicts that countries with few capabilities get near-zero return from any new capability. The dynamic consequence (Cristelli 2017) is that these countries' trajectories are chaotic: their future growth depends on which random capability they acquire next (if any), on commodity prices, on political stability — factors that are not deterministic from their current position in the Fitness-GDPpc plane. Countries above the quiescence trap are in the laminar regime because their large capability set constrains the set of feasible trajectories: any shock leads to recombination within the existing capability space, not random drift. The laminar regime = the dynamic signature of escape from the quiescence trap.

**3. From country to firm: what changes and what doesn't.** The FC algorithm is defined on M_cp (countries × products); at the firm level, it becomes M_fp (firms × products). The mathematical structure is identical. What changes: (1) the population is much larger (millions of firms vs. 140 countries), enabling within-country identification; (2) treatment can be exogenous (tariff shocks) rather than endogenous (policy choices); (3) the relevant measure of capability position is the firm's block membership and d_in/d_out outcomes. What doesn't change: the logic of why capability-rich entities have more predictable adjustment paths and why the FC algorithm is the right measure.

**4. SPS parsimony as a template for the project's robustness checks.** SPS achieves IMF-equivalent performance with one parameter and one dataset. This suggests that for our firm-level regressions, Fitness alone (without many controls) should have substantial predictive power for d_in/d_out responses to tariff shocks. The project's robustness should include a "SPS-inspired" test: does a simple non-parametric comparison of firms in the same Fitness-revenue neighborhood before the shock predict their post-shock diversification trajectory, independently of the regression framework?

**5. The natural resources problem and its firm-level analog.** Countries whose GDP growth is driven by commodity prices (Brazil, Russia) show declining Fitness: they are not accumulating capabilities, just extracting rents. The firm-level analog is firms whose export revenue is concentrated in a single commodity-like product (high RCA in one product, low diversification). These firms will show the largest short-run revenue drops from tariff shocks on that product, but their capability structure gives them no basis for systematic within-core reconfiguration. They are in the chaotic regime. This motivates including a natural-resource indicator (or product Herfindahl) as a heterogeneity moderator in the project's regressions.

---

## §2c — ECI optimization and the value-added exports critique (Batch 2c)

*Papers read in full 2026-06-04: Stojkoski & Hidalgo (2025) "Optimizing Economic Complexity" [preprint]; Koch (2021) "Economic Complexity and Growth: Can value-added exports better explain the link?" Economics Letters.*

Batch 2c covers two complementary methodological extensions to the EFC/ECI framework. Hidalgo-Stojkoski (2025) moves beyond description and into optimization: given an ECI target, which activities should an economy enter? Koch (2021) challenges the gross-export foundation of standard ECI/EF: what happens when complexity is measured on value-added rather than gross exports?

---

### Stojkoski & Hidalgo (2025) — "Optimizing Economic Complexity"
*HAL preprint hal-04990629, March 2025*

**Note:** Despite its title, this is NOT an introductory overview of economic complexity. It is a methods paper for industrial policy practitioners that introduces a formal optimization procedure for strategic diversification.

- **Main contribution.** Introduces the ECI Optimization method — a forward-looking, 0-1 integer programming approach for selecting a portfolio of new activities (products/industries) that minimizes the "effort" required to reach a target level of economic complexity. This replaces the prevailing practice of using relatedness-complexity scatter plots (RC diagrams), which the paper demonstrates are heuristic, static, and non-optimal.

- **Why RC diagrams fail.** Three documented limitations: (1) *Relatedness is incomplete*: the probability of entering a product depends on relatedness + specialization levels + trends + multiple relatedness types; relatedness alone (as plotted on the x-axis) misses the full picture. A full entry model with 15 predictors vastly outperforms relatedness alone (Jun et al. 2020). Applied literature still commonly uses relatedness in isolation. (2) *Static complexity*: PCI values change over time. Fully-assembled cars (SITC 7810) fell from rank 17 to 208 in PCI between 1962–2016 as middle-income countries entered. An economy targeting car assembly in 1985 would have overestimated the complexity gain. (3) *No optimal portfolio*: Alshamsi et al. (2018) show optimal diversification requires a mixture of related and unrelated activities whose balance varies with an economy's ECI level (inverted-U); RC diagrams provide no principled way to construct this portfolio.

- **The ECI Optimization method.** Three components:
  1. *Steppingstone model*: A linear regression predicts future log(1+RCA) of each activity as a function of: log RCA at the steppingstone year t+τ, log RCA at the start year t, relatedness ω_cp(t), and relative relatedness ω̃_cp(t). Separate models for entry (RCA<1→≥1) and exit (RCA≥1→<1). Average R² ≈ 0.46–0.49 (entry models). The model is stable across starting years; coefficients depend more on steppingstone duration τ than on starting year.
  2. *Effort estimation*: W_cp = additional RCA at time t+τ that the model predicts is needed for the economy to achieve specialization (RCA≥1) by the target year t+Δt. W_cp is the "cost" of entering activity p for economy c.
  3. *0-1 integer program*: Minimize Σ W_cp·M*_cp (total effort at steppingstone) subject to: average PCI of selected new activities ≥ ECI*. M*_cp ∈ {0,1} is the optimized specialization matrix.
  Future PCI uses the steppingstone model's counterfactual forecast (setting W_cp=0) to capture PCI drift.

- **Properties vs. RC diagram benchmark.** Benchmark: select the N activities with the highest (normalized relatedness × normalized complexity) score.
  - *RCA leverage*: ECI optimization selects products where the economy already has near-comparative advantage (mean RCA ≈ 0.8). RC diagram selects more marginal activities. Interpretation: the optimizer finds the low-hanging fruit that requires minimal incremental investment.
  - *Relatedness balance*: ECI optimization selects relatively more unrelated activities for low-to-medium complexity economies (ECI ≈ 0–0.5), matching the Alshamsi inverted-U. RC diagrams target high relatedness unconditionally.
  - *Activity count*: Both methods suggest similar numbers of activities; ECI optimization requires ~$1B less additional export volume on average.
  - Results replicate on US metropolitan area payroll data (subnational, industry-level), confirming robustness across data granularity and classification type.

- **Growth targeting.** Panel growth regression: Δlog(GDPpc) = a₁·ECI + a₂·log(GDPpc) + a₃·ECI×log(GDPpc) + period FE. ECI coefficient: 0.868*** (standalone) and 1.073*** (with interaction); interaction ECI×income: −1.536*** (complexity raises growth more for lower-income countries). R² grows from 0.09 (Solow baseline only) to 0.19 (ECI only) to 0.23 (ECI + income + interaction). Inverting this equation for a target growth rate yields the ECI* target, which then enters the integer program.

- **Application.** Vietnam (illustration of effort-complexity diagram). Thailand and Mexico (similar ECI ≈ 0.99 but different optimal portfolios): Thailand → Electrical Capacitors (8532), Iron Springs (7320); Mexico → Metal Insulating Fittings (8547), Additive Manufacturing Machines (8485). Despite similar complexity levels, the method tailors recommendations to each economy's existing productive structure.

- **Limitations acknowledged.** Goodhart's Law (optimizing ECI distorts it as an indicator), no general equilibrium effects, simple linear steppingstone model (could use ML), single-dimensional analysis (trade OR payroll, not both).

- **Relevance to project.** Three points:
  1. *ECI-growth link formalized*: The growth regression (ECI coefficient 0.868–1.073, R²=0.23 with interaction) formalizes what Hausmann-Hwang-Rodrik (2007) established descriptively. The interaction term ECI×log(GDPpc) < 0 confirms that complexity raises growth *more* for lower-income economies — at the firm level, this suggests that capability accumulation (measured by EFC Fitness) matters *more* for smaller, less complex Chinese firms than for large, already-complex ones. This strengthens the heterogeneous treatment effect prediction.
  2. *Relatedness as one of many entry predictors*: The paper's critique of RC diagrams — that relatedness alone is a poor guide for entry/exit — directly validates the use of BRIM block membership (rather than simple relatedness) as the outcome in the project. BRIM captures a richer structure than pairwise product proximity, and our d_in/d_out outcomes are richer than "did firm enter product p."
  3. *Steppingstone dynamics*: The distinction between steppingstone timing τ and target horizon Δt (5 vs. 10 years) mirrors the project's event-study horizon choices. The steppingstone model shows that product specialization dynamics have meaningful structure at 5-year intervals — supporting a 5-year pre/post shock window for the event study.

---

### Koch (2021) — "Economic Complexity and Growth: Can value-added exports better explain the link?"
*Economics Letters 198: 109682*

- **Main contribution.** Proposes VXF (Value-added export Fitness) — an FC-algorithm variant applied to domestic value-added exports rather than gross exports. Using World Input-Output Database (WIOD) data for 56 industries and 43 countries (2000–2014), Koch shows that VXF produces substantially different country rankings from EF and ECI, and that VXF better explains GDP per capita growth in panel regressions with fixed effects.

- **Motivation.** Gross exports embed foreign value-added (imported intermediate inputs that are re-exported as part of final goods) and double-counted flows. As GVC integration deepened, the foreign content share of gross exports grew substantially. For countries deeply embedded in GVCs (e.g. China's electronics), gross export complexity reflects partly the capabilities of foreign suppliers, not domestic capabilities. Value-added exports (domestic value-added eventually consumed abroad) strip out foreign content and provide a cleaner signal of domestic productive knowledge.

- **Method.** Weighted adjacency matrix: W_cs = VX_cs / Σ_c VX_cs (country c's share of value-added exports in industry s, normalized across countries for each industry). This is an intensive weighting scheme — each industry's total weight sums to 1. The FC iterative algorithm is then applied with this weighted matrix:
  > F̃_c^(N) = Σ_s W_cs · Q_s^(N−1) [fitness = weighted sum of industry complexities]
  > Q̃_s^(N) = 1 / Σ_c W_cs/F_c^(N−1) [complexity = harmonic mean, weighted]
  Converges to unique fixed point (VXF_c, Q_s). Note: ECI cannot be applied to the weighted matrix (all row sums = 1, so k_s,N = 1 for all iterations — no variation); VXF adapts EF.

- **Rankings divergence (2014).** VXF top: USA (1), CHN (2), DEU (3), GBR (4), JPN (5). EF top: CHN (1), DEU (2), JPN (3), ITA (4), USA (5). ECI top: JPN (1), DEU (2), CHE (3), SGP (4), KOR (5). Major discrepancies: USA ranks 1st in VXF but 5th in EF; Singapore ranks 4th in ECI but absent from VXF top-10 (small domestic value-added base despite high export sophistication). China ranks 1st in EF but 2nd in VXF and much lower in ECI.

- **Growth regressions.** Panel first-differenced model (Δlog GDPpc = α·log GDPpc_t-4 + β₁·ΔlogC + β₂·log C_t-4 + γ'X_t + θ_t + ε, with X = population growth, capital growth, human capital). Three complexity metrics compared:
  - **Column (1) VXF**: Δlog(VXF) coeff = 0.270*** (s.e. 0.044); log(VXF)_lag coeff = 0.159*** (s.e. 0.030); R² = 0.690, adj-R² = 0.480.
  - **Column (2) EF**: Δlog(EF) = 0.073 (n.s.); log(EF)_lag = 0.112* (s.e. 0.068); R² = 0.585, adj-R² = 0.304.
  - **Column (3) ECI**: ΔECI = 0.069** (s.e. 0.030); ECI_lag = 0.064** (s.e. 0.031); R² = 0.577, adj-R² = 0.291.
  - Non-dynamic FE (columns 4–6): VXF still significant; EF and ECI lose significance.
  - Robustness with KOF trade openness: results qualitatively unchanged; VXF remains superior.

- **Key finding.** VXF unconditional R² = 0.63 vs ECI = 0.31 vs EF = 0.24 (Figure 1). This is a strong result: the link between complexity growth and GDP growth is twice as tight when complexity is measured on value-added rather than gross exports.

- **Relevance to project.** Three specific implications:
  1. *Gross vs. value-added bias in Chinese firm data*: Our M_ipt uses gross exports from Chinese customs data. China is deeply embedded in GVCs, especially in electronics and machinery — sectors where foreign content of exports is high. Our firm-level EFC Fitness scores will partly reflect the capabilities of foreign suppliers (via imported inputs) rather than pure domestic capabilities. This is a measurement caveat that should be noted in the paper. Robustness: if data on firm-level value-added exports existed (they do not for China's customs data), VXF-type scores would be preferable.
  2. *EF vs. ECI choice*: Koch finds that EF (Fitness, the FC algorithm) outperforms ECI in growth regressions even on gross exports (EF adj-R² = 0.304 vs ECI = 0.291). Combined with Cristelli 2013's formal argument that FC is mathematically correct and MR is not, this confirms the project's use of FC/EF-type Fitness for firm-level EFC scores rather than ECI (Method of Reflections).
  3. *Sample restriction to 40 countries*: Koch's WIOD covers only 40+ relatively high-income countries. The Chinese firm-level analysis covers a single exporting country (China) and its product-destination diversification — the GVC issue is still present but cannot be corrected within the available data.

---

### Cross-paper synthesis (§2c)

**1. Optimization vs. description.** The EFC/ECI literature has moved from *describing* complexity (Hausmann-Hidalgo 2011, Cristelli 2013) to *predicting* growth from complexity (Cristelli 2017) to *optimizing* complexity (Stojkoski-Hidalgo 2025). The project sits between prediction and optimization: we predict how tariff shocks affect firms' capability trajectories (d_in/d_out), which implicitly reveals whether firms are "optimally" diversifying within their capability set. The steppingstone dynamics from Stojkoski-Hidalgo validate that 5-year event-study windows are the right horizon for observing meaningful changes in specialization patterns.

**2. The relatedness critique cuts both ways.** Stojkoski-Hidalgo's finding that relatedness is only one of many entry predictors is a direct validation of BRIM over simpler measures: BRIM community detection recovers a latent block structure that encodes the full co-specialization pattern (not just pairwise proximity), and our d_in/d_out outcomes measure whether firms moved within or across that latent structure — a richer concept than "did the firm increase relatedness."

**3. Gross exports as a GVC-contaminated signal.** Koch's VXF result has a direct implication for our project: Chinese firm-level gross export complexity (EFC Fitness) confounds domestic capabilities with the foreign content of GVCs. For Chinese electronics and machinery firms (major exporters), Fitness scores may overstate domestic capabilities. This is not a fatal flaw (all existing firm-level EFC papers, including De Stefano 2025, use gross exports), but it motivates a robustness check: do results differ across sectors with different GVC intensities (electronics vs. textiles)?

**4. ECI-growth interaction with income level.** Both Stojkoski-Hidalgo (growth regression with ECI×log(GDPpc) < 0) and Koch (VXF better predicts growth in lower-middle vs. high income) confirm that complexity matters *more* at lower income levels. At the firm level: for small/medium-sized peripheral firms (lower EFC), tariff shocks that destroy capabilities should have proportionally *larger* growth effects than for large/central firms. This strengthens the heterogeneous treatment effect hypothesis: the capability-income interaction at the country level maps to a capability-revenue interaction at the firm level.

**5. Confirmed: EF (FC algorithm) > ECI for growth prediction.** Koch's head-to-head comparison (EF adj-R²=0.304 vs ECI=0.291 in growth regressions) adds an empirical dimension to Cristelli 2013's theoretical argument for FC over MR. The project's use of EF-type Fitness for firm-level scores is supported on both theoretical (correct mathematical specification) and empirical (better growth predictor) grounds.

---

## §2d — Product market dynamics, diversification theory and related variety (Batch 2d)

*Papers read in full 2026-06-04: Angelini, Cristelli, Zaccaria & Pietronero (2017) "The complex dynamics of products and its asymptotic properties"; Freire (2019) "Economic diversification: a model of structural economic dynamics and endogenous technological change"; Boschma & Capone (2015) "Institutions and diversification: related versus unrelated diversification in a varieties of capitalism framework"; Frenken, Van Oort & Verburg (2007) "Related variety, unrelated variety and regional economic growth."*

Batch 2d brings together four papers that each tackle the dynamics of diversification from a different angle: product-market dynamics in the Complexity–income plane (Angelini 2017), a simulation model replicating EFC stylized facts (Freire 2019), institutional moderators of relatedness-driven diversification (Boschma-Capone 2015), and the entropy-based decomposition that is the direct conceptual ancestor of d_in/d_out (Frenken 2007).

---

### Angelini, Cristelli, Zaccaria & Pietronero (2017) — "The complex dynamics of products and its asymptotic properties"
*PLoS ONE 12(5): e0177360*

- **Main contribution.** Introduces logPRODY — a log-scale version of PRODY (Hausmann et al. 2007) — as the monetary counterpart to product Complexity (Q from the FC algorithm), and characterizes the joint dynamics of products in the ranked Complexity vs. ranked logPRODY (RCLP) plane. The central finding is that products move toward an *asymptotic zone* in this plane that reflects the characteristic market configuration for a product of a given complexity level.

- **logPRODY definition.** logPRODY_p = Σ_c R̃_cp · log₁₀(Y_c), where R̃_cp = RCA_cp / Σ_c RCA_cp is the RCA-normalized export-value-share weight and Y_c is per-capita GDP. Using logarithms rather than levels (as in the original PRODY) is justified by the four-orders-of-magnitude span of GDPpc across countries; the geometric mean is more appropriate than the arithmetic mean for such a distribution.

- **The RCLP plane and velocity field.** Products are represented by their yearly ranked Complexity r(Q) and ranked logPRODY r(logPRODY) coordinates. The average 1-year displacement vector field v̄ shows that products drift toward a *asymptotic zone* — a line in the plane slightly skewed from the main diagonal (Spearman correlation between r(Q) and r(logPRODY) = 0.72). Products far from the asymptotic zone have high drift velocities back toward it; products on the asymptotic zone diffuse outward randomly in all directions (average velocity near zero), consistent with stationarity. The shape of the velocity field is stable across time intervals (1–10 years) and datasets (BACI HS4 1995–2014; Feenstra SITC 1963–2000).

- **Herfindahl as a potential.** The competition on each product's export market, measured by the Herfindahl index H_p = Σ_c s²_cp (where s_cp = export share of country c in product p), maps onto the RCLP plane as a scalar field. Key finding: the gradient of H acts as a force — v̄ ≈ −k·∇H — so products move toward lower Herfindahl (higher competition). The minima of H per column coincide with the asymptotic zone. The mechanism: producers enter low-competition ("blue ocean") markets, increasing competition, which pulls logPRODY and Complexity toward their asymptotic values. The Herfindahl explains most but not all of the velocity field; residuals in the top-left quadrant (high-GDPpc but mixed-Fitness exporters) are explained by Complexity increases from the exclusion of low-Fitness exporters — the FC Leontief condition operating empirically.

- **Asymptotic market shapes.** At the asymptotic zone, the distribution of comparative advantage across Fitness deciles is characteristic of each Complexity level: high-Complexity products have RCA strongly peaked on the highest-Fitness countries; low-Complexity products have a flat or mildly peaked distribution across all countries. This is the empirical signature of the Leontief complementarity: any single low-Fitness exporter of a product suppresses its Complexity score, so high-Complexity products can only persist in markets where low-Fitness countries have been excluded.

- **Relevance to project.** Three specific points: (1) logPRODY is used in the project's regressions as a product-sophistication control. This paper shows logPRODY is well-defined, non-redundant with Complexity (correlation 0.72, not 1.0), and has economically meaningful dynamics — transient deviations from the asymptotic zone revert predictably. (2) When a tariff shock hits product p for Chinese firm i, the product's export market is disrupted: new entrants from non-shocked countries may fill the gap, increasing competition and pulling logPRODY toward a new asymptotic value. This is a confound to control for — we need logPRODY to be a predetermined (pre-shock) control. (3) The long-run stationarity of the RCLP plane implies that product Complexity and logPRODY are mean-reverting at medium horizons — tariff shocks produce temporary dislocations that equilibrate over 5–10 years. Our event study must be long enough (5+ year horizon) to capture the adjustment dynamics.

---

### Freire (2019) — "Economic diversification: a model of structural economic dynamics and endogenous technological change"
*Structural Change and Economic Dynamics 49: 13–28*

- **Main contribution.** Provides a formal simulation model that derives the two main EFC stylized facts — (1) diversification is positively associated with total GDP; (2) diversification is negatively associated with average ubiquity of exports — as *emergent properties* of a multi-country, multi-product economy with endogenous product innovation, emulation, and structural change. The model bridges the EFC empirical literature with Pasinetti's structural economic dynamics theory.

- **Model structure.** Short-run: R countries, m products. Prices = labour costs × markups. Quantities determined by linear programming (Duchin 2005 World Trade Model) that minimizes total expenditure subject to labour availability, preventing full specialization. Wages are endogenous (reflect average productivity). Long-run: R&D sector funded by markups engages in four types of technological change: (i) process innovation (Poisson process, reduces labour coefficient); (ii) product innovation (Poisson process, creates new product via combination of two existing technologies — adjacent possible, Kauffman 2008); (iii) process emulation; (iv) product emulation. Consumption follows generalized Engel's law (hierarchical preferences, saturation). R&D effort allocation endogenous: when employment is high, R&D shifts toward process innovation; when employment is low, toward product innovation (new demand creation).

- **Key results (100 Monte Carlo runs, 30 countries, 10 initial products, 100 periods).**
  - Slope of log(diversification) × log(GDP): mean = +4.61, std = 0.46, R² ≈ 0.94 — replicates stylized fact 1.
  - Slope of log(diversification) × log(average ubiquity): mean = −0.85, std = 0.03, R² ≈ 1 — replicates stylized fact 2.
  - Additional emerging regularities: diversification positively associated with employment, consumption per capita; negatively associated with average labour coefficient (diversified countries achieve higher average productivity via process innovation).
  - Sensitivity: robust to variation in innovation arrival rates and emulation rates. The stylized facts are qualitative properties of the model, not calibration artifacts.

- **Mechanism.** The model clarifies the causal chain: more diversified countries have higher employment (more products = more production sectors = higher employment share) → more R&D devoted to process innovation (endogenous allocation) → lower labour coefficients → lower prices → competitive advantage → further diversification opportunities. This is a Kaldor-Verdoorn type virtuous circle. The adjacent possible constraint enforces path dependency: new products can only be created by combining existing technologies, so the set of feasible new products is bounded by the current portfolio.

- **Relevance to project.** The adjacent possible mechanism is the simulation-model analog of BRIM block-consistency: within-block diversification (d_in) involves entry into products sharing a technology base (adjacent in the capability graph); out-of-block diversification (d_out) requires crossing a larger technological gap (non-adjacent). The model predicts that d_in should be the natural default (combinatorially more likely from within the existing portfolio), while d_out requires an unusual capability acquisition. This justifies the project's prior that the baseline response to a tariff shock should be d_in dominance — firms reinforce their existing core — with d_out representing a strategic reorientation under special conditions (e.g. total destruction of the core product set, large shock, institutional support for unrelated diversification).

---

### Boschma & Capone (2015) — "Institutions and diversification: related versus unrelated diversification in a varieties of capitalism framework"
*Research Policy 44: 1902–1914*

- **Main contribution.** Integrates the varieties of capitalism (VoC) framework (Hall & Soskice 2001) with the related diversification literature (Hidalgo et al. 2007). Tests whether national institutions — specifically the LME/CME distinction and continuous institutional indicators — moderate the effect of product proximity (density) on diversification into new products. Data: BACI HS 4-digit (1241 products), 23 developed countries, 1995–2010, 5-year horizon.

- **Key formal objects.** Product *proximity*: φ_{ij} = min(P(RCA_i|RCA_j), P(RCA_j|RCA_i)) — symmetric, conservative conditional probability of co-specialization. *Density*: d_{i,c,t} = Σ_j x_{j,c,t}·φ_{ij} / Σ_j φ_{ij} — share of product i's neighborhood currently produced by country c. High density = product i is close to country c's existing portfolio. Regression: LPM with country-year and product-year FE, country-clustered SE, 5-year lags.

- **Key results.**
  1. *Density is the dominant driver of product entry*: β(density on new products) ≈ 0.136–0.157*** across all specifications. Countries diversify overwhelmingly into products close to their current portfolio. R² ≈ 0.62–0.69.
  2. *VoC categorical dummies (Table 1) are not significant*: LME/CME/MME interaction with density never reaches 5% significance. Coarse categorical classification is too crude.
  3. *Continuous institutional indicators (Table 3) are significant*: Labor Relations Index (strategic coordination) × density on new = 0.039* (26% larger density effect); Corporate Governance Index × density on new = 0.038** (16% larger). Combined PCA index also significant.
  4. *Robustness (Table 4)*: Product market regulation (PMR) × density = positive and significant; M&A activity × density = negative and significant; firm cooperation (FCO) × density = positive and significant. Vocational training negative in one spec, not robust.
  5. *Interpretation*: CME-type institutions (non-market coordination in labor, finance, product markets, inter-firm relations) amplify the density effect by 16–32%. Firms in CME contexts have specialized assets, long-term relationships, and industry-specific skills that make related diversification more efficient. LME-type institutions (market coordination: fluid labor, M&A access, generic assets) reduce the density effect, enabling larger "jumps" in product space.

- **Relevance to project.** Three points: (1) *Density is the right concept of relatedness for our outcomes*: the d_in outcome directly measures whether firms enter products within their existing capability block (high density in BRIM terms). The paper establishes density as the dominant predictor of product entry, not raw sector classification. (2) *Institutional moderators at the firm level*: Chinese SOEs are more CME-like (long-term relationships, patient capital, specialized labor); private firms are more LME-like (market coordination, high turnover). This predicts that SOEs respond to tariff shocks with more relatedness-constrained diversification (d_in > d_out) relative to private firms. An SOE vs. private firm heterogeneity test is motivated by this literature. (3) *The density measure* is the precursor of our block-consistent diversification: proximity φ_ij in the product space is the non-parametric counterpart of BRIM community membership. Our d_in = products with high φ to existing portfolio (within-block); d_out = products with low φ (cross-block). The Boschma-Capone finding that density explains 60–70% of entry variance validates the fundamental claim that capability relatedness dominates product diversification trajectories.

---

### Frenken, Van Oort & Verburg (2007) — "Related variety, unrelated variety and regional economic growth"
*Regional Studies 41(5): 685–697*

- **Main contribution.** Introduces the entropy-based decomposition of sectoral diversity into *related variety* (RV, within-sector variety at fine-grained classification) and *unrelated variety* (UV, between-sector variety at coarse classification), and shows they have opposite effects on regional economic outcomes. This is the conceptual and methodological precursor of d_in/d_out.

- **Definitions (entropy decomposition).**
  - Let two-digit sector g have employment share P_g; sub-sectors i within g have share p_i.
  - Unrelated variety (UV) = Σ_g P_g log₂(1/P_g) — entropy across 2-digit sectors.
  - Related variety (RV) = Σ_g P_g · H_g, where H_g = Σ_{i∈g} (p_i/P_g) log₂(P_g/p_i) — weighted sum of entropy within 2-digit sectors.
  - By Theil (1972) decomposition: 5-digit entropy = UV + RV. The two components are orthogonal (correlation = −0.046 in Dutch data).

- **Hypotheses and results (Dutch NUTS 3 regions, n=40, 1996–2002, OLS with controls).**
  - H1: Related variety (Jacobs externalities) → employment growth: **CONFIRMED**. β(RV) ≈ 0.638*** (standardized); robust across all specifications and time windows. Population density not significant — it is the *related variety within cities* that drives job creation, not urban density per se.
  - H2: Localization economies (Los-index) → productivity growth: **NOT confirmed**. Los-index never significant. Productivity is explained by investment, R&D, and capital-labour ratio growth — the standard neoclassical suspects.
  - H3: Unrelated variety → lower unemployment growth: **CONFIRMED** in 3/5 specifications. β(UV) ≈ −0.395** (standardized). Unrelated sectors act as a portfolio: demand shocks in sector g are not correlated with shocks in unrelated sectors, so regions with higher UV absorb unemployment better.
  - Additional finding: related variety → productivity growth is *negative* (β ≈ −0.273*). This is consistent with Pasinetti's theory: related variety drives new product introduction and employment creation, not within-sector efficiency gains. Productivity requires process innovation (R&D, capital deepening), not cross-sector spillovers.

- **Mechanisms and theory.** Related variety generates Jacobs externalities through within-sector spillovers: knowledge from sub-sector i spills to sub-sector j within the same 2-digit class because they share inputs, workers, and technologies. This enables product innovation and employment creation. Unrelated variety acts as a portfolio (Markowitz 1952 analog at the regional level): sectors with uncorrelated demand shocks insulate the region against asymmetric shocks, preventing unemployment. The two mechanisms are separate and empirically distinguishable because UV and RV are orthogonal.

- **Relevance to project.** This paper is the direct conceptual precursor of d_in/d_out in our framework. The mapping is:
  - RV = firm-level d_in: diversification *within* the same capability block is related variety — the new products share capabilities with the existing core, enabling spillovers and learning.
  - UV = firm-level d_out: diversification *across* different capability blocks is unrelated variety — the new products draw on different capabilities, providing portfolio protection against demand shocks.
  - The Frenken et al. predictions translate to firm-level hypotheses: firms that increase d_in (related variety) should experience employment/revenue growth via capability spillovers; firms that increase d_out (unrelated variety) should be better insulated against future tariff shocks (portfolio effect). This is the dual interpretation of our dependent variables: d_in captures capability deepening; d_out captures portfolio diversification.
  - The key finding that related variety drives employment but *not* productivity is important: our outcome d_in should predict export growth (revenue/product scope) better than firm-level TFP — consistent with Grazzi (2012, §4g) who found that exporter status predicts productivity but not profitability.

---

### Cross-paper synthesis (§2d)

**1. logPRODY and Complexity as a dynamic equilibrium system.** Angelini et al. (2017) establish that the Complexity-logPRODY plane has an attractor: products drift toward their asymptotic market configuration driven by competition (Herfindahl dynamics). This means the EXPY and EFC scores we use as controls in our regressions are not arbitrary snapshots — they reflect meaningful equilibrium positions in a well-characterized dynamical system. Deviations from asymptotic values (caused e.g. by a tariff shock) are transient; the long-run dynamics pull products back.

**2. Freire's model grounds the adjacent-possible mechanism.** The simulation model establishes that the triangular M_cp structure and the diversification-ubiquity stylized facts emerge from a combination of path-dependent innovation (adjacent possible), markup-driven competitive dynamics, and Engel's law consumption saturation. At the firm level: the adjacent possible constraint = block-consistent diversification — firms can only realistically enter products reachable in one or two capability steps from their current portfolio. This formalizes why d_in is the default diversification direction and d_out requires special conditions.

**3. Boschma-Capone: density dominates, institutions moderate.** Product density (proximity-weighted neighborhood of existing specializations) explains 60–70% of the variance in product entry across countries and time. Relatedness is not just one of many factors; it is *the* primary predictor of diversification. Institutional frameworks modulate how tightly relatedness constrains diversification: CME institutions amplify relatedness (d_in favored); LME institutions allow wider jumps (d_out possible). At the firm level, Chinese SOEs may behave more CME-like (relatedness-constrained = d_in dominant) while private firms behave more LME-like (d_out feasible). This is an empirically testable heterogeneity.

**4. Frenken et al.: related vs. unrelated variety is the founding decomposition for d_in/d_out.** The entropy decomposition (RV within 2-digit sectors / UV across 2-digit sectors) is the methodological ancestor of BRIM block-consistent diversification. Key empirical regularities from Frenken that should hold at the firm level: (i) d_in (RV) → export/employment growth; (ii) d_out (UV) → shock insulation; (iii) neither necessarily drives productivity/TFP growth, which requires process innovation (R&D and capital deepening). Our empirical design should test hypotheses (i) and (ii) explicitly.

**5. What is new in our project.** These four papers all operate at the country or regional level. Our contribution is to take the same conceptual framework — related vs. unrelated diversification, density as a predictor of entry, institutional moderators, product-space dynamics — to the *firm* level with a *causal identification strategy* (Bartik tariff shock). The firm-level decomposition into d_in/d_out via BRIM community detection is more precise than entropy-based measures because it recovers the latent capability structure of the network rather than relying on administrative sector classifications. This is the methodological advance over Frenken's entropy approach that De Stefano (2025, Batch 1) established, and that the project exploits for causal inference.

---

## §2e — Nestedness: observation, emergence, and implications (Batch 2e)

*Paper read in full 2026-06-04: Mariani, Ren, Bascompte & Tessone (2019) "Nestedness in complex networks: observation, emergence, and implications." arXiv:1905.07593 (preprint, 140pp).*

This is the central methods reference for nestedness analysis — a comprehensive interdisciplinary review covering metrics, null models, emergence mechanisms, systemic implications, and mesoscopic nestedness detection. For the project, the paper provides: (1) the formal definitions of NODF and the maximum-entropy null model that validate our bipartite network construction; (2) the mathematical grounding for the relationship between nestedness, modularity, and in-block nestedness that underpins the BRIM community detection in De Stefano (2025); and (3) the formal quality function I for detecting in-block nested structures — the structural pattern that our d_in/d_out outcomes are designed to measure.

---

### Mariani, Ren, Bascompte & Tessone (2019) — "Nestedness in complex networks: observation, emergence, and implications"
*arXiv:1905.07593 (Elsevier preprint, 140pp)*

- **Main contribution.** First comprehensive unified review of nestedness spanning both bipartite networks (ecological mutualistic systems, country-product trade) and unipartite networks (interbank, contractor, social). The review covers three pillars: (1) metrics and null models for observing nestedness; (2) theoretical mechanisms explaining its emergence; (3) implications for systemic stability and robustness. Section 7, on nestedness at the mesoscopic scale (including in-block nestedness), is directly relevant to the project.

---

#### Part I: Observing nestedness — metrics and null models

**Definition.** A perfectly nested network satisfies: for any two nodes i and j with k_i < k_j, the neighborhood of i is a subset of the neighborhood of j. This is equivalent to the network's adjacency matrix (sorted by degree) having a triangular shape — a monotonic separatrix above which all entries are 1 and below which all are 0. In bipartite networks (countries × products), the comparison is restricted to nodes of the same class. Perfectly nested networks are equivalent to threshold graphs (Chvátal-Hammer 1977) and nested split graphs (Földes-Hammer 1977): a node has a link with another if and only if the sum of their fitness exceeds a threshold.

**Nestedness metrics.** Four families:

1. *Gap-counting*: N₀ (unexpected absences — times a node is not a neighbor of a higher-degree node that could be in its neighborhood), N₁ (unexpected presences), and D (number of departures). Lower values = more nested.

2. *Distance-based*: Nestedness temperature T (Atmar-Patterson 1993) — the minimum matrix temperature obtained by optimally reshuffling the adjacency matrix. Lower T = more nested. The algorithm for minimizing T is BINMATNEST. Key connection: the Fitness-Complexity (FC) algorithm sorts the adjacency matrix in a way that approximates, and often outperforms, BINMATNEST in maximizing nestedness (Section 3.3.2 — the FC algorithm is a nestedness maximizer).

3. *Overlap-based*: **NODF** (Nestedness based on Overlap and Decreasing Fill, Almeida-Neto et al. 2008) — the central metric. For row nodes i and j with k_i > k_j, the pairwise row-NODF is N^R_{ij} = O_{ij}/k_j (where O_{ij} = Σ_α A_{iα}A_{jα} is the overlap = number of shared neighbors), else 0. The column-NODF N^C_{αβ} is defined analogously. Total NODF = (Σ_{pairs ij} N^R_{ij} + Σ_{pairs αβ} N^C_{αβ}) / (N(N-1)/2 + M(M-1)/2). NODF = 0 when no pair is nested; NODF = 100 when perfectly nested. S-NODF (stable-NODF by Bastolla 2009) is a regularized version that avoids penalizing pairs of equal degree and is more robust to small perturbations.

4. *Eigenvalue-based*: Spectral radius ρ(A) (Staniczenko 2011) — the largest eigenvalue of the adjacency matrix. Rigorous bounds on ρ from graph theory make it analytically tractable.

**Key recommendation from the review.** NODF combined with the maximum-entropy null model (see below) is the best-established metric combination for bipartite networks (Section 3.4). BINMATNEST is not recommended as a standalone nestedness quantifier.

**Null models.** Nine basic classes formed by combining row/column degrees that are equiprobable (E), proportional (P), or fixed (F): EE, EP, EF, PE, PP, PF, FE, FP, FF. The FF model (exactly preserves both row and column degree sequences) is the most conservative; the EE model (only preserves total link density) is the least conservative. Key trade-off: FF is too restrictive (randomized networks are almost identical to the empirical one, leaving no room to reject nestedness as significant); EE is too lax (almost never rejects nestedness as non-significant). The PP model (Bascompte 2003, proportional to degrees but stochastic) and the BiCM-equivalent maximum-entropy model are the recommended compromises.

**Maximum-entropy approach (Squartini-Garlaschelli 2012).** Constructs a probability distribution over binary networks that has maximum entropy subject to the constraint that the expected degrees match the observed ones. Formally, for each link (i,α), the probability of the link exists is p_{iα} = x_i y_α / (1 + x_i y_α) where x_i and y_α are Lagrange multipliers fixed by the degree constraints Σ_α p_{iα} = k_i and Σ_i p_{iα} = k_α. This yields an analytic expected value <NODF> and standard deviation σ(NODF), enabling z-score calculation without Monte Carlo. The resulting null model is the BiRG (bipartite random graph) or BiCM (bipartite configuration model).

**Critical finding on the country-product network.** Saracco et al. (2015, 2017 — in our Batch 3c papers) showed that when using the BiCM null model, the z-score of the NODF of the bipartite country-product network is NOT significantly greater than expected from the degree sequence alone — the global nestedness of the network is largely explained by the heterogeneous degree distribution. However, the *country-level contribution* to NODF (row-NODF, measuring nestedness across country pairs) remains statistically significant for 1995–2010. This means: the global triangular shape is partly a statistical artefact of degree heterogeneity, but the cross-country nested ordering has genuine signal.

---

#### Part II: Nestedness vs. modularity

**Modularity (Barber 2007 for bipartite).** Q = (1/E) Σ_{i,α} (A_{iα} − k_i k_α / E) δ(Ξ_i, Ξ_α), where Ξ is a partition of nodes into blocks. Modularity measures how much the within-block link density exceeds what would be expected under the configuration model. BRIM (Barber 2007) maximizes Q for bipartite networks through alternating row/column label reassignment.

**Nestedness-modularity relationship.** At low network density (few links relative to nodes): nestedness and modularity are *positively* correlated — networks can be simultaneously nested and modular (Fortuna et al. 2010). At high density: negatively correlated. For the bipartite firm-product network (sparse, ~8–20% fill as in Hausmann-Hidalgo 2011): the positive correlation regime applies, meaning the BRIM-detected blocks are likely to also exhibit internal nested structure. This is the structural justification for d_in/d_out.

**Modular-to-nested transition.** Borge-Holthoefer et al. (2017) found that a Twitter user-meme network transitions abruptly from modular to nested topology when collective attention narrows from multiple sub-topics to a single topic. This suggests nestedness and modularity are not mutually exclusive but represent different organizational regimes. A system can move between them.

**Critical problem.** Modularity optimization (including BRIM) tends to cluster the high-degree nodes together in sparse networks, producing incorrect community detection when the true underlying structure is in-block nested rather than purely modular. Specifically: in a network with planted in-block nested structure (each block is internally nested, but nodes of the same block are also somewhat heterogeneously connected), BRIM can fail to correctly recover the planted blocks even when inter-block links are zero (Section 7.3.1, Solé-Ribalta et al. 2018).

---

#### Part III: Economic applications (Section 4.3)

**Firm survival and nestedness.** Saavedra et al. (2011) analyzed a 15-year manufacturer-contractor bipartite network. Individual nestedness contribution C_i = (N − μ_i(N)) / σ_i(N) (deviation of nestedness when node i's links are randomized). Finding: strongest contributors to nestedness are the least likely to survive. Interpretation: the most "generalist" firms that connect the network's nested structure are also the most exposed to competitive shocks (because their survival depends on many links being maintained simultaneously).

**Link prediction.** Bustos et al. (2012) showed that the bipartite country-product network's nested structure predicts future link appearance and disappearance: appearances tend to be close to the "diversity-ubiquity line" (the ideal nested frontier), disappearances tend to fall far outside it. AUC for disappearance prediction = 0.81; for appearances = 0.62. The nested structure is highly predictive of future diversification paths.

**Growth prediction.** The Fitness-Complexity algorithm (Cristelli 2013) sorts the adjacency matrix to maximize nestedness, and countries' fitness scores derived from this ranking predict future GDP growth (Section 4.3.3, connecting to Cristelli 2017 from §2b). The fitness-GDPpc plane exhibits laminar (predictable) dynamics for high-fitness countries.

**Hidden capabilities model.** Section 4.3.4 formalizes the Hausmann-Hidalgo (2011, §2a) capabilities model: A_{iα} = 1 iff Σ_κ C_{iκ} P_{ακ} = Σ_κ P_{ακ} (firm has ALL capabilities required by product). The binomial model (Hausmann-Hidalgo) assigns each capability with independent probability r and q; the uniform model (Bustos et al.) allows heterogeneous capability endowments (uniform draws), producing more realistic nestedness levels.

---

#### Part IV: In-block nestedness — Section 7.3 (KEY SECTION)

**Definition.** An *in-block nested* (or "nested-modular" or "combined") structure is a network that (1) can be partitioned into blocks (communities) and (2) each block exhibits an internally nested structure. This is the structural pattern that the firm-product bipartite network in the project implements: BRIM partitions firms and products into blocks (capability communities), and within each block, the sub-network is nested (the most capable firms in the block export all products of the block; less capable firms export a subset).

**Why modularity optimization alone fails.** Solé-Ribalta et al. (2018) showed that BRIM and other modularity-maximization algorithms fail to correctly recover planted in-block nested blocks when:
- The within-block structure is sparse and nested (low p = high nestedness parameter)
- Inter-block links are few but non-zero
In this regime, BRIM tends to merge blocks that should be separate (clustering the high-degree hub nodes together across blocks). The failure is systematic: modularity maximization is "blind" to the internal nested organization of blocks.

**The in-block nestedness quality function I.** Solé-Ribalta et al. (2018) introduce I for bipartite networks:
> I = (2/(N+M)) × [Σ_{ij same block} (O_{ij} − ⟨O_{ij}⟩) Θ(k_i − k_j) / (k_j (|Ξ_i| − 1)) + Σ_{αβ same block} (O_{αβ} − ⟨O_{αβ}⟩) Θ(k_α − k_β) / (k_β (|Ξ_α| − 1))]

This is a normalized NODF function restricted to *within-block* pairs, compared against the expected overlap ⟨O_{ij}⟩ under the configuration model (analogous to how Barber's modularity Q compares within-block link density to the configuration-model expectation). I combines partition discovery (which block each node belongs to) and nestedness assessment (how nested is the within-block structure) in a single objective. Maximizing I jointly finds the partition and certifies that each block is internally nested.

**Performance.** I-optimization outperforms modularity-based approaches across a broad range of parameter values (low p and low µ). In real data across 334 networks, I, Q, and NODF are approximately independent — knowing one tells you little about the other two. This justifies using all three as separate structural dimensions.

**Resolution limit.** Modularity (Q) suffers from a resolution limit: cannot detect modules smaller than a scale determined by network properties (Fortunato-Barthélemy 2007). Solé-Ribalta et al. found numerically that I does *not* exhibit an analogous resolution limit — small blocks with internally nested structure can be detected. This is important for the project because Chinese firm-product networks may have many small blocks corresponding to niche capability clusters.

---

### Cross-paper synthesis (§2e)

**1. BRIM detects modularity, not in-block nestedness.** The key methodological insight from Mariani 2019 is that BRIM (used in De Stefano 2025 and by extension in the project) maximizes Barber's modularity Q — it detects blocks with high internal link density relative to the configuration model. It does NOT guarantee that the detected blocks are internally nested. The literature (Solé-Ribalta 2018) shows these are distinct properties. The correct interpretation of BRIM blocks is: "capability clusters where within-cluster firm-product links are denser than expected by chance" — not "capability clusters where within-cluster firm-product links form a nested hierarchy." The blocks are likely internally nested (given the positive nestedness-modularity correlation at low density), but this should be verified with the I quality function as a robustness check.

**2. The triangular M_ipt is confirmed but partially explained by degree heterogeneity.** The finding that global nestedness of the bipartite network is largely explained by the degree sequence (Saracco et al.) means our firm-level M_ipt's triangular shape is expected from the heterogeneous distribution of firm diversification (some firms export hundreds of products, most export few). The genuine signal is in the *cross-firm nested ordering* (row-NODF): firms that export fewer products tend to export a subset of what the most-diversified firms export. This validates the capability hierarchy interpretation.

**3. The FC algorithm as a nestedness maximizer.** Mariani 2019 makes explicit (Section 3.3.2, citing Cristelli 2013) that the FC algorithm sorts the bipartite adjacency matrix in a way that maximizes nestedness and often outperforms BINMATNEST. This means EFC Fitness scores do double duty: they measure country/firm competitiveness AND order the adjacency matrix to reveal its nested architecture. For the project: high-Fitness firms are at the "top" of the nested hierarchy; low-Fitness firms are at the "bottom."

**4. The maximum-entropy null model (BiCM) is the correct baseline.** For any nestedness statistic computed from M_ipt, the z-score should be based on the BiCM (Squartini-Garlaschelli 2012). Raw NODF scores are not interpretable without controlling for degree heterogeneity. The project's data construction should include a BiCM-based validation that the firm-product network is significantly nested beyond what would be expected from the observed degree sequence.

**5. The d_in/d_out decomposition is formally grounded in in-block nestedness.** The project's d_in = Σ_{p: b(i)=b(p)} M_{ipt} counts products that firm i enters that are within the same BRIM block. d_out = Σ_{p: b(i)≠b(p)} M_{ipt} counts cross-block entries. In the language of Mariani 2019: d_in measures firms' progress up the within-block nested hierarchy (adding products within their existing capability community); d_out measures firms' jumps across blocks (entering a different capability community). The in-block nestedness function I (Solé-Ribalta 2018, in our Batch 3b) is the formal quality criterion that validates whether the BRIM-detected blocks have the internally nested structure that makes d_in interpretable as a within-hierarchy movement. This paper (Mariani 2019) provides the review-level context for why this structure matters and how to measure it.

**6. Firm survival and nestedness.** The Saavedra et al. finding — that the strongest contributors to nestedness are also the most vulnerable to extinction — has a direct firm-level analog: firms with the highest individual nestedness contribution (generalists that hold the bipartite structure together) are most exposed to tariff shocks. These are the high-Fitness, high-diversification firms at the "top" of the nested hierarchy. A tariff shock hitting their core products destabilizes the entire capability architecture around them. This motivates including a "nestedness contribution" term as a heterogeneity moderator in the project's regressions.

---

## §3a — Community detection and nestedness: founding algorithms (Batch 3a)

*Papers read in full 2026-06-04: Barber (2007) "Modularity and community detection in bipartite networks"; Newman (2006) "Modularity and community structure in networks"; Blondel, Guillaume, Lambiotte & Lefebvre (2008) "Fast unfolding of communities in large networks"; Duch & Arenas (2005) "Community detection in complex networks using extremal optimization"; Almeida-Neto, Guimarães, Guimarães Jr, Loyola & Ulrich (2008) "A consistent metric for nestedness analysis in ecological systems."*

Batch 3a covers the foundational algorithmic papers for community detection and nestedness measurement that underpin the network methods used throughout EFC and in the project. BRIM (Barber 2007) is the algorithm De Stefano (2025) uses to detect capability blocks in the bipartite firm-product network. Newman (2006) is the unipartite precursor on which BRIM is modeled. Blondel et al. (2008) is the Louvain algorithm — the dominant modern alternative for large networks. Duch & Arenas (2005) is the extremal optimization benchmark used in the Newman (2006) comparison. Almeida-Neto et al. (2008) is the original NODF paper — the central nestedness metric for bipartite networks.

---

### Barber (2007) — "Modularity and community detection in bipartite networks"
*Physical Review E 76: 066102*

- **Main contribution.** Defines a null model appropriate for bipartite networks and uses it to construct Barber's bipartite modularity Q and the BRIM algorithm for community detection. This is the direct mathematical foundation of the community detection step in De Stefano (2025) and in the project's construction of d_in/d_out.

- **Bipartite null model.** The key departure from Newman-Girvan unipartite modularity is that the null model must assign zero probability to edges between nodes of the same colour (firms with firms, products with products). For a bipartite network with p row-nodes (firms) and q column-nodes (products), m total edges, row-degree k_i and column-degree d_α, the null model probability of edge (i,α) is P̃_{iα} = k_i d_α / m. This is the natural bipartite analog of the configuration model: probability proportional to degree products, normalized to preserve expected degrees on each side.

- **Barber's bipartite modularity.** With biadjacency matrix Ã (p×q, entries = 1 if firm i exports product α with RCA>1) and P̃ as above:
  > Q = (1/m) Σ_{i,α} (Ã_{iα} − k_i d_α / m) δ(Ξ_i, Ξ_α)
  where Ξ_i is the block assignment of firm i and Ξ_α of product α. δ(Ξ_i, Ξ_α) = 1 iff i and α are in the same block. Q > 0 means within-block link density exceeds what the null model predicts from the degree sequence alone. In matrix form: Q = (1/m) Tr(R^T B̃ T) where R (p×c) and T (q×c) are binary assignment matrices for rows and columns respectively, and B̃ = Ã − P̃.

- **Spectral structure.** The full bipartite modularity matrix B is block off-diagonal:
  > B = [[0, B̃], [B̃^T, 0]]
  This means eigenvalues of B come in ±λ pairs: for every eigenvector (u, v)^T with eigenvalue λ, there is (u, −v)^T with eigenvalue −λ. Only eigenvectors with positive eigenvalues (σ_i > 0, the singular values of B̃) contribute positively to Q. Therefore, community detection reduces to the SVD of B̃: the leading left and right singular vectors (u₁, v₁) of B̃ give the optimal bipartition (sign of u₁ assigns firms to blocks, sign of v₁ assigns products to the same blocks).

- **BRIM algorithm.** Bipartite Recursively Induced Modules. Iterative procedure exploiting the bipartite structure:
  1. Fix product block assignments T. Then maximize Q over row (firm) assignments R: each firm i is assigned to the block k* that maximizes row k of the aggregated matrix T̃ = B̃T.
  2. Fix firm block assignments R. Then maximize Q over column (product) assignments T: each product α is assigned to block k* maximizing row α of R̃ = B̃^T R.
  3. Repeat 1–2 until Q no longer increases.
  Each step guarantees Q never decreases → always converges to a local maximum. The number of modules c is selected adaptively via bisection search: start with c=1 (Q=0), double c while Q keeps increasing, then bisect to find c_max bracketed by inferior solutions at c_max±1. This adds only O(log n) overhead.

- **Key properties.** (1) Joint assignment: both firms and products are simultaneously assigned to the same blocks (unlike projecting onto one side). (2) Informed by bipartite structure: the SVD of B̃ is the natural decomposition for asymmetric matrices, recovering more information than the spectral decomposition of the symmetric unipartite B. (3) Resolution limit applies: as in unipartite modularity, modules below a scale depending on m cannot be reliably detected.

- **Empirical validation.** Southern women network (18 women × 14 events): Q=0.345 with 4 modules, outperforming prior studies' 2-module solutions (Q≈0.321). Scotland corporate interlock (131 directors × 86 firms): ~20 communities at best Q=0.566, significantly better than naive initialization.

- **Relevance to project.** BRIM is exactly what De Stefano (2025) applies to the bipartite firm × product network M_ipt. The block partition Ξ = {Ξ_i, Ξ_α} identifies capability communities: firms and products assigned to the same block share a latent capability bundle. d_in = products firm i enters in year t+1 that belong to block b(i); d_out = products that cross into a different block b ≠ b(i). The mathematical guarantee of convergence to a local Q maximum means BRIM will always find a valid partition — though it may not find the global optimum. Multiple random initializations are needed in practice.

---

### Newman (2006) — "Modularity and community structure in networks"
*PNAS 103(23): 8577–8582*

- **Main contribution.** Derives the unipartite modularity matrix B and introduces a spectral method for community detection that is faster and more accurate than prior algorithms. This is the direct precursor that Barber (2007) extends to bipartite networks.

- **Unipartite modularity matrix.** For a network with adjacency matrix A, degree sequence k, and total edges m:
  > B_ij = A_ij − k_i k_j / 2m
  Q = (1/4m) s^T B s, where s_i = +1 or −1 indicates group membership for two-group split.
  Key property: rows and columns of B sum to zero → always has eigenvector (1,1,…) with eigenvalue 0 (trivial partition) → algorithm cannot put all vertices in one group as long as any positive eigenvalue exists.

- **Spectral algorithm.** Leading eigenvector u₁ of B: assign vertex i to group 1 if (u₁)_i > 0, group 2 otherwise. Magnitude of (u₁)_i measures strength of community membership. For multiple communities: recursive bipartition using the generalized B^(g) matrix for subgraph g — which adjusts for edges removed from the full network. Stop when leading eigenvalue of B^(g) ≤ 0 (subgraph is "indivisible" — no positive-modularity division exists).

- **Fine-tuning.** After spectral bipartition, apply a Kernighan-Lin-like vertex-moving heuristic: move vertices one at a time to maximize Q; find the state with highest Q among all intermediate states; repeat. Adds ~few% to Q but is the difference between good and exceptional performance.

- **Performance.** Against GN (Girvan-Newman), CNM (Clauset-Newman-Moore), DA (Duch-Arenas): matches or exceeds DA for large networks (>6% better for largest tested network). O(n² log n) for sparse graphs vs O(n³) for GN and O(n² log² n) for DA.

- **Relevance to project.** Newman (2006) establishes the modularity-eigenvector framework that Barber (2007) generalizes to bipartite networks via SVD. The indivisibility criterion (no positive eigenvalue → no meaningful split) is critical for adaptive BRIM: it tells us when to stop subdividing blocks. The eigenvector magnitudes (strength of community membership) provide a firm-level "coreness" measure within each block — a potential heterogeneity moderator.

---

### Blondel, Guillaume, Lambiotte & Lefebvre (2008) — "Fast unfolding of communities in large networks"
*Journal of Statistical Mechanics P10008* — **Louvain algorithm**

- **Main contribution.** Introduces the Louvain algorithm, the most widely used community detection method. Two-phase iterative approach running in near-linear time, capable of handling networks with hundreds of millions of nodes, and producing a hierarchical (multi-resolution) community structure.

- **Algorithm.** Starting state: each node in its own community.
  *Phase 1 (local optimization)*: For each node i, evaluate ΔQ of moving i into each neighbor j's community. Key formula:
  > ΔQ = [Σ_in + 2k_{i,in}] / 2m − [(Σ_tot + k_i)/2m]² − [Σ_in/2m − (Σ_tot/2m)² − (k_i/2m)²]
  where Σ_in = sum of weights inside the community, Σ_tot = sum of all weights incident to community, k_{i,in} = weight of links from i to community. Move i to community giving max ΔQ (if positive). Repeat sequentially over all nodes until no improvement (local maximum of Q). 
  *Phase 2 (aggregation)*: Build a new weighted network where nodes are the communities found in Phase 1. Self-loops represent within-community edges. 
  Repeat phases (each iteration = one "pass") until no further improvement.

- **Key properties.** (1) Hierarchy: each pass produces a level of the community hierarchy; multiple passes provide different organizational scales. (2) Speed: near-linear on sparse graphs (O(n log n) typically); 118M-node network processed in 152 minutes. (3) Multi-resolution: the intermediate partitions at each pass correspond to local Q maxima at different scales, partially addressing the resolution limit. (4) Ordering invariance: Q values robust across node orderings (σ_Q ≈ 10⁻² for 2M-node network); computation time more variable.

- **Empirical validation.** Belgian mobile phone network (2M customers, 6 months of calls): identified 261 communities, strongly segregated by language (>85% monolingual in all but one large community of mixed French/Dutch speakers). This demonstrates community detection can recover non-trivial socio-economic structure.

- **Resolution limit.** Recognized but partially mitigated: the first phase only moves individual nodes, so distinct small communities (even a ring of cliques) can be detected at the first pass; they may only be merged in later passes. This gives the user access to multiple resolution levels.

- **Relevance to project.** Louvain is the standard alternative to BRIM for unipartite or larger networks. For Chinese firm-product networks with millions of firm-product pairs, Louvain may be more computationally tractable than BRIM for robustness checks. The hierarchical output also provides a natural multi-resolution view of capability blocks: coarser passes give fewer, larger capability communities; finer passes give more, smaller communities. Robustness of the d_in/d_out decomposition across Louvain resolutions would strengthen the empirical findings.

---

### Duch & Arenas (2005) — "Community detection in complex networks using extremal optimization"
*Physical Review E 72: 027104*

- **Main contribution.** Extremal optimization (EO) algorithm for modularity maximization. Introduces a node-level fitness measure λ_i and uses it to drive a search that avoids local optima better than greedy algorithms. This is the best prior algorithm against which Newman (2006) and Blondel (2008) are benchmarked.

- **Node fitness.** For node i in community r(i):
  > λ_i = κ_{r(i)} / k_i − a_{r(i)}
  where κ_{r(i)} = number of links from i to nodes in the same community, k_i = degree of i, a_{r(i)} = fraction of all network links incident to community r(i). λ_i ∈ [−1, 1]; positive means i has more within-community links than expected; negative means i is poorly placed in its community.

- **Algorithm.** Start with random bipartition of vertices into two equally-sized groups. At each step, select the node with the lowest fitness λ (the "worst-fitting" node) using τ-EO: P(q) ∝ q^{−τ} where q is the rank of the node by fitness and τ ≈ 1 + 1/ln(N) is tuned near the optimal value. Move that node to the other partition. Track the best Q found so far. Stop after αN steps without improvement (α=1 in practice). Recursively cut edges between the two partitions and repeat on each connected component.

- **Performance.** Q_{EO} > Q_{Newman} by up to 15% across tested networks. Detects communities up to z_out = 8 (vs z_out = 6 for GN) in benchmarks with 4 communities of 32 nodes. O(N² log N) time — slower than Louvain, not suitable for networks >30K nodes.

- **Relevance to project.** DA is the benchmark for community detection quality; it is cited in Newman (2006) as the best prior method and outperformed by Newman's spectral approach for large networks. For the project, DA's performance on small/medium networks (up to 10K firms) provides a quality ceiling for BRIM — if BRIM finds Q values comparable to DA on the same network, the partition is near-optimal.

---

### Almeida-Neto, Guimarães, Guimarães Jr, Loyola & Ulrich (2008) — "A consistent metric for nestedness analysis in ecological systems: reconciling concept and measurement"
*Oikos 117(8): 1227–1239*

- **Main contribution.** Introduces NODF — Nestedness based on Overlap and Decreasing Fill — as a replacement for matrix temperature T and discrepancy d, which are shown to suffer systematic type I errors (detecting nestedness where none exists). NODF is the standard nestedness metric in EFC literature (used in Mariani 2019, §2e, and in the Saracco et al. null model papers, Batch 3c).

- **Two conditions for nestedness.** For rows (or columns), nestedness between row i and row j requires:
  1. *Decreasing fill (DF)*: MT_i > MT_j (row i has more 1's than row j). If MT_i ≤ MT_j → N^paired_{ij} = 0 (no contribution).
  2. *Paired overlap (PO)*: The fraction of row j's 1's that coincide with row i's 1's: PO_{ij} = O_{ij} / k_j.
  Combined: N^paired_{ij} = PO_{ij} if MT_i > MT_j, else 0.

- **NODF formula.** 
  > NODF = Σ_{all row pairs} N^R_{ij} + Σ_{all column pairs} N^C_{kl}  /  [m(m−1)/2 + n(n−1)/2]
  where m = number of rows, n = number of columns, and the sums are over all pairs where the ordering (by fill) is strict. NODF = 100 for a perfectly nested matrix (complete overlap with strictly decreasing fill); NODF ≈ 50 for a random matrix of moderate fill; NODF = 0 for non-nested structures (checkerboard, compartmented, etc.).

- **Key critique of prior metrics.** For random matrices (no nestedness): T gives 52%, d₁ gives 67–68%, and NC gives 0%. Only NODF gives ~50% (indistinguishable from a random expectation with no type I error). For non-nested structures (checkerboard, beta-diversity, exclusive subsets): T and d₁ incorrectly detect "nestedness" (T=9–38%, d₁=33–51%), while NODF correctly gives 0. This makes T and d₁ fundamentally unreliable.

- **Additional properties.** (1) Separate row-nestedness and column-nestedness can be computed — allows testing whether diversification (row-nestedness) and product specialization (column-nestedness) differ. (2) Unaffected by matrix shape and size (confirmed by simulations). (3) Mildly related to fill for absolute values but z-scores under FF null model are fill-independent. (4) 237/287 empirical ecological matrices significantly nested under EE null; only 3/287 under FF null — confirming that null model choice is critical (reiterating §2e's BiCM recommendation).

- **Critical empirical finding.** T and d₁ overestimate nestedness for 92.3% and 99.6% of empirical matrices relative to NODF. This means all studies using matrix temperature to validate EFC bipartite networks have likely over-reported nestedness significance. The appropriate metric for validating M_ipt is NODF with the BiCM null model.

- **Relevance to project.** NODF is the metric to use when validating that the firm-product bipartite matrix M_ipt is significantly nested. Specifically: (1) compute raw NODF for M_ipt; (2) compute z-score against the BiCM null model (Squartini-Garlaschelli 2012, §2e); (3) report separately for row-NODF (cross-firm nested ordering) and column-NODF (cross-product nested ordering). The finding that column-NODF may be lower than row-NODF (as in §2e for the country-product matrix) would indicate that product specialization is less nested than firm diversification — informative for the project's interpretation of d_in/d_out.

---

### Cross-paper synthesis (§3a)

**1. The algorithmic chain: Q → BRIM → d_in/d_out.** Newman (2006) establishes the modularity framework (Q = fraction of within-group edges in excess of random expectation) and the eigenvector method. Barber (2007) adapts it to bipartite networks via SVD of B̃ and introduces BRIM. De Stefano (2025, Batch 1) applies BRIM to M_ipt to produce the block partition {Ξ_i, Ξ_α}. d_in and d_out directly measure movement within vs. across those blocks. The entire chain from raw trade data to our causal outcome variables passes through this sequence.

**2. Q is a relative measure.** All modularity metrics measure departure from the configuration-model null (k_i d_α/m for bipartite; k_i k_j/2m for unipartite). Q > 0 means real structure beyond what the degree sequence alone predicts. This is analogous to the BiCM z-score for NODF: both compare the observed structure to a degree-preserving random baseline. For the project, a high Q for M_ipt means the firm-product co-specialization pattern is genuinely block-structured, not merely a consequence of some firms being highly diversified and some products being widely exported.

**3. BRIM finds local optima; robustness requires multiple runs.** BRIM guarantees convergence to a local maximum of Q. For the project's M_ipt, multiple random initializations of BRIM should be run, and the partition with the highest Q selected. The stability of d_in/d_out outcomes across multiple BRIM runs (using normalized mutual information between partitions) is an empirical check of partition robustness.

**4. NODF is the correct nestedness measure; T is not.** Almeida-Neto (2008) establishes that matrix temperature T and discrepancy d₁ both produce systematic type I errors. The appropriate metric is NODF with a degree-preserving null model (FF or BiCM). Any prior EFC paper using temperature to validate nestedness of the country-product or firm-product network has likely inflated its nestedness estimates. The project should use NODF + BiCM throughout.

**5. The Louvain algorithm as a robustness tool.** For large Chinese firm-product networks (potentially millions of firm × product pairs per year), Louvain (Blondel 2008) is computationally superior to BRIM and can serve as a robustness check on the block structure. If d_in/d_out estimates are stable across BRIM and Louvain partitions, the results are insensitive to the specific community detection algorithm.

---

## §3b — Community Detection Review + In-Block Nestedness (Batch 3b)

*Papers read in full, 2026-06-04*

---

### Fortunato & Hric (2016) — "Community detection in networks: A user guide"
*Physics Reports 659: 1–44* — **Comprehensive review: definitions, validation, methods critique**

- **Main contribution.** A 44-page practitioner-oriented review of network community detection, covering (1) what communities are, (2) how to validate algorithms, (3) a critical assessment of popular methods. Particularly important for our project: the resolution limit of modularity, the detectability threshold, the consensus clustering technique, and the recommendation for a posteriori stochastic block modelling as the gold standard. Co-author Hric focuses on the structure-vs-metadata mismatch result.

- **Definition landscape.** Classic definitions (strong community = every vertex has more internal than external edges; weak community = sum of internal degrees > sum of external degrees) are shown to be size-dependent and unreliable. The modern view replaces edge counting with edge probabilities via the stochastic block model (SBM): P(i↔j) = p_{g_i, g_j}, where g_i is vertex i's group label. SBM encompasses assortative (communities), disassortative, core-periphery, and multipartite structures within a single framework. For M_ipt, the SBM framework is more flexible than BRIM's pure-assortative Q, and is directly relevant for the bipartite SBM by Larremore et al. [Phys. Rev. E 90, 012805 (2014)].

- **Detectability limit** (§3.3). For the sparse planted partition model with q groups and total expected degree ⟨k⟩, the theoretical detectability threshold (Decelle et al. 2011) is:
  > ⟨k_in⟩ − ⟨k_out⟩/(q−1) > √(⟨k_in⟩ + ⟨k_out⟩)
  Below this threshold, no algorithm can detect communities better than random assignment — not a failure of the method but a fundamental information-theoretic limit. For the GN benchmark (4 groups, ⟨k⟩=16), theoretical limit is ⟨k_out⟩≈9, not 12 (the edge-density criterion) or 8 (the strong-community criterion). In sparse Chinese firm-product networks (low average firm degree), some years may fall in the undetectable regime — this must be empirically checked via the non-backtracking matrix spectrum before interpreting BRIM results.

- **Structure vs. metadata mismatch** (§3.4). Critical negative result: structural communities detected by topology-based algorithms are poorly correlated with annotated groups in most large real networks (NMI < 0.2 for social, information, and technological networks with thousands of vertices). For the project: industry classification (HS sections or 2-digit codes) should not be used as external validation of BRIM blocks. The BRIM blocks reflect co-export proximity structure, not pre-defined sector boundaries. Validating BRIM against HS product sections would conflate structural and metadata-based communities.

- **Resolution limit of modularity** (§4.6). The most operationally important section for BRIM users. Newman-Girvan modularity Q has a preferential community scale:
  > Q prefers communities of size k_C ~ √m
  Communities smaller than √m are systematically merged by modularity maximisation. For a firm-product network with m edges, if m = 10^6 (realistic for Chinese data), the resolution limit is ~10^3 edges per community — meaning product blocks with fewer than ~1000 firm-product links may be artifactually merged by BRIM. **This is a direct limitation of De Stefano's BRIM application that must be addressed in the empirical strategy.** Solutions: (a) run hierarchical BRIM (multiple passes from refined initial partition); (b) use I-optimization (Solé-Ribalta 2018, below); (c) report robustness across a range of q values.

- **Modularity landscape fragmentation** (§4.6). The space of high-Q partitions is exponentially large, with many structurally dissimilar partitions having nearly identical Q values. This explains why BRIM produces different block assignments across multiple random initializations. **Consensus clustering is the recommended fix**: run BRIM n_P times, build consensus matrix D_{ij} = fraction of runs in which firms i and j are assigned to the same block, threshold D at τ, and re-cluster until convergence. This produces a unique, robust partition. For d_in/d_out measurement, the consensus partition is more reliable than any single BRIM run.

- **Consensus clustering** (§4.2). Algorithm: (1) run algorithm n_P times → n_P partitions; (2) compute D_{ij} = fraction of runs co-assigning i,j; (3) zero entries of D below τ; (4) re-cluster D; (5) repeat until convergence (D becomes block-diagonal). Shown to improve accuracy by 10–20% on LFR benchmarks even when individual partitions are poor. Recommended for any application where stochastic algorithms are used (BRIM, Louvain).

- **Multislice modularity and temporal networks** (§4.8). Mucha et al. (2010) extend Q to multilayer/temporal networks via inter-layer coupling parameter ω:
  > Q_multislice = (1/2μ) Σ_{ij,st} [A_{ij,s}δ_{st} − γ_s k_{is}k_{js}/(2m_s)δ_{st} + δ_{ij}ω_{st}] δ(g_{is}, g_{jt})
  where s,t index time slices, ω_{st} is the coupling weight between consecutive slices (non-zero only for |s-t|=1 in a sequential network), and μ = Σ_s m_s + ω × n × (T-1) is the total weight. ω → 0 recovers independent per-slice Q; ω → ∞ forces identical partitions across all slices. This is directly the framework behind the TEMPORAL-COUPLED BRIM decision (ADR-0001) in the project. The coupling ω suppresses spurious relabeling across years, so block identity is stable and d_out counts genuine firm movements rather than algorithmic reassignments.

- **Significance of detected communities** (§4.9). Many clustering algorithms find communities in random graphs (Erdős-Rényi) simply due to random fluctuations. One must always test whether the detected block structure is statistically significant. For M_ipt: (a) compute z-score of Q against the configuration-model null (rewire edges preserving degrees); (b) use OSLOM or BiCM (Squartini-Garlaschelli 2012, Batch 3c) as the significance test. Any block structure with z < 3 should be treated with caution and not reported as meaningful without further validation.

- **Method recommendation** (§4.10). Hierarchy of recommended methods: (1) a posteriori SBM (degree-corrected, Karrer-Newman; hierarchical, Peixoto) is the gold standard — flexible, detects all structure types, model selection to find q; (2) cluster quality functions (OSLOM) for local exploration; (3) modularity optimization only when q is known and constrained. Louvain is good for speed on large networks but use the bottom hierarchy level (smallest clusters), not the highest-Q partition.

- **Relevance to project.** Three direct implications: (a) The resolution limit means BRIM on M_ipt may merge small capability blocks — this must be checked empirically and addressed via multi-resolution robustness. (b) Consensus clustering over multiple BRIM runs (n_P ≥ 50, threshold τ = 0.5) should be the standard methodology, not a single run. (c) Temporal-coupled BRIM (ADR-0001) is formally motivated by multislice modularity framework — ω parameter should be set by cross-validation (robustness of d_in/d_out to ω) or set to the Mucha et al. recommended ω = median(k_{is}) across years.

---

### Solé-Ribalta, Tessone, Mariani & Borge-Holthoefer (2018) — "Revealing in-block nestedness: Detection and benchmarking"
*Physical Review E 97: 062302* — **In-block nestedness quality function I + joint partition/nestedness optimization**

- **Main contribution.** Introduces in-block nestedness (IBN) as a compound structural property: a network exhibits IBN if it is divided into blocks that are each internally nested. Proposes the IBN fitness function I (Eq. 4) that jointly optimizes partition assignment and within-block NODF. Shows that existing approaches — measuring Q and NODF independently, or measuring NODF within Q-detected blocks — systematically miss IBN structure. Tested on 334 real networks (57 unipartite, 277 bipartite). **This paper is the direct methodological basis for d_in in the project.**

- **Global nestedness N̂.** The paper first defines a null-model-corrected global nestedness:
  > N̂ = (2/(N_r + N_c)) × [Σ_{row pairs s,t} (O_{st} − ⟨O_{st}⟩) / (k_t(N_r − 1)) × Θ(k_s − k_t) + same for columns]
  where O_{st} = overlap (number of shared column neighbors), ⟨O_{st}⟩ = k_s k_t / N_c (expected under configuration null). Θ(k_s − k_t) is the Heaviside function enforcing the decreasing-fill condition (only pairs where s has strictly more links than t contribute). This differs from raw NODF (§3a) in that it subtracts the degree-sequence baseline.

- **In-block nestedness fitness I** (Eq. 4). The full formula for bipartite networks:
  > I = (2/(N_r + N_c)) × [Σ_{s,t: α_s=α_t} (O_{st}^{block} − ⟨O_{st}⟩) / (k_t(C_s − 1)) × Θ(k_s − k_t) + same for columns]
  where: (a) α_s = membership variable (block assignment of row node s); (b) O_{st}^{block} = Σ_υ A_{sυ}A_{tυ}δ(α_s, α_υ) = overlap restricted to column nodes in the SAME BLOCK as s and t; (c) ⟨O_{st}⟩ = k_s k_t / N_c (expected overlap over ALL columns, regardless of block, under configuration null); (d) C_s = size of the block containing s (number of rows + columns). Critical: I reduces to N̂ when all nodes are in one block (single partition), and I → Q-like formula when within-block nestedness is absent.

- **I has no resolution limit.** Unlike Q, I is built on normalized pairwise overlaps (a local quantity relative to block size C_s), NOT relative to the total number of links m. Formal result: for a ring of in-block nested subgraphs, I_{single} > I_{pairs} for ALL values of B (the number of blocks in the ring). Q_{single} < Q_{pairs} for large B (Q's resolution limit). Intuition: adding a node to a block improves I only if the node fits the nested structure; otherwise it is better placed in a separate block. This means I-optimization will correctly identify small capability blocks that BRIM (Q-based) would merge.

- **Q is insensitive to internal nestedness.** Synthetic experiment (B=3, ξ=3, varying p and μ): Q is nearly constant across all values of p (within-block noise parameter). This means BRIM (Q-optimization) cannot distinguish between a block with perfectly nested internal structure (p=0) and a block with random internal structure (p=1). The partition it produces is modularity-optimal but agnostic about within-block hierarchy. **This is a fundamental limitation of De Stefano's BRIM application: the detected blocks have good modularity but their internal nested hierarchy is unverified by the optimization procedure itself.**

- **Sequential approach (Q first, then NODF within blocks) fails.** I-values from Q-detected partitions are far below the I-values from I-optimized partitions for most of the (p, μ) parameter space, especially when there are clear IBN structures. The sequential approach (used in much prior ecology literature) misses IBN structure in ~80% of real networks in the 334-network empirical study.

- **Empirical evidence.** Of 334 real networks, most show significant IBN structure under I-optimization that goes undetected by Q+NODF analysis. Key examples: (a) host-parasite bipartite network: I-optimization finds one large nested block + several small nested clusters; Q-optimization finds several equally-sized dense modules with no nested internal organization. (b) pollination mutualistic network: clear IBN detected by I, completely missed by Q. (c) global nestedness N̂ ≈ 0 for some of these networks — the IBN structure is hidden because it coexists with modularity, and the global NODF is suppressed by the block structure.

- **Q and I are uncorrelated in real networks.** Scatter plot of (Q, I) for all 334 networks: low correlation. Networks with moderate Q (near random-graph value) can have high I. Networks with high Q (clear block structure) can have low or high I. The two measures capture genuinely different structural properties.

- **Optimization algorithm.** I-maximization uses a biologically inspired algorithm (Karaboga-Akay artificial bee colony, Artificial Intelligence Review 31: 61, 2009). The I formulation "closely follows modularity Q", so most existing heuristics for Q-optimization (including BRIM's SVD-based assignment) can be adapted. The paper notes that I-maximization can also be performed with the Combo algorithm (Sobolevsky et al., Phys. Rev. E 90, 012811, 2014) after adaptation.

- **Resolution limit analysis** (§IV). Detailed proof that I has no resolution limit: (a) unlike Q, I doesn't depend on a global quantity like m; (b) for a ring of nested subgraphs connected by ℓ* inter-block links, even in the adversarial case where I_{pairs} > I_{single} at B=2, the ordering reverses as B grows — I eventually recovers the natural partition. (c) detectability of small blocks INCREASES as network size grows (opposite of Q's resolution limit).

- **Connection to Mariani (2019) (§2e).** Mariani's §7.3 directly cites this paper and explains that d_in = progress up within-block nested hierarchy (as measured by I) and d_out = jumping to a new block. The current paper makes this connection explicit: firms with higher within-block degree (more intra-block capabilities) are the "hubs" of the within-block nested structure; d_in = a new product whose column node is nested below these hubs in the same block; d_out = a product in a different block.

- **Relevance to project.** Four direct implications for the empirical design:
  1. **BRIM is a measurement approximation, not the ideal method.** BRIM maximizes Q, not I. The within-block nested hierarchy that defines d_in is not optimized by BRIM. For robustness, I-optimization should be run as an alternative partition method and d_in/d_out estimates compared.
  2. **The I function is computable on M_ipt.** The bipartite formulation (Eq. 4) applies directly to firm-product bipartite networks. Row = firms, column = products, α_i = block assignment, O_{st}^{block} = number of shared-product exports within the same block. This can be implemented in Python using the BRIM partition as initialization and optimizing I locally.
  3. **Within-block degree ranking is meaningful.** For a given block b, rank firms by their degree within M_ipt restricted to block b. Firms at the top of this ranking are the most diversified within the block = most central in the within-block nested hierarchy. A tariff shock hitting these hub firms should have different effects on d_in vs. d_out compared to firms lower in the block hierarchy. This is a source of heterogeneous treatment effects.
  4. **"NODF within Q-detected blocks" is insufficient.** Simply computing NODF for products within each BRIM block does not give the IBN-optimal partition. The I-optimization procedure should be run at least as a robustness check.

---

### Cross-paper synthesis (§3b)

**1. The chain from Q-optimization (BRIM) to I-optimization (in-block nestedness).** Barber (2007, §3a) introduced BRIM as a bipartite Q-maximizer. Fortunato & Hric (2016) expose the resolution limit and consensus clustering recommendations for any Q-based method. Solé-Ribalta et al. (2018) show that Q is insensitive to within-block nested structure and propose I as the correct objective function when within-block hierarchy matters. For the project: the full measurement chain for d_in should ultimately run I-optimization on M_ipt, with BRIM as a computationally tractable approximation and I-optimization as the robustness check.

**2. Consensus clustering + I-optimization = the recommended pipeline.** From Fortunato (2016): run BRIM n_P times, build consensus matrix, re-cluster. From Solé-Ribalta (2018): optimize I on the consensus partition as initialization. This two-step pipeline — consensus BRIM to stabilize the block partition, then local I-optimization to refine within-block structure — gives the most reliable d_in/d_out decomposition.

**3. The detectability limit constrains early years of the panel.** Fortunato (2016) §3.3 shows that for sparse networks with few inter-block connections, communities can be fundamentally undetectable regardless of algorithm. Chinese firm-product networks in early years (2000–2003) likely have lower average degree (fewer products per firm before China's WTO accession ramp-up). The non-backtracking matrix spectrum test should be run per year to confirm that block structure is detectable before interpreting BRIM results.

**4. The resolution limit invalidates small-block interpretation without correction.** Fortunato's resolution limit (communities smaller than √m are merged) is operationally binding for M_ipt. If the project's BRIM detects K blocks with ≈ m/K edges each, blocks with k_block < √m are suspect. Multi-resolution robustness (varying the effective resolution parameter in multislice BRIM) and comparison with I-optimization (which has no resolution limit) are both needed.

**5. Temporal-coupled BRIM (ADR-0001) is formally grounded in multislice modularity.** Mucha et al.'s multislice modularity with inter-layer coupling ω is exactly the framework behind ADR-0001. ω suppresses spurious block-label permutations across years, ensuring that measured d_out counts real cross-block product entries rather than algorithmic relabeling. Fortunato (2016) §4.8 provides the mathematical basis and warns that the multislice approach inherits Q's resolution limit — for temporal BRIM, run consensus clustering across time slices (overlapping windows) rather than single-shot optimization.

**6. NODF, Q, and I are measuring three different things.** NODF + BiCM (§2e/§3a) tests whether M_ipt is globally nested beyond degree-sequence expectation. Q (BRIM, §3a) tests whether M_ipt has block structure beyond the configuration model. I (this batch) tests whether M_ipt has blocks that are themselves internally nested. The project needs all three: NODF for baseline structural validation, Q for block detection, I for within-block hierarchy measurement (the precise definition of d_in).

---

## §3c — Entropy/BiCM Null Models (Batch 3c)

*Papers read in full, 2026-06-04*

---

### Squartini & Garlaschelli (2011) — "Analytical maximum-likelihood method to detect patterns in real networks"
*New Journal of Physics 13: 083001* — **Foundational maximum-likelihood method for randomized network ensembles**

- **Main contribution.** Proposes the maximum-entropy/maximum-likelihood (ML) method for generating analytically tractable randomized ensembles of real networks, replacing both computational LRA methods (expensive) and naive analytical approximations (incorrect). The method covers binary undirected (CM), directed (DCM), reciprocal (RCM), and weighted (WCM) networks within a unified framework. This paper is the direct mathematical foundation for the BiCM (Saracco 2015) and for all z-score-based pattern detection in EFC research.

- **The problem with the naive null model.** The standard approximation p_{ij} = k_i k_j / (2L) [Eq. 1] — used in virtually all prior literature including the standard modularity Q — is formally incorrect for any network where k_i k_j > 2L (i.e., for high-degree nodes in dense or scale-free networks). The correct expression requires solving a system of N coupled nonlinear equations. The naive expression also makes modularity Q biased: the correct Q requires the exact p_ij from the ML method, not the approximation.

- **The ML method — binary undirected case.** Find the parameter vector x* = {x_1,...,x_N} that solves:
  > Σ_{j≠i} x_i* x_j* / (1 + x_i* x_j*) = k_i(G*) ∀i   [Eq. 5]
  The correct link probability is then:
  > p_ij* = x_i* x_j* / (1 + x_i* x_j*)   [Eq. 6]
  This replaces the naive approximation and is always in [0,1] by construction. The expectation value of any topological property X (clustering, ANND, motif counts, NODF, modularity) is obtained by substituting p_ij* for a_ij in the definition of X. Standard deviation σ*[X] follows analytically from the same parameters. Z-score: z[X] = (X(G*) − ⟨X⟩*) / σ*[X].

- **Computational advantage.** Total time to compute ⟨X⟩ analytically ≈ O(T_E + T_X), where T_E is negligible. The LRA alternative requires O(M · R · T_R + M · T_X) where M ≫ 1 and R ≫ L — orders of magnitude slower. For the large Chinese firm-product networks (N_firms ~ 10^4−10^5, N_products ~ 5000), the LRA would be prohibitively slow; the ML method makes null-model computation feasible.

- **Extension to weighted networks (WCM).** Constraints: strength sequence {s_i = Σ_j w_ij*}. System:
  > Σ_{j≠i} x_i* x_j* / (1 − x_i* x_j*) = s_i(W*) ∀i   [Eq. 16]
  Expected weight: ⟨w_ij⟩* = x_i* x_j* / (1 − x_i* x_j*)   [Eq. 17]. Note the negative sign in the denominator (vs. positive for binary). The naive expression ⟨w_ij⟩ = s_i s_j / (2W) [Eq. 15] is equally incorrect as its binary counterpart.

- **Consequence for modularity.** Q (Newman-Girvan) is defined as Q = (1/2L) Σ_{i≠j} (a_ij − p_ij) δ(C_i, C_j). Using the naive p_ij = k_i k_j / 2L gives a biased Q. The correct Q uses exact p_ij* from Eq. 6. For any network that is dense, small, or has a broad degree distribution (all three apply to firm-product networks), the naive Q underestimates the expected number of within-community links, inflating Q and potentially detecting spurious community structure. **BRIM — which maximizes the naive Q — is therefore built on an approximation. For rigorous community detection on M_ipt, the exact BiCM p_ipt should replace the naive null model in Q.** This has not been addressed in De Stefano (2025) or the EFC literature more broadly.

- **Directed case (DCM).** Constraints: joint in-degree and out-degree sequences {k_i^in, k_i^out}. Two parameter vectors x*, y* solving 2N equations; link probability p_ij = x_i* y_j* / (1 + x_i* y_j*). Also shown: under the correct DCM, the null model can be assortative (not just disassortative) — the topology of the specific real network determines the direction, not any universal prior.

- **Relevance to project.** Three direct implications: (1) All z-score validation of M_ipt (NODF, modularity, motif counts) must use the ML-derived p_ipt = x_i* y_p* / (1 + x_i* y_p*), not the naive approximation. (2) The BiCM (Saracco 2015) and BRIM's Q are both derived from this framework — BRIM uses the approximate version, BiCM uses the exact version. (3) A rigorous BRIM implementation would replace the naive null model in Q with exact BiCM link probabilities; this would change the detected partition and remove the approximation-induced bias.

---

### Saracco, Di Clemente, Gabrielli & Squartini (2015) — "Randomizing bipartite networks: the case of the World Trade Web"
*Scientific Reports 5: 10595* — **BiCM: Bipartite Configuration Model**

- **Main contribution.** Extends the ML method (Squartini & Garlaschelli 2011) to bipartite networks, introducing the BiCM. Applied to the binary, undirected bipartite representation of the World Trade Web (WTW), 1963–2000 (C ≤ 151 countries, P = 538 products, RCA-binarized). This is the null model used in Mariani (2019) §2e for NODF z-scores, and the baseline for all statistical validation of M_ipt.

- **BiCM formulation.** Constraints: country diversification sequence {d_c} and product ubiquity sequence {u_p}. Hamiltonian: H(M, α, β) = α·d(M) + β·u(M). Link probability:
  > p_cp = x_c y_p / (1 + x_c y_p)
  where x_c = e^{−α_c}, y_p = e^{−β_p}, and (x*, y*) solve the system:
  > Σ_p x_c y_p / (1 + x_c y_p) = d_c ∀c;    Σ_c x_c y_p / (1 + x_c y_p) = u_p ∀p   [Eq. 19]
  Identical functional form to Eq. 6, but with TWO sets of parameters (one per layer). The link probability for the bipartite case is fully factored: P(M | x*, y*) = Π_{c,p} p_cp^{m_cp} (1−p_cp)^{1−m_cp}.

- **Key empirical results on WTW.**
  1. *Assortativity (ANPU, ANCD)*: BiCM captures the decreasing (disassortative) trend, but many observed points lie outside ±2σ. Prediction is close to the BiRG (random graph), reducing entropy by only 16% (vs. 41% in the monopartite projection). **The bipartite degree sequence explains MUCH LESS of the network structure than the monopartite degree sequence does.** This is the fundamental limitation of the BiCM as a null model for capability detection.
  2. *Fitness and complexity*: BiCM reproduces the fitness/complexity trends closely (observed points lie within ±2σ) — the poverty trap structure and the beak shape of complexity are explainable by degree heterogeneity.
  3. *V-motifs (country co-export)*: z_{Vn} < −1.65 across all years. Countries form FEWER co-export pairs than expected under BiCM → countries AVOID competing on the same products beyond what diversification/ubiquity would predict. This is non-trivial: it means the capability structure is not captured by degree sequence alone. **For M_ipt: if firms exhibit similar Vn z-score patterns (fewer co-export firm pairs than BiCM expects), this would directly confirm that firm-level export specialization has a capability basis beyond mere size/diversification.**
  4. *Nestedness (NODF)*: BiCM reproduces global NODF (within ±2σ) across the full 38-year dataset. Global nestedness IS largely explained by degree heterogeneity. BUT row-NODF (firm diversification axis) is underestimated in some years → additional structure in rows beyond degree sequence. Confirmed by Mariani (2019) §2e: row-NODF is more significant than column-NODF under BiCM z-score.
  5. *Assortativity coefficient r*: BiCM overestimates r (predicts less disassortative than observed) — additional disassortativity in real WTW not captured by degree constraints.

- **Comparison BiCM vs. monopartite projection.** Working in bipartite representation reveals structure invisible in the monopartite case. When the WTW is projected to the country-country layer and the monopartite CM is applied, 41% of Shannon entropy is explained by degree sequence. In bipartite representation, only 16%. This means: the bipartite structure contains richer capability information than the projected structure, and a higher fraction of it remains unexplained by degree heterogeneity alone. For M_ipt, this strongly supports working with the bipartite firm-product matrix directly rather than projecting to firm-firm or product-product monopartite networks.

- **BiCM as standard null model.** The BiCM provides: (a) a z-score for NODF = (NODF_obs − ⟨NODF⟩_BiCM) / σ_BiCM; (b) z-scores for any motif count; (c) expected Vn motifs for subsets of firms (e.g., by region, ownership, industry). All structural validation of M_ipt should use the BiCM as baseline. Firms that form significantly more V-motifs than BiCM expects are forming capability clusters not explainable by their diversification level alone.

- **Software.** The BiCM can be computed using the `bicm` Python package (https://github.com/tsakim/bicm), cited by Cimini et al. (2022). The system (Eq. 19) is solved by Newton-Raphson or gradient descent. For C=10^4 firms and P=5000 products, the 15,000 equations are computationally demanding but tractable.

- **Relevance to project.** Four direct implications: (1) The BiCM p_{ipt} is the correct link probability to use in both the NODF z-score and the corrected BRIM Q. (2) Vn motif z-scores for M_ipt constitute a direct test of capability clustering beyond diversification. (3) Row-NODF z-score distinguishes whether firm-level nested ordering is a degree artifact or a genuine structural feature. (4) The finding that assortativity is NOT explained by degree sequence in the bipartite WTW suggests that Chinese firm export patterns likely have additional structure beyond diversification/ubiquity — motivating the block-level analysis.

---

### Cimini, Carra, Didomenicantonio & Zaccaria (2022) — "Meta-validation of bipartite network projections"
*Communications Physics 5: 76* — **Reconciliation of CM formulations for projection validation**

- **Main contribution.** Systematically compares four CM-based null models for validating monopartite projections of bipartite networks (Hypergeometric, Curveball, BiPCM, BiCM). Shows that these models produce VERY different validated networks for the same significance threshold p*. Proposes a meta-validation approach: compare validated networks at equal link density ρ (not equal p*) to identify model-specific thresholds where structural similarity is maximized. Applied to the bipartite country-scientific-field network (307 fields × 239 countries, RCA-binarized).

- **Four null models taxonomy** (Table 1):
  | Model | Constraints | Type |
  |---|---|---|
  | Hypergeometric | One layer (set L) only | Partial + Hard/microcanonical |
  | BiPCM | One layer (set L) only | Partial + Soft/canonical |
  | Curveball | Both layers | Full + Hard (link swap algorithm) |
  | BiCM | Both layers | Full + Soft/canonical |
  Key: Partial models (Hypergeometric, BiPCM) use ⟨C_ij⟩ = k_i k_j / |Γ|; Full models (Curveball, BiCM) use ⟨C_ij⟩ = k_i k_j Σ_α κ_α^2 / E^2 > k_i k_j / |Γ| (larger expected co-occurrence). BiCM is most conservative (validates fewest links).

- **Why different models give different results.** Full models account for heterogeneity in BOTH layers; partial models ignore one layer's heterogeneity. Hard constraints fix degree sequences exactly; soft constraints fix them as averages (wider distributions → lower p-values needed to reject null). These differences are strongest for high-degree nodes (Fig. 3 in paper): mean co-occurrences and variance of Hypergeometric vs. BiCM differ by factors of 2–10 for node pairs with degree > 0.5|Γ|.

- **Meta-validation finding.** Comparing validated networks at the SAME p* gives low structural similarity (Jaccard, DeltaCon, Portrait < 0.5). Comparing at EQUAL LINK DENSITY ρ gives much higher similarity. AMI between community partitions peaks at ρ ≈ 0.2 for the scientific field network, where all four models find the same 4-community structure (matching broad scientific disciplines: life sciences, social/economics, physical sciences, formal sciences). This is the meta-validated partition.

- **Meta-validation algorithm.** (1) For each model, compute ρ(p*) curve. (2) Compute AMI between all 6 model pairs as a function of ρ. (3) Find ρ* that maximizes average AMI. (4) For each model, adjust p* to achieve ρ = ρ*. (5) The partition found at ρ* is the meta-validated partition — the most robust community structure independent of null model choice.

- **Key negative results.** (1) Applying a monopartite null model directly on the projection (instead of defining the null on the bipartite network) "discards the information contained in the original bipartite network" — leads to entirely different and typically non-significant results. (2) Community structure detected via BiCM-validated projection does NOT match Scopus expert classification (ASJC subject areas) — same structure-vs-metadata mismatch found by Fortunato (2016) §3.4. (3) The difference between microcanonical (hard) and canonical (soft) ensembles does not vanish in the thermodynamic limit — non-equivalence of ensembles is fundamental (Squartini et al. 2015, Phys. Rev. Lett. 115: 268701).

- **Relevance to project.** Three implications: (1) For validating the product-product co-occurrence projection of M_ipt (C_pp' = Σ_i M_ipt M_ip't), meta-validation should be run across all four CM formulations. The BiCM is most conservative but the meta-validated partition at ρ* is the most robust result. (2) If BiCM and Hypergeometric agree on capability clusters at equal ρ, those clusters are genuinely structural. (3) This framework applies to validating the PROXIMITY network φ_{pp'} = C_pp' / max(u_p, u_p') — the foundation of the product space / relatedness concept — replacing ad hoc threshold choices with a principled meta-validation approach.

---

### Cross-paper synthesis (§3c)

**1. The correct null-model pipeline for M_ipt.** The full rigorous pipeline integrating §3a–§3c is: (a) Compute BiCM parameters (x_i*, y_p*) by solving Eq. 19 (Saracco 2015) for each year t; (b) Use p_{ipt} = x_i* y_p* / (1 + x_i* y_p*) as the correct null; (c) Compute NODF z-score against BiCM for structural validation (Almeida-Neto 2008 + Mariani 2019); (d) Compute corrected BRIM Q by replacing the naive k_i d_α / m with BiCM-derived null in Barber (2007) Eq. 4; (e) Validate product-product projection C_pp' using meta-validation across Hypergeometric/BiPCM/Curveball/BiCM (Cimini 2022); (f) Run I-optimization for within-block nestedness (Solé-Ribalta 2018). Each step has a distinct role and cannot be replaced by the others.

**2. The naive modularity Q used in BRIM is formally incorrect.** Squartini (2011) shows that the p_ij = k_i k_j / (2L) used as the null model in Newman-Girvan Q — and therefore in Barber's bipartite extension and BRIM — is an approximation that fails for dense networks and high-degree nodes. The correct null is p_{ipt} = x_i* y_p* / (1 + x_i* y_p*) from BiCM. The resulting corrected BRIM Q partition may differ from the standard BRIM partition, particularly for hub firms (high diversification) and hub products (high ubiquity). Running corrected BiCM-Q BRIM alongside standard BRIM is a robustness check that directly addresses this bias.

**3. V-motifs as a capability-clustering diagnostic.** Saracco (2015) shows that WTW Vn z-scores < −1.65: countries form FEWER shared-product pairs than BiCM expects. For M_ipt, computing V-motif z-scores tests whether firms within the same BRIM block form more co-export pairs than expected by the BiCM (within-block V-motif enrichment). If z_{Vn}^{within-block} > 0 and z_{Vn}^{cross-block} ≈ 0, this would directly confirm that BRIM blocks capture genuine capability clusters beyond what diversification/ubiquity explains. This is a non-trivial validation of the block partition that has not been performed in the EFC firm-level literature.

**4. Microcanonical vs. canonical non-equivalence.** Cimini (2022) notes that ensemble non-equivalence holds even in the thermodynamic limit for bipartite networks with an extensive number of node-specific constraints. This means the Curveball (microcanonical, exactly fixes both degree sequences) and BiCM (canonical, fixes them on average) are not interchangeable even for large networks. For M_ipt: the BiCM is computationally tractable analytically; the Curveball requires Monte Carlo. For standard NODF z-score computation and BRIM null model correction, the BiCM (canonical) is the right choice. The Curveball provides an independent robustness check when computational resources permit.

**5. Meta-validation provides principled thresholds for the product space.** The product space φ_{pp'} = min conditional co-export probability (Hidalgo-Hausmann 2007, implicit; see also proximity in §2d) is typically thresholded ad hoc to select "significant" relatedness links. Cimini's meta-validation framework — find ρ* that maximizes AMI across models — replaces this ad hoc choice with a principled criterion: the density at which the product-product structure is most robustly recovered across all null model formulations. This is directly applicable to selecting which φ_{pp'} links to include in the relatedness/proximity network used for product space visualization.

---

## §5a — Trade, Intermediate Inputs, and Firm-Level Productivity (Batch 5a)

*Papers read in full, 2026-06-04*

---

### Amiti & Konings (2007) — "Trade Liberalization, Intermediate Inputs, and Productivity: Evidence from Indonesia"
*American Economic Review 97(5): 1611–1638* — **Foundational input-tariff / productivity paper**

- **Main contribution.** First paper to isolate the productivity effect of reducing input tariffs from the effect of reducing output tariffs at the firm level, and the first to show that importing firms capture LARGER gains from input tariff cuts than non-importers. Using the Indonesian manufacturing census 1991–2001 (~170,741 firm-year observations, 15K firms/year), it establishes that input tariffs dominate output tariffs as the key trade-policy lever for firm TFP growth.

- **Data and identification.** Annual manufacturing census (SI) covering all firms ≥ 20 employees. Indonesia joined WTO in January 1995 with commitment to reduce all bound tariffs to 40% or below. Tariff variation is cross-industry (291 5-digit ISIC categories) and over time (1991–2001). Political economy concerns about endogeneity addressed: Mobarak-Purbasari (2005) show political connections did not affect tariff rates in Indonesia (corruption operated at firm level via import licenses, not tariff level). Endogeneity checks: IV using initial tariff levels and unskilled labor share — results unchanged.

- **Input tariff construction.** Input tariff for industry k at time t:
  > input_tariff_kt = Σ_j w_jk × output_tariff_jt
  where w_jk = cost share of industry j's output in industry k's production, derived from 288-industry plant-level I/O table (1998 data). Unlike studies using aggregate I/O tables, this uses firm-level cost shares — captures the escalating tariff structure (lower tariffs on inputs, higher on final goods) that aggregate industry classifications miss.

- **TFP estimation.** First stage: Olley-Pakes (1996) methodology, corrected for simultaneity between productivity shocks and (a) input choices, (b) decision to import, (c) decision to export, and (d) exit. Separate production functions estimated for each 3-digit sector (29 industries). Second stage: firm FE panel regression of ln(TFP) on tariff measures.

- **Main specification.** Two-way FE panel (firm + island-year):
  > ln(TFP_it) = α_i + α_lt + γ_1 output_tariff_kt + γ_2 input_tariff_kt + γ_3 (input_tariff_kt × FM_it) + γ_4 FM_it + γ_5 FX_it + γ_6 FF_it + ε_it
  where FM_it = 1 if firm imports any inputs; FX_it = 1 if exporter; FF_it = 1 if ≥10% foreign ownership; α_lt = island × year FE.

- **Key results.** (Table 4):
  - 10pp fall in output tariff → 0.7% TFP gain (after controlling for input tariffs; raw estimate without input tariffs = 2.1% → **omitted variable bias** of >2x when input tariffs excluded)
  - 10pp fall in input tariff → 3% TFP gain for all firms; **12% for importing firms** (γ_3 = −0.91***)
  - FM dummy: importers are 9.2% more productive than non-importers (conditional on tariffs)
  - Exit: firms exiting next period are 4% less productive (selection effect)
  - Product switching: firms that switch main product are 2.9% more productive → some of the tariff gain is from product-mix reallocation (important for the project's d_in/d_out interpretation)

- **Channels identification.** Concentrated industries: output tariff gains accrue ONLY in competitive industries (Herfindahl interaction positive and significant → competition channel only works where mark-ups can be squeezed). Input tariff gains persist equally in concentrated AND competitive industries → input tariffs work via **technology/quality/learning effects**, not competition channel. Exporter interacted with input tariff × FM: insignificant → importing-driven TFP gains are not a learning-by-exporting artifact. Foreign firms excluded: domestically-owned importers still enjoy 10% TFP gain from 10pp input tariff cut.

- **Robustness.** Results hold across: value added per worker, OLS TFP with Cobb-Douglas, OLS TFP with translog, 2-period differences, 5-period differences, 9-period differences, import-weighted tariffs, 3-digit aggregated tariffs (less significant due to multicollinearity), controlling for Asian crisis interactions and trade-weighted exchange rates.

- **Relevance to project.** Five direct implications:
  1. **Input tariff construction methodology.** The weighted-average approach (w_jk × output_tariff_jt) is the standard for constructing firm/industry-level tariff exposure. For the project's EXPORT tariff (the tariff Chinese firms' products face abroad), the Bartik shift-share approach replaces the cost-share weighting — but the logic is analogous: a predetermined weight (pre-shock export share to destination d) × time-varying tariff rate (τ_pdt from Teti GTD) = firm-level tariff exposure.
  2. **The omitted variable problem is documented.** Excluding the interaction term (heterogeneous tariff effect across firm types) overestimates the average main effect. The project must similarly include the d_in × tariff and d_out × tariff decomposition to avoid conflating in-core with out-of-core responses.
  3. **Product switching as a productivity channel.** Amiti shows that firms switching their main product after tariff cuts gain 2.9% in measured TFP, and the interaction (product-switch × input_tariff × FM) is insignificant — input tariff gains for importers are NOT from product switching. For the project: d_in (within-block new products) and d_out (cross-block new products) are precisely the capability-reconfiguration analog of Amiti's product-switch dummy, measured continuously and directionally.
  4. **Selection vs. learning.** The 9.2% importer productivity premium is largely a pre-selection effect (importers are already more productive when they start importing — consistent with Syverson 2011 §4j). The project should analogously test whether firms with higher baseline capability fitness (d_in/d_out level) are more responsive to tariff shocks, not just whether tariff shocks induce diversification.
  5. **Tariff source caution.** Amiti uses Indonesian official HS9-digit tariffs matched to ISIC5-digit via BPS concordance. The project uses Teti GTD (HS6 → HS88/92, bilateral). The tariff concordance challenge (Chinese HS vs. HS88/92) is analogous to Amiti's HS9 → ISIC5 concordance challenge.

---

### Le & Tomasi (2023) — "Trade liberalization and firms' productivity in Vietnam: the role of local business environment"
*Regional Studies 57(9): 1681–1713* — **Tomasi institutional-moderation paper**

- **Main contribution.** Extends the Amiti-Konings framework to a moderated framework: how does the quality of the local business environment where firms are located alter the productivity gains from trade liberalization? Using Vietnamese Enterprise Survey (VES) 2006–2012 (394,403 firm-year observations, 57K firms by 2012) around Vietnam's WTO accession (2007), it shows that firms in provinces with stronger governance capture LARGER gains from tariff cuts. The mechanism runs primarily through importing activity.

> **Note: This paper is co-authored by Chiara Tomasi (University of Trento), Giovanni's institution. Marginal annotations in the PDF suggest Giovanni is reading it as a methodological blueprint for adapting the interaction framework to capability diversification outcomes.**

- **Setting.** Vietnam WTO accession January 2007: large-scale, exogenous MFN tariff reductions, average tariff fell from 18.3% (2007) to 13.8% (2008), industry-varying across 4-digit VSIC sectors. Provincial competitiveness index (PCI) measured annually since 2006 for all 61 provinces — captures governance quality variation that is predominantly cross-sectional (stable over time within province, variable across provinces), providing the moderating dimension.

- **Four provincial governance dimensions.** (1) Legal Institutions: property rights enforcement, court effectiveness, anti-corruption; (2) Land Policies: land-use right certificates (LURCs), expropriation risk, fair compensation; (3) Regulatory Compliance: time spent on bureaucracy, inspection frequency; (4) Education & Labour: provincial vocational training investment.

- **Model.** Two-step:
  - Step 1 (baseline): ln(TFP_ft) = α + β_1 ln(t_it) + β_2 ln(I_pt) + γX_ft + λZ_it + νW_pt + ε_ft [tariff + governance]
  - Step 2 (interaction): ln(TFP_ft) = α + β_1 ln(t_it) + β_2 ln(I_pt) + **β_3 ln(t_it) × D_pt** + γX_ft + λZ_it + νW_pt + ε_ft [key: β_3 < 0 iff better governance amplifies tariff-TFP channel]
  - Three FE variants: (i) sector-year + region trend; (ii) industry-province + year + trends; (iii) firm + year + trends (most demanding)

- **Key results.** (Table 5, 6, 7, 8):
  - Baseline: 100% tariff reduction → 4–20% TFP gain (depending on specification); all four governance dimensions positive for TFP
  - Interaction β_3: negative and significant for all four dimensions. **Magnitudes (100% tariff reduction):**
    - Legal Institutions: +1.2% additional TFP gain for firms in high-quality legal provinces
    - Land Policies: +4.4% (strongest moderator; land as collateral for trade finance)
    - Regulatory Compliance: +3.2% (administrative friction reduces ability to exploit tariff opportunities)
    - Education & Labour: significant only at 10% level
  - Most robust (firm FE, Table 9): Legal Institutions (−0.008**, p<0.05) and Land Policies (−0.019***) remain significant; Regulatory Compliance and Education & Labour weakly significant
  - Import mechanism (Table 10): ln(t_it) × Importer_ft = −0.027 to −0.037*** → importers gain LARGER TFP from tariff cuts, as in Amiti-Konings. This confirms the replication of the Amiti result in Vietnam/WTO context
  - Mediation (Table 11): tariff cuts × governance → higher probability of importing → mechanism is: better governance ENABLES firms to access import opportunities that are opened up by tariff cuts. β_3 on Importer_ft probability equation: legal institutions (−0.002**), land policies (−0.008***), regulatory compliance (−0.003*), education (−0.005**)

- **Identification.** Vietnam's WTO accession is largely exogenous (Vietnam had weak bargaining position, reverse causality tested and rejected — Appendix A3). Endogeneity of PCI partly addressed by the fact that dependent variable (TFP) and regressors (tariffs, provincial indexes) come from independent data sources. Cross-sectional variation in governance dominates time variation in PCI → most identification comes from cross-province differences, not within-province changes.

- **Relation to Amiti-Konings.** Key differences: (a) outcome same (TFP); (b) tariff source: UNCTAD TRAINS vs. Indonesian official HS tariffs — both are MFN applied tariffs, but TRAINS has the systematic interpolation and selection issues documented by Teti (2024, §teti_synthesis); (c) moderator: provincial governance vs. none in Amiti; (d) mechanism: governance enables importing, which drives TFP gain.

- **Relevance to project.** Four direct implications:
  1. **This paper is the closest methodological template for the project's empirical design.** Giovanni's annotations reveal he is adapting it: replace TFP outcome with d_in/d_out; replace PCI governance moderator with regional strategic dependence (ExpDep); replace TRAINS tariffs with Teti GTD. The core interaction structure β_3 (tariff × governance/dependence) is directly transplantable.
  2. **The moderation design is well-identified in the project context.** Vietnam's WTO accession = sudden tariff reduction → exogenous shock identifying β_1. Province-level variation = cross-sectional moderator. For the project: China-US trade war tariff exposure (Bartik) = exogenous shock; regional strategic dependence = cross-sectional moderator (predetermined at baseline). The identification logic is identical.
  3. **TARIFF CAVEAT.** Tomasi uses UNCTAD TRAINS — which Teti (2024) shows has systematic interpolation artifacts. The project uses Teti GTD, which is more accurate. This is an explicit improvement over the Tomasi framework (and over the prior China-firm literature including Brandt et al. 2017, which Tomasi cites).
  4. **The import mechanism finding (Table 10–11) provides the micro-foundation for the project's d_in vs. d_out asymmetry.** If firms with higher probability of importing (= firms with within-block capability access to new products = d_in channels) gain more from tariff cuts, this directly motivates the project's hypothesis: firms with within-block access gain from tariff exposure via input quality/variety channels (d_in), while firms that must jump blocks (d_out) face capability constraints that local institutional frictions exacerbate. The Tomasi import mediation mechanism maps onto d_in as the constrained capability channel.

---

### Cross-paper synthesis (§5a)

**1. The standard empirical design for tariff-productivity at firm level.** Amiti-Konings (2007) establishes the blueprint: (a) construct firm/industry-level tariff exposure as weighted-average upstream or downstream tariffs; (b) estimate TFP via Olley-Pakes or Levinsohn-Petrin-Wooldridge; (c) run two-way FE panel with tariff main effect + importing-firm interaction; (d) use industry-level tariff variation as identification (with political-economy endogeneity tests). Tomasi (2023) adds the province-level moderator × tariff interaction. The project extends this by replacing TFP with d_in/d_out and replacing PCI governance with regional strategic dependence.

**2. The omitted variable problem from Amiti applies to the project.** Excluding the d_in × tariff and d_out × tariff decomposition would conflate the within-block and cross-block responses, producing a biased average effect. The Amiti result (output tariff effect more than doubled when input tariffs excluded) is an exact analog: if the project estimates only a single diversification response without the in/out decomposition, the estimated average effect mixes the capability-constrained d_in response with the capability-unconstrained d_out response, biasing both.

**3. The heterogeneous treatment effects are motivated at two levels.** Amiti: within industry, IMPORTING firms gain 4× more than non-importers from input tariff cuts (12% vs. 3%). Tomasi: within industry, HIGH-GOVERNANCE firms gain more from output tariff cuts (provincial moderator). For the project: (a) WITHIN-BLOCK firms (d_in type) should gain more from tariff exposure if their block capabilities are adjacent to disrupted products; (b) firms in HIGH-STRATEGIC-DEPENDENCE regions should respond DIFFERENTLY to tariff exposure depending on whether their capability blocks are in exposed vs. insulated sectors.

**4. Mechanism asymmetry: input tariffs ≠ export tariffs.** Amiti's mechanism is input-side: cheaper imported inputs → learning, variety, quality effects. The project's treatment is output-side: higher tariffs on exports to foreign destinations → demand destruction for existing product-destination pairs. These are mechanically different. Amiti's result provides the baseline for what tariff-productivity effects look like; it does not directly predict d_in/d_out directions. The capability-reconfiguration prediction must be built from Penrose-Bottazzi-Dosi theory (Batches 4a–4j) rather than extrapolated from Amiti's input channel.

---

## §5b — China Firm Finance/Growth + Event Study Identification (Batch 5b)

*Papers read in full, 2026-06-04*

> **Note on misidentifications.** The file labeled `Nguyen_2010.pdf` is NOT a China firm-level paper — it is Vinh, Epps & Bailey (ICML 2009), the AMI clustering comparison paper, already synthesized in §3c (cited as [69] in Cimini 2022). The file labeled `Sun_2020.pdf` is NOT a China firm-level paper — it is Sun & Abraham (*Journal of Econometrics* 225: 175–199, 2021), the foundational paper on heterogeneous treatment effects in TWFE event studies, which is highly relevant to the project's identification strategy and is synthesized here. Nguyen/Vinh et al. is already covered and not repeated.

---

### Guariglia, Liu & Song (2011) — "Internal finance and growth: Microeconometric evidence on Chinese firms"
*Journal of Development Economics 96: 79–94* — **Chinese NBS panel, financial constraints, and growth by ownership type**

- **Main contribution.** Rationalizes the "Chinese growth puzzle" (fast firm growth despite malfunctioning financial system) using microeconometric evidence: highly productive private firms finance their spectacular asset growth entirely from internally generated cash flow, despite being systematically excluded from bank credit. SOEs are not financially constrained (soft budget constraints); private and foreign firms are. Financial constraints do not cause efficiency losses — constrained high-growth firms actually have higher TFP.

- **Data.** Chinese NBS annual industrial enterprise survey, 2000–2007. All SOEs plus non-SOEs with annual sales ≥ 5 million yuan (~$650,000). After cleaning: 79,841 firms, 499,001 firm-year observations (unbalanced panel, minimum 5 consecutive years). Ownership measured as continuous fraction of paid-in capital (not binary registration code). Key ownership groups: State-owned (6.2%), Foreign (18.3%), Private/legal person/individual (64.9%), Collective (9.2%). **This is the same NBS dataset the project uses.**

- **Model.** Dynamic assets growth model estimated by first-difference GMM (Arellano-Bond):
  > ΔAssetsGrowth_it = α_0 ΔAssetsGrowth_{i,t-1} + α_1 (CF/Assets)_it + year_dummies + industry×year_dummies + ε_it
  Financially constrained firms: α_1 ≈ 1 (one-for-one cash flow → growth). Unconstrained firms: α_1 ≈ 0.

- **Key results.**
  - **SOEs** (col. 1): α_1 = 0.25, insignificant → NOT financially constrained; soft budget constraints (state banks lend regardless of profitability). Mean assets growth = 1.0%; CF/assets = 4.5%; labor productivity = 160.
  - **Foreign firms** (col. 2): α_1 = 1.09***, significant, p(H0: α_1 ≥ 1) = 0.81 → financially constrained via collateral effect; rely on both parent company finance AND domestic credit markets.
  - **Private firms** (col. 3): α_1 = 0.98***, significant, p(H0: α_1 ≥ 1) = 0.95 → most severely financially constrained; cash flow ≈ assets growth (8.3% ≈ 8.5%); self-financed growth.
  - **Collective firms** (col. 4): α_1 = 0.63, insignificant → partially constrained; local government connections provide some soft budget support.

- **Heterogeneity within private firms.** Coastal region + negligible foreign ownership = highest constraints (α_1 = 1.23, p=0.77). Interior region or firms with any foreign participation → lower constraints. Political affiliation insignificant in this context (political favors operate through permits and licenses, not tariffs). **Coastal private Chinese exporters without foreign capital = most financially constrained group — directly the target population for the project's China-US tariff shock analysis.**

- **No efficiency losses from constraints.** Firms with high cash-flow sensitivity (high CFS) AND high growth have higher, not lower, TFP (340.4 vs. 275.5%), higher wage growth (11.5 vs. 8.7%), higher training investment → financial constraints do not force a productivity-investment tradeoff. Rather: HIGH PRODUCTIVITY drives high cash flow, which enables growth despite credit rationing. "The Chinese miracle... may have been made possible by [private firms'] ability to generate vast amounts of internal funds."

- **Mechanism.** Supply schedule: horizontal for SOEs/collective (unlimited cheap bank credit), upward-sloping for private/foreign (standard moral hazard debt premium). CF increase → longer horizontal segment AND flatter upward slope (collateral effect) → one-for-one or slightly-greater-than-one growth-to-CF sensitivity for constrained firms.

- **Robustness.** Holds for: (a) assets net of cash, (b) strict 100% majority ownership definition, (c) fixed investment model (α_1 ≈ 0.36-0.37 for private/foreign), (d) alternative CFS definition (Hovakimian 2009). Results robust to balanced panel and different lag depths.

- **Relevance to project.** Four implications:
  1. **The project uses the same dataset.** NBS industrial enterprise survey 2000-2007 (Guariglia) → project likely extends to 2015. The ownership classification methodology (majority average paid-in capital shares, not registration codes) is directly applicable and accounts for round-tripping FDI.
  2. **SOE vs. private heterogeneity is a pre-specified moderator.** SOEs have soft budget constraints and are shielded from market pressure → likely less responsive to tariff shocks (less incentive to reconfigure capabilities). Private coastal firms are most financially constrained AND most exposed to tariff shocks → maximum capability-reconfiguration pressure. The interaction (SOE × tariff exposure) should be included as a heterogeneity test alongside the RegDependency moderator.
  3. **Financial constraints may interact with d_in/d_out asymmetry.** In-block diversification (d_in) is cheaper (adjacent capabilities, lower search costs) than out-of-block diversification (d_out = capability mismatch, higher fixed costs). For financially constrained private firms, the capability-investment cost of d_out may be prohibitive → under tariff pressure, constrained firms are predicted to concentrate on d_in, while financially healthy firms (SOEs, foreign JVs) have more slack to attempt d_out. This generates a testable ownership × tariff × capability-type interaction.
  4. **TFP is the sufficient statistic for the productivity mechanism.** Guariglia confirms that high TFP enables internal finance accumulation which enables growth. The project does not use TFP as an outcome (it uses d_in/d_out) but TFP should be controlled for as a covariate — high-TFP firms have more capability slack to reconfigure, which could generate positive selection into d_out.

---

### Sun & Abraham (2021) — "Estimating dynamic treatment effects in event studies with heterogeneous treatment effects"
*Journal of Econometrics 225: 175–199* — **TWFE contamination + Interaction-Weighted estimator**

- **Main contribution.** Shows that in event studies with variation in treatment timing (staggered adoption), the standard TWFE coefficient µ_ℓ on the ℓ-th lead/lag indicator is a linear combination of CATTs from ALL cohorts AND ALL relative periods — not just cohort e and period ℓ. Under heterogeneous treatment effects across cohorts, this contamination is non-zero and the weights can be negative (non-convex). Pre-trend tests based on pre-period µ_ℓ are therefore invalid. Proposes the Interaction-Weighted (IW) estimator as the robust alternative.

- **Setup.** Staggered adoption: firm/unit i treated at time E_i (absorption). Cohort e = {i: E_i = e}. Cohort-specific ATT on the treated (CATT): CATT_{e,ℓ} = E[Y_{i,e+ℓ} − Y^∞_{i,e+ℓ} | E_i = e]. The standard TWFE "fully dynamic" spec includes leads and lags {D^ℓ_{i,t}} with µ_ℓ as the estimate. All papers in the Roth (2019) survey use this spec.

- **Decomposition result (Proposition 2).** Under parallel trends + no anticipation:
  > µ_g = Σ_{ℓ∈g, e} ω^g_{e,ℓ} CATT_{e,ℓ}  +  Σ_{ℓ'∉g, e} ω^g_{e,ℓ'} CATT_{e,ℓ'}
  Weights ω^g_{e,ℓ}: (a) sum to 1 for own-period; (b) sum to 0 for other included periods; (c) sum to −1 for excluded periods. Key: weights are non-linear functions of cohort distribution and can be negative → µ_ℓ is NOT a convex average of CATTs, and can fall outside the convex hull of underlying effects.

- **Contamination of pre-trends test (Proposition 3/Section 3.7).** Even under parallel trends + no anticipation, µ_g for pre-period indicators (ℓ < 0) picks up POST-TREATMENT CATTs from other periods. A test of µ_{-ℓ} = 0 cannot accept or reject pretrends without strong assumptions on treatment effects homogeneity. This invalidates the standard pre-trend visualization used by almost all event study papers.

- **IW estimator (Section 4).** Three-step procedure:
  1. Estimate CATT_{e,ℓ} by running the saturated regression: Y_{it} = α_i + λ_t + Σ_{e,ℓ} δ_{e,ℓ} (1{E_i=e} × D^ℓ_{it}) + ε_it. δ_{e,ℓ} is a DID estimator for CATT_{e,ℓ} using pre-period s=e−1 and control cohort = never-treated (or latest-treated).
  2. Estimate cohort shares Pr{E_i=e | E_i ∈ [−ℓ, T−ℓ]} by sample frequencies.
  3. Form ν̂_g = (1/|g|) Σ_{ℓ∈g, e} δ̂_{e,ℓ} × (cohort share weight).
  Result: ν̂_g is by construction a CONVEX AVERAGE of CATT_{e,ℓ∈g} with cohort-share weights; immune to contamination from other periods; consistent for the interpretable weighted average νg.

- **Key diagnostic.** The weights ω^g_{e,ℓ} can be estimated via the auxiliary regression (Equation 13) using Stata package `eventstudyweights`. This allows researchers to visualize which cohorts and which periods contaminate any given µ_ℓ estimate. If weights are near-zero for other periods → contamination small → standard TWFE may be valid. If weights are large and negative → use IW.

- **Comparison with related estimators.** Similar to Callaway-Sant'Anna (2020) in spirit but: (a) uses last cohort as control when no never-treated group; (b) can be cast as a regression; (c) without covariates and with never-treated units, coincides with Callaway-Sant'Anna. Can also use the `did` R package from Callaway-Sant'Anna.

- **Relevance to project.** Four direct implications:
  1. **The project's event study requires IW or equivalent.** The project uses Chinese firm-level data 2000–2015 with tariff shocks that hit different firms at different times (US-China tariffs 2018-2019, and earlier bilateral tariff changes). With heterogeneous treatment timing → staggered adoption setting → standard TWFE event study is contaminated if treatment effects differ across tariff-exposure cohorts (which they will, since early vs. late-shock firms face different competitive environments).
  2. **Pre-trend plots cannot be based on standard TWFE leads.** The research spec mentions event-study as the identification strategy. If the pre-trend test uses standard µ_{-ℓ} from TWFE, it is formally invalid (Proposition 3). The pre-period parallel trends test must be conducted using IW estimates or Callaway-Sant'Anna.
  3. **CATT decomposition reveals heterogeneous effects.** IW provides estimates CATT_{e,ℓ} for each cohort (tariff-exposure group). This allows testing whether high-exposure cohorts (high Bartik × tariff) respond differently to the shock than low-exposure cohorts — directly addressing the heterogeneous treatment effect concern and providing richer evidence on capability reconfiguration dynamics.
  4. **Adão + Sun-Abraham are COMPLEMENTARY.** The Adão (2019) shift-share inference (cited in research spec) addresses cross-sectional clustering: firms in the same industries share correlated shocks, so industry-cluster-robust SE understate true sampling uncertainty. Sun-Abraham addresses the temporal panel dimension: coefficients from different leads/lags contaminate each other when cohorts differ. Both corrections are needed for the full event study to be valid.

---

### Cross-paper synthesis (§5b)

**1. The NBS dataset is the project's actual data.** Guariglia (2011) is the canonical paper using the same NBS industrial enterprise survey, confirming that: (a) the dataset covers all firms ≥ 5M yuan sales including privately owned manufacturers; (b) ownership is measured continuously by paid-in capital fractions; (c) SOEs and private firms behave fundamentally differently in growth dynamics. These choices should be carried into the project's data construction directly.

**2. Ownership × tariff × capability-type creates a 3-way interaction hypothesis.** From Guariglia: SOEs are not financially constrained (soft budget) → less responsive to market pressure; private coastal firms most constrained → most pressure to reconfigure under tariff shock. From EFC theory (Batches 2-4): d_in is cheaper than d_out (adjacent vs. novel capabilities). Prediction: financially constrained private firms under tariff shock → d_in (accessible, cheap); SOEs → less response overall; firms with access to finance (foreign JV, politically connected) → potentially d_out. This 3-way interaction should be a pre-registered secondary hypothesis.

**3. The event study specification requires IW + Adão simultaneously.** For the project's causal claims to be credible: (a) construct Bartik shift-share tariff exposure per firm as the treatment; (b) test parallel trends using IW pre-period estimates (not standard TWFE leads); (c) estimate dynamic effects using IW estimator per cohort (tariff-exposure tercile); (d) inference using Adão shift-share variance (not cluster-robust SE). This four-step identification strategy is more demanding than standard practice but addresses both contamination sources simultaneously.

**4. Sun-Abraham aligns with Adão on the fundamental critique of TWFE.** Both papers show that standard TWFE produces estimates that are linear combinations of treatment effects with potentially negative weights. Adão addresses this via the "leave-one-out" estimator; Sun-Abraham via the IW estimator. For the project: use IW for event-study dynamic paths + Adão-corrected SE for cross-sectional inference. The two approaches are not in conflict — one corrects for the *what is estimated* problem (IW), the other for the *how variable is it* problem (Adão).

---

## §5c — Export Volatility, Diversification, and Capability Shocks (Batch 5c)

*Papers read in full, 2026-06-05*

---

### Vannoorenberghe, Wang & Yu (2016) — "Volatility and diversification of exports: Firm-level theory and evidence"
*European Economic Review 89: 216–247* — **Firm-level export diversification × volatility: size-conditional reversal**

- **Main contribution.** Documents a counter-intuitive fact using Chinese customs data: among SMALL exporters, more diversified destinations → MORE volatile exports. Among LARGE exporters, the standard portfolio-theory result holds (more diversification → less volatility). The paper develops a theoretical model with fixed costs of export per destination and short-run demand shocks, generating "occasional exports" to some markets. The composition effect (occasional exports are intrinsically more volatile than continuous exports) dominates the diversification effect for small firms.

- **Data.** Chinese Customs Trade Statistics (CCTS) 2000–2006, full universe of exporters. Matched to NBS Annual Survey (ASIF) for balance sheet controls. Sample: 23,822 continuous exporters (all 7 years); 8,387 matched with ASIF. Same Chinese customs + NBS data combination used in the project.

- **Key empirical finding.** Baseline specification (Table 3):
  > Volatility_j = β_0 + β_1 Herf_j + β_2 Size_j + β_3 (Herf_j × Size_j) + controls + province/industry/ownership FE
  - β_1 (Herf) = −0.54*** (CCTS): higher concentration → LOWER volatility for small exporters
  - β_2 (Exports) = −0.28***: larger exports → less volatile
  - β_3 (Herf × Exports) = +0.045***: interaction positive → for large exporters, the negative Herf effect is reversed
  - Break-even firm size (marginal Herf effect = 0): log exports ≈ 11.87 (CCTS) / 14.74 (matched). Below this: diversification raises volatility. Above: diversification lowers volatility.
  - Product diversification (Herf_prod): same qualitative pattern — β_1 < 0, β_3 > 0 — confirming that the mechanism operates equally across product and destination dimensions.

- **Model mechanism.** Two markets, fixed cost f per market per year, idiosyncratic demand shocks (s̄ > s). Firm j continuously exports to market i iff λ_ji × s > f. Exports occasionally to i' iff λ_ji' × s̄ > f > λ_ji' × s. 
  - Continuous exports: VAR_ji = 2μ (bounded by demand shock coefficient of variation μ < 1)
  - Occasional exports: VAR_ji' = 2 (maximum variance: firm sells in good years, zero in bad years)
  - Total volatility V^O_j = 2μ × Herf_j + 2(1−μ) × ω_ji'^2
  The second term (composition effect) is increasing in ω_ji' (share of sales to the occasional market). For small firms, ω_ji' is large relative to total sales → composition effect dominates diversification effect → dV/dHerf < 0 (lower Herf = more diversification = higher volatility).

- **Mechanism validation.** Contribution of extensive margin (entry/exit of destinations) to volatility is DECREASING in Herfindahl concentration and INCREASING with diversification — especially for small firms (Fig. 5). Firms exporting to a market for only 1-3 years account for the majority of the volatility contribution. Larger firms export to each destination for longer (median 3 years unweighted, 6.5 years export-value-weighted) → occasional exports less prevalent.

- **Relevance to project.** Five direct implications:
  1. **d_out is an "occasional export" to a new capability block.** When a Chinese firm jumps to a new block (d_out), it is, by definition, entering territory where it has partial capabilities — the firm-block match is imperfect. By the Vannoorenberghe model, this is exactly the "occasional export" scenario: the firm will export to new-block products only when demand shocks are favorable enough to cover the "capability development cost" (analog of fixed cost f). PREDICTION: d_out moves generate MORE export volatility for small/low-capability firms, and this volatility decreases as the firm's total export scale increases.
  2. **Tariff shocks are negative demand shocks that eliminate occasional markets.** A tariff shock (τ_pdt ↑) reduces ζ_jit below the threshold for occasional destinations. Firms drop those markets from their export portfolio. Small firms who were diversifying via occasional d_out moves are forced to retrench; large firms with persistent export relationships survive the shock. This directly predicts HETEROGENEOUS RESPONSES: tariff shocks cause small Chinese firms to REDUCE d_out (destination diversification collapses to core markets) while large firms absorb the shock via margin compression.
  3. **The Herfindahl × Size interaction is the correct specification for testing diversification effects.** In the project's panel regression of d_in/d_out on tariff exposure, an interaction with firm size (or capability fitness) should be included. Without this interaction, the average diversification effect confounds opposite responses by small and large firms.
  4. **Product diversification mirrors destination diversification.** The paper shows (Table 3, cols 4, 8) that the same sign pattern holds for product Herfindahl × Size. This validates the use of BRIM-based product-block diversification (d_in/d_out) as the outcome variable — the Vannoorenberghe mechanism operates in both dimensions simultaneously.
  5. **"Change in number of destinations" controls.** The paper uses ΔN_destinations as a control (coefficient −0.016***) to avoid confounding the Herfindahl effect with secular destination expansion during China's export boom. The project should include ΔN_products per year as a control variable in regressions, to separate the extensive margin expansion of the export basket from the intensive capability reconfiguration captured by d_in/d_out.

---

### Barbieri, Capoani, Cattaruzzo & Corò (2024) — "Export diversification dimensions and performance: Analysis and industrial policy insights from Italian territories over Covid-19 shocks"
*Socio-Economic Planning Sciences 94: 101923* — **Sectoral vs. geographical diversification; capabilities dual-lens**

- **Main contribution.** Proposes two novel HHI-based diversification metrics for Italian provinces (99 NUTS-3, 2017–2021, cross-sectional) that separately measure productive capabilities (sectoral diversification) and geoeconomic capabilities (geographical diversification). Shows that sectoral diversification predicts export intensity but NOT stability during Covid-19; geographical diversification mildly predicts stability; EU market exposure is the strongest stabilizer. Industry concentration raises instability. Institutional quality boosts both intensity and stability.

- **Metrics.**
  - Sectoral diversification_i = N_sectors_3dig_i / HHI_2dig_i (ratio of breadth to within-macro-sector concentration)
  - Geographical diversification_i = N_countries_i / HHI_macroareas_i (ratio of country reach to continental concentration)
  Both metrics integrate related-variety logic: they count breadth at the fine level while normalizing by concentration at the coarse level.

- **Key findings.** (Tables 3, 4, 5):
  - Sectoral diversification: β = +0.285*** (intensity); insignificant for instability.
  - Geographical diversification: β = +0.605*** (intensity); mild negative for instability (−0.044** in some specs).
  - EU exposure: β = −0.856*** on instability → strongest stabilizer. Other macro-areas not significant.
  - Industry concentration (C3): β = −0.379*** (intensity); β = +0.321*** (instability).
  - Institutional quality (IQI): β = +1.225/1.297*** (intensity); β = −0.447/0.660*** (instability).
  - Sectoral and geographical diversification are positively correlated (ρ = 0.64): territories diversified in products are also diversified in destinations. The link holds most strongly for highest/lowest export intensity quartiles (Fig. 4) and highest stability quartiles (Fig. 5).

- **Conceptual framework.** Sectoral diversification = proxy for PRODUCTIVE CAPABILITIES (can produce varied goods; diverse skill base; recombination potential). Geographical diversification = proxy for GEOECONOMIC CAPABILITIES (established trade networks; ability to navigate diverse markets; diplomatic-commercial reach). This directly maps onto the d_in / d_out dual-capability structure: d_in = within-block product diversification = productive capabilities; d_out = cross-block product entries spanning diverse destinations = geoeconomic capabilities.

- **Italy North-South divide.** Northern provinces (Milan, Bologna, Torino) are top-right (high both dimensions); Southern and island provinces are bottom-left (low both). NE regions most intense AND most stable. This parallels China's coastal/interior divide in Guariglia (§5b) and in the project's regional strategic dependence moderator.

- **Covid as exogenous shock.** The 2020 Covid-19 shock hits provinces differently based on their diversification structures, providing a natural experiment analogous to the US-China tariff shock. The EU anchoring result — EU-exposed provinces more stable during Covid — maps onto the project's hypothesis: firms integrated into stable institutional trade networks (e.g., low-tariff, high-mutual-dependence partners) are more resilient to shocks.

- **Relevance to project.** Three direct implications:
  1. **Productive capabilities (d_in) → intensity; geoeconomic capabilities (d_out) → stability.** Barbieri's result (sectoral diversification → intensity, not stability; geographical diversification → stability, not intensity) directly predicts that in the Chinese firm panel: d_in (product diversification within block = productive capability accumulation) should predict EXPORT LEVEL GROWTH, while d_out (destination diversification across blocks) should predict EXPORT STABILITY UNDER SHOCKS. Testing these two predictions requires separate outcome variables: export value level and export value coefficient of variation.
  2. **EU exposure = anchor for stability.** For Chinese exporters, the analog is a stable high-income, low-tariff destination (pre-shock EU, stable ASEAN partners, etc.). Firms with concentrated exposure to US/high-tariff destinations (high ExpDep toward tariff-imposing countries) → more fragile. This directly motivates the project's regional strategic dependence moderator: high-dependence regions are the "low EU-exposure" analog.
  3. **Concentration × stability inversion.** Barbieri confirms (C3 → instability) that firm-level concentration of export within provinces generates shock fragility. For the project: within-block concentration (firm's d_in portfolio concentrated on few core products) generates fragility to block-level shocks; cross-block diversification (d_out) generates resilience but only if the new blocks are stable (geoeconomic capabilities reach stable markets).

---

### Cross-paper synthesis (§5c)

**1. The size-conditional reversal is a key moderator for all diversification-volatility effects.** Vannoorenberghe establishes that diversification raises volatility for small exporters and lowers it for large exporters. For the project: the effect of d_out on firm performance under tariff shocks is SIZE-CONDITIONAL. Small Chinese firms attempting d_out under tariff pressure face higher export volatility; large firms benefit from d_out's shock-insulation. The Frenken (§2d) result (unrelated variety = UV → shock insulation) and the Vannoorenberghe result are reconciled: UV reduces shock sensitivity at the aggregate but raises volatility at the micro-level for small exporters. The project must include a firm-size × d_out interaction in its main regressions.

**2. Sectoral d_in → growth; geographical d_out → stability — the Barbieri decomposition.** Barbieri separates the two dimensions empirically for Italian provinces: sectoral (d_in analog) → export intensity; geographical (d_out analog) → stability. This is the exact dual-outcome hypothesis the project needs to test: h1: d_in → export expansion; h2: d_out → export resilience under tariff shocks. These are distinct testable predictions requiring separate dependent variables.

**3. Tariff shocks collapse occasional exports first.** Vannoorenberghe's model predicts that demand shocks eliminate "occasional" markets (those below the fixed cost threshold). For the project's Chinese firms: a US tariff shock on product p eliminates the firm-p-US export flow first (the occasional US market). This causes: (a) apparent d_out REDUCTION (the firm retreats to its core block); (b) apparent d_in INCREASE (the firm deepens within-block capability as a substitute strategy). The tariff shock thus generates an endogenous d_in/d_out composition shift even without any capability reconfiguration — this is a MEASUREMENT CONCERN: the project must distinguish capability-driven diversification (genuine d_in/d_out moves) from demand-shock-driven portfolio pruning. Controlling for the change in number of destinations (Vannoorenberghe's ΔN_dest) and using the predetermined BRIM partition (ADR-0001) as the measurement benchmark addresses this concern.

**4. Institutional quality is the missing link between diversification and performance.** Both papers — Barbieri (Italian provinces) and Tomasi §5a (Vietnamese firms) — find that institutional quality amplifies the diversification-to-performance link. For the project, the regional strategic dependence (ExpDep) operates as a negative institutional moderator: high strategic dependence = low institutional insulation from external shocks = attenuated capability-reconfiguration gains from tariff exposure. The moderator works through the same channel as Tomasi's land/legal institutions: it limits firms' ability to exploit new capability opportunities opened by the tariff-induced shock.

---

## §5d — Competition, Innovation, and Step-by-Step Capability Accumulation (Batch 5d)

*Papers read in full, 2026-06-05*

---

### Aghion, Harris, Howitt & Vickers (2001) — "Competition, Imitation and Growth with Step-by-Step Innovation"
*Review of Economic Studies 68: 467–492* — **Theoretical foundation of the escape-competition effect**

- **Main contribution.** Extends Schumpeterian endogenous growth theory to allow step-by-step innovations by incumbent duopolists. Shows that product market competition (PMC) USUALLY raises growth — the escape-competition effect (neck-and-neck firms innovate to escape competition) dominates the Schumpeterian appropriability effect (competition destroys post-innovation rents) for most parameter values. Imitation is inverse-U shaped in growth: a little imitation raises growth (composition effect: more neck-and-neck competition) while too much destroys incentives.

- **Model structure.** Continuum of industries, each a Bertrand duopoly. Firms innovate step-by-step (laggard cannot leapfrog leader; must first catch up, then compete for the lead). R&D cost ψ(x) = βx²/2; imitation parameter h (ease of follower catch-up). Industry state: technological gap n ≥ 0 (neck-and-neck = n=0; leader/follower = n≥1). PMC parameterized by product substitutability α ∈ [0,1]: at α=0, firms earn identical profits regardless of technology → no incentive to innovate; at α=1, winner-take-all competition. Key profit function property: for neck-and-neck firms, incremental profit from innovating (Δπ₀ = π(y,α) − π(1,α)) is strictly increasing in α → escape-competition effect is always active.

- **Growth rate formula.** g = (2μ₀x₀ + Σₖ₌₁ μₖxₖ) ln γ, where μ₀ = fraction of neck-and-neck industries, x₀ = R&D effort of neck-and-neck firm, xₖ = leader's R&D in gap-k industry. Growth depends critically on μ₀ (the composition effect) and x₀ (the escape-competition effect). Both are affected by PMC in opposite directions: ∂x₀/∂α > 0 (escape-competition) but ∂μ₀/∂α < 0 (higher PMC → industries leave neck-and-neck state faster, reducing μ₀).

- **Key results.**
  1. **Growth always increases initially with competition.** At α=0, no incentive to innovate → g=0. Raising α above zero creates escape-competition motive → g>0. This is the anti-Schumpeterian finding.
  2. **Effect of PMC on growth: usually monotonically positive; sometimes inverted-U.** For most parameter values, the escape-competition effect dominates. The inverted-U appears when γ (innovation size) is very large — leaders stop innovating (already at maximum profit), and further competition discourages laggard catch-up.
  3. **Imitation is inverse-U shaped.** At h=0: no composition effect → g suboptimal. A little h raises g by inducing more neck-and-neck competition (composition effect). Too much h: destroys incremental rents → R&D effort x₀ → 0 → g → 0.
  4. **Policy complementarity.** Anti-trust (raising PMC) and patent policy (reducing h) are COMPLEMENTARY: the maximal growth rate is achieved by maximal PMC AND a moderate positive level of patent protection. This is the opposite of the standard Schumpeterian prediction.

- **Relevance to project.** Three direct implications:
  1. **Step-by-step capability accumulation is the correct innovation model for Chinese firms.** A Chinese firm cannot jump directly from having zero capabilities in a new block (d_out territory) to being a frontier producer — it must first accumulate within-block capabilities (d_in, moving up the nested hierarchy established in §2e/§3b). The step-by-step constraint provides the micro-foundation for why d_in occurs before d_out in the project's capability ladder (Coad-Mathew-Pugliese §4g, within-block degree ranking).
  2. **Tariff shocks as competition shocks.** A tariff shock on product p in destination d is equivalent to an increase in PMC that the Chinese firm faces from foreign competitors (the destination market becomes more competitive for the tariff-imposing country's domestic producers, and LESS accessible for the Chinese exporter — demand destruction). This is not the same as standard PMC in the Aghion model, but the mechanism is analogous: the exporter's incremental rents from maintaining a capability in the tariffed product/market are REDUCED → Schumpeterian effect suppresses capability investment in that direction. However, if the firm is neck-and-neck with the frontier in its capability block, the escape-competition effect may still be operative: the firm innovates more vigorously within the block to maintain competitive position. The net effect depends on whether the firm is a frontier firm or a laggard within its block.
  3. **Composition effect in the project.** Analogously to Aghion's industry composition effect (fraction of neck-and-neck vs. unleveled industries), the project's capability partition has a composition across blocks: some firms are "neck-and-neck" with the capability frontier (high within-block fitness rank) and some are "laggards" (low within-block fitness rank). Tariff shocks that reduce returns to existing products will differentially affect these two groups. This motivates including the firm's within-block fitness rank as a moderator of the tariff-to-d_in/d_out response.

---

### Aghion, Bloom, Blundell, Griffith & Howitt (2005) — "Competition and Innovation: An Inverted-U Relationship"
*Quarterly Journal of Economics 120(2): 701–728* — **Empirical inverted-U + two-state closed-form model**

- **Main contribution.** Provides the first empirical evidence of an inverted-U relationship between competition and innovation using UK panel data (311 firms, 17 2-digit SIC codes, 1973–1994). Develops a two-state closed-form version of the Aghion et al. (2001) model that derives the inverted-U analytically and delivers two additional testable predictions: (P4) technological gap increases with competition; (P5) the inverted-U is steeper in neck-and-neck industries. Both predictions are confirmed.

- **Empirical specification.** Dependent: citation-weighted patents per industry-year. Competition: Lerner index c_{jt} = 1 − (1/N_{jt}) Σᵢ π_{it}/sales_{it}. Specification: log E[p_{jt}] = g(c_{jt}) + x'_{jt}β (Poisson with industry + year FE; nonparametric g(·) approximated by exponential quadratic). IV: Thatcher privatizations, EU Single Market Programme (1988, differential industry impacts), Monopoly and Mergers Commission actions.

- **Main result (Table 1, column 2).** c_{jt}: +387.46*** ; c²_{jt}: −204.55*** (Poisson with industry + year FE). Both significant. Inverted-U confirmed, peak near median Lerner value (0.95) — the data span both the increasing and decreasing portions. Robust to IV specification (column 4) and 5-year averages (column 3).

- **Two-state theoretical model.** Maximum gap m=1 (automatic spillovers prevent leaders from building more than 1-step leads). Two types of sectors:
  - **Leveled/neck-and-neck** (m=0): π₀ = εʼπ₁, competition parameter Δ = 1 − ε. R&D: n₀ = √(h² + 2Δπ₁) − h → INCREASES with Δ (escape-competition effect)
  - **Unleveled** (m=1): leader earns π₁ = 1 − γ⁻¹; laggard earns π₋₁ = 0. Leader does no R&D (automatic catch-up). Laggard: n₋₁ = √(h² + n₀² + 2π₁) − h − n₀ → DECREASES with Δ (Schumpeterian effect)
  - Aggregate innovation rate ν(n₀) = 4n₀(n₋₁ + h)/(2n₀ + n₋₁ + h): inverted-U in n₀ (proxy for competition) with peak at x̃ = √((h² + 2π₁)/3). Peak is INTERIOR when x̃ ∈ (x̲, x̄).

- **Prediction 4 confirmed (Table 3, cols 1-2).** Technology gap G = μ₁ increases with competition: coefficient ≈ 0.94−2.86*** → more competition → more industries unleveled → more laggard/leader asymmetry. This was COUNTERINTUITIVE: static selection would predict competition reduces TFP spread (exits low-TFP firms). Instead, escape-competition INCREASES spread by inducing frontier firms to innovate more, widening the gap.

- **Prediction 5 confirmed (Table 3, cols 3-4; Figure III).** Neck-and-neck industries (below-median technology gap) show steeper inverted-U: the increase in innovation with competition is larger and the peak occurs at higher competition. Interaction terms (Competition × Technology gap, Competition² × Technology gap) jointly significant at p<0.02.

- **Relevance to project.** Four direct implications:
  1. **The inverted-U maps onto d_in response to competition intensity.** For the project: the tariff shock reduces market access (effective demand for the firm's products in destination d). This is an increase in "competition" for surviving in destination d. For firms near the capability frontier of their block (neck-and-neck): escape-competition effect → d_in increases (firms innovate within block to maintain position). For laggard firms in their block: Schumpeterian effect → d_in decreases (reduced rents suppress capability investment). At very high tariff levels, even frontier firms face the Schumpeterian effect → d_in decreases. Result: the relationship between tariff intensity and d_in is INVERTED-U shaped at the firm level, with the peak depending on the firm's within-block fitness position.
  2. **Technological gap as heterogeneity moderator.** Aghion et al. measure technology gap as proportional distance to frontier TFP. For the project: within-block fitness rank (from the BRIM-based d_in hierarchy, §3b Solé-Ribalta) is the direct analog. Low-within-block-rank (laggard) × high tariff = Schumpeterian suppression of d_in. High-within-block-rank (frontier, neck-and-neck) × moderate tariff = escape-competition amplification of d_in. The fitness rank × tariff interaction should be included in the project's main specification.
  3. **EU Single Market Programme 1988 as an identification parallel.** The paper instruments competition with discrete policy shocks (SMP, MMC actions, privatizations) that vary by industry and year. For the project: Bartik shift-share tariff exposure is the equivalent instrument — it uses predetermined product-destination weights to isolate exogenous variation in tariff pressure. The Aghion IV strategy provides a direct methodological precedent for the Bartik approach in the Chinese context.
  4. **Patent/imitation complementarity → regional spillover implications.** Aghion finds that anti-trust (competition) and patent (moderate imitation) policy are complementary. For the project: the escape-competition effect on d_in is strongest where IP protection is moderate (not zero, not infinite). Chinese industrial regions with strong technological capabilities AND moderate knowledge spillovers (e.g., Yangtze River Delta vs. pure export-assembly zones) should show stronger capability reconfiguration responses to tariff shocks. This motivates including a regional spillover-intensity proxy in the RegDependency moderator.

---

### Cross-paper synthesis (§5d)

**1. Step-by-step capability accumulation provides the micro-foundation for the d_in/d_out ladder.** Aghion (2001) establishes that laggards must first catch up (d_in analog) before they can compete for the lead (d_out analog). This is the formal basis for the empirical finding in Coad-Mathew-Pugliese (§4g) that capability accumulation follows a ladder structure. For the project: firms must achieve sufficient within-block capability (rise in the within-block nested hierarchy, §3b Solé-Ribalta I-function) before d_out becomes feasible. Tariff shocks that disrupt this ladder impose disproportionate costs on firms mid-climb.

**2. The escape-competition effect creates an asymmetry between frontier and laggard firms.** Aghion (2005) Proposition 5: the escape-competition effect is steeper for neck-and-neck industries. For the project: Chinese firms that are near the capability frontier of their block (high within-block fitness rank) respond to tariff shocks by intensifying d_in (escape-competition motive). Firms that are laggards within their block respond to tariff shocks by REDUCING d_in (Schumpeterian suppression of catch-up incentives). This generates SIGN REVERSAL in the tariff-to-d_in effect depending on within-block fitness position — a critical source of heterogeneous treatment effects that must be tested empirically.

**3. The inverted-U links to Vannoorenberghe's size-conditional reversal.** Vannoorenberghe (§5c) shows that the diversification-volatility relationship is size-conditional (negative for small, positive for large). Aghion shows that the competition-innovation relationship is frontier-conditional (positive for neck-and-neck, negative for laggards). Both results have the same structure: the effect of competitive pressure (on volatility or innovation) REVERSES based on the firm's position in the capability/size distribution. For the project: tariff shock × within-block-fitness interaction should replicate both stylized facts simultaneously.

**4. The composition effect of PMC matters as much as the direct effect.** Aghion (2001): PMC raises x₀ (neck-and-neck R&D) but reduces μ₀ (fraction of neck-and-neck industries). The composition effect (change in distribution across industry types) can dominate. For the project's panel: the tariff shock will not only affect each firm's d_in/d_out response directly but will also change the DISTRIBUTION of firms across within-block fitness ranks (firms that fail to reconfigure exit blocks; new entrants appear; the blocks themselves may shift). This dynamic composition effect is part of the "temporal-coupled BRIM" motivation (ADR-0001) — the block partition must be updated to track these movements.

---

## §5e — International Trade, Innovation, and Endogenous Growth (Batch 5e)

*Papers read in full, 2026-06-05*

---

### Akcigit & Melitz (2022) — "International Trade and Innovation"
*BFI Working Paper 2022-02; Handbook of International Economics Vol. 5* — **Unified framework: market size + business stealing + escape competition**

- **Main contribution.** Handbook chapter (Gopinath-Helpman-Rogoff Handbook of International Economics, Vol. 5) reviewing the literature on globalization and innovation and developing a unified theoretical model combining three key mechanisms: (1) market size effect (export access → larger market → more innovation); (2) business stealing effect (import competition → reduced monopoly rents → less innovation); (3) escape competition (neck-and-neck incumbents respond to competition with MORE innovation). Reviews empirical evidence separately on export market and import competition channels.

- **Baseline model (quality ladder, myopic).** Final good Y = (L^β/(1−β)) ∫₀^N q_j^β k_j^{1−β} dj. Each intermediate j is a monopolist earning π_j = ΥLq_j (quality-proportional profits, where Υ ≡ [(1−β)/η]^{(1−β)/β} · β). Incumbent's innovation choice: maximize E[π_j] − θq_j x_j²:
  > x_j = (1 − z_j) · λΥL / (2θ)   [Eq. 6]
  where z_j = exogenous entry probability (business stealing channel), λ = innovation step, L = market size.
  
  Key results:
  - **Result 2** (market size): ∂x_j/∂L > 0 — innovation increases with market size
  - **Result 3** (business stealing): ∂x_j/∂z_j < 0 — entry/competition reduces innovation
  - Innovation independent of quality q_j → Gibrat's law (consistent with §4f Coad 2009)

- **Export market selection.** Exporter's effective market size L = L_D + τ^{−(1−β)/β} L_F > L_D. Trade liberalization (τ → τ') induces: (a) existing exporters innovate more by Δx^{exp}_j = (1−z_j)Υλ L_F (τ'^{−(1−β)/β} − τ^{−(1−β)/β}) / (2θ); (b) new exporters innovate even MORE than existing exporters (Δx^{new}_j > Δx^{exp}_j). This is because new exporters have the largest gap between pre-export and post-export market size. For the REVERSE experiment (tariff shock INCREASES τ for Chinese exporters): existing exporters lose market size → innovate LESS; some firms DROP OUT of exporting.

- **Escape competition (neck-and-neck extension).** Neck-and-neck firm f=0 with N rivals all producing at quality q₀: expected next-period profit only if firm's own innovation succeeds AND no rival succeeds AND no entry:
  > x₀^N (1 − x₀)^N = (1 − z) · (1 + λ) · ΥL / (2θ)   [Eq. 13]
  vs. single leader: x₁ = (1 − z) · λΥL / (2θ). The escape-competition "kick" is the +1 added to λ: neck-and-neck firms escape zero profits (current π₀ = 0) by innovating → incremental gain is (1 + λ) times the post-innovation profit, not just λ. When λ → 0, single leader innovation → 0 but neck-and-neck innovation remains positive.

- **Dynamic model.** Value function V(q_j) = νq_j (linear in quality). Innovation effort:
  > x_j = (z_j + r)/λ − √[(z_j + r)/λ]² − ΥL/θ
  Same comparative statics as myopic case. Endogenous entry under constant CES eliminates market size channel (Sutton result); variable markups or oligopoly reinstate it.

- **Empirical evidence synthesis (§4).** 
  - Export market access → innovation: UNAMBIGUOUSLY POSITIVE across all studies. Coelli et al. (2021): global tariff decline in 1990s explains 7% of global patenting. CUSFTA: +6% within-firm productivity (Lileeva-Trefler 2010). France: patenting increases with export market access, concentrated in more productive exporters (Aghion et al. 2019).
  - Import competition → innovation: MIXED in developed countries; POSITIVE in developing countries.
    - US: Autor et al. (2020): Chinese import competition → NEGATIVE patenting; mainly less profitable, less capital-intensive US firms. Above-median firms: no significant effect.
    - Europe: Bloom et al. (2016): Chinese imports → POSITIVE innovation response. European firms diversify into more differentiated products.
    - China: Bombardini et al. (2018): Chinese firms facing WTO competition → positive patenting, concentrated in MORE PRODUCTIVE firms.
    - Aghion et al. (2021, France): negative innovation only for firms that DON'T use imported Chinese intermediates.
  - Key explanation for divergence: heterogeneous responses depend on firm's characteristics. Neck-and-neck frontier firms → escape competition (+). Laggard firms with already-low profits → Schumpeterian profit destruction (−).
  - Product vs. process innovation: positive import competition response concentrated in product innovation (more differentiated products) — Hombert & Matray (2018, US), Fieler & Harrison (2018, China).

- **Tariff shock as negative market size + positive competition.** A tariff increase on Chinese exports to destination d operates via TWO opposing channels simultaneously: (a) NEGATIVE market size: reduces L_F accessible to Chinese exporters → less innovation/capability accumulation; (b) AMBIGUOUS competition: higher foreign tariffs reduce Chinese firms' revenues → depends on whether firms are neck-and-neck (escape-competition → more innovation) or laggards (Schumpeterian → less). For products where Chinese firms are competitive and face frontier foreign rivals in destination d: competition channel can be positive. For products where Chinese firms are already dominant: primarily market size destruction.

- **Protectionist tariffs generate dynamic welfare losses.** Key result from Akcigit et al. (2018): tariff increase → static benefit (protection) + TWO dynamic costs: (i) inferior domestic goods replace quality imports → aggregate productivity loss; (ii) reduces escape-competition incentive for domestic firms → LESS innovation in long run. Dynamic costs eventually dominate. For the project: sustained tariff exposure (US-China 2018+) should generate LONG-RUN capability stagnation in heavily-exposed sectors, not just short-run diversification responses.

- **Relevance to project.** Four direct implications:
  1. **Export market size is the primary positive driver of d_in.** Chinese firms export to multiple destinations; the capability accumulation captured by d_in is partly motivated by accessing larger export markets (product quality upgrading to serve diverse markets). Tariff shocks that reduce accessible market size → direct suppression of d_in via market-size channel. Control variable: firm's pre-shock export market size and number of destinations should be included in regressions.
  2. **New entrants to export blocks (d_out) respond most strongly to liberalization.** By analogy: firms that first enter a new capability block (d_out move) respond most to tariff shocks in THAT block because they have the largest gap between pre-entry and post-entry capability value. This is the dynamic version of the "new exporters innovate most" result: the first d_out move into a block generates the strongest incentive to subsequently d_in (within that new block). Testing this requires tracking firms' sequential block-entry events.
  3. **Sectoral heterogeneity in competition channel direction.** Chinese firms in sectors where they are globally competitive (neck-and-neck with frontier) → positive escape-competition from tariff shocks → MORE d_in. Firms in sectors where they are laggards facing advanced-country competition → Schumpeterian effect → LESS d_in. The project's BRIM-based within-block fitness rank directly identifies which Chinese firms are neck-and-neck vs. laggard within each capability block.
  4. **Intermediate input imports vs. output market competition must be separated.** Aghion et al. (2021) show that French firms facing Chinese competition respond NEGATIVELY only if they don't use Chinese inputs. For Chinese firms: firms that IMPORT inputs (via d_out into input-sourcing capability blocks) have different innovation dynamics than firms facing competition. The project should distinguish d_out UPWARD (entering higher-complexity blocks) from d_out DOWNWARD (sourcing inputs from lower-complexity blocks).

---

### Rivera-Batiz & Romer (1991) — "Economic Integration and Endogenous Growth"
*Quarterly Journal of Economics 106(2): 531–555* — **Trade in goods vs. flows of ideas: permanent growth effects**

- **Main contribution.** Foundational paper in endogenous growth theory with open-economy extensions. Shows that economic integration (trade in goods and/or flows of ideas) can generate a PERMANENT increase in the worldwide growth rate through scale effects in the R&D sector. The direction of the growth effect depends critically on the specification of the R&D technology. Key insight: integration raises growth permanently if and only if it increases the effective scale of the GROWTH ENGINE (the equation generating new designs).

- **Two R&D specifications.**
  - **Knowledge-driven (KD):** Ȧ = δH_A·A. New designs require human capital and access to existing knowledge stock A. Growth rate: g = (δH − Aρ)/(Aσ + 1) [Eq. 9] — linear in H. Knowledge is a non-rival public good available to all researchers.
  - **Lab equipment (LE):** Ȧ = B·H^α·L^β·(K/A)^{1−α−β}·A^{α+β}. New designs require the same physical inputs as manufacturing (no knowledge spillovers). Growth rate: g = (FH^αL^β − ρ)/σ [Eq. 10] — function of H AND L. Price of patent is fixed: P_A = 1/B.

- **Key results on integration and growth.**
  1. **KD model: Trade in goods has NO permanent growth effect; flows of ideas DO.** Trade in goods increases the market for each patent (doubles profits) but this is exactly offset by the increased marginal product of human capital in manufacturing → no reallocation of H_A into research → no growth effect (level effect only). But allowing flows of ideas doubles the effective research productivity parameter δ (research in each country benefits from the full global knowledge stock A + A*) → shifts the r^{technology} curve upward → permanently higher g. Algebraically: g increases from (δH − Aρ)/(Aσ+1) to (2δH − Aρ)/(Aσ+1) when ideas flow freely.
  2. **LE model: Trade in goods DOES permanently raise growth (same as full integration); flows of ideas add nothing.** Trade in goods doubles the patent value (larger market for each design). Since P_A = 1/B is fixed by technology, the interest rate must increase (by factor 2^{α+β}). Higher r → higher savings → faster capital accumulation → faster growth. This is the same growth rate as if the two economies fully merged (substituting 2H and 2L into Eq. 10). Ideas per se have no direct productive value in LE model, so their flows add no growth.
  3. **General principle.** Integration raises growth permanently iff it increases the effective scale in the sector producing new designs. In KD: needs idea flows (designs are the sector). In LE: goods trade suffices (research uses the same inputs as manufacturing, so expanding the goods market = expanding the research sector).

- **Scale effects and welfare.** Both models have too little innovation relative to the social optimum (positive externality from new designs on future research). Integration brings the economy closer to the social optimum by internalizing the scale of the research sector. Restricting trade (tariffs) between similar developed economies is likely welfare-reducing through permanent growth effects.

- **Limitation: symmetric economies.** The analysis applies cleanly only to two IDENTICAL economies. Grossman-Helpman (1990) show that trade between countries with different endowments can EITHER speed up OR slow down growth, depending on whether trade shifts resources toward or away from the R&D-intensive sector. For China in the 2000–2015 period: China is moving from low-skill manufacturing toward higher-complexity capabilities → the question is whether trade exposure shifts resources toward or away from capability-intensive sectors.

- **Relevance to project.** Three direct implications:
  1. **Tariff shocks reduce the effective scale of the growth engine.** Whether Chinese manufacturing follows the KD or LE mechanism is sectoral: high-tech exports (electronics, machinery) follow KD (ideas flow along supply chains → idea spillovers from exposure to sophisticated foreign buyers); low-tech exports (textiles, basic manufacturing) follow LE (physical capital goods are what matters). The China shock tariffs primarily target MANUFACTURING goods → LE mechanism → permanent growth rate reduction via goods trade channel. High-tech sectors lose BOTH goods market scale AND idea flows if tariffs restrict supply chain relationships.
  2. **The irreversibility of permanent growth effects motivates large tariff × capability interactions.** In static models, tariff shocks have level effects that reverse when tariffs are removed. In Rivera-Batiz-Romer, tariff shocks have PERMANENT growth effects that COMPOUND over time. For the project: if tariff shocks suppress d_in permanently (not just temporarily), the long-run welfare loss far exceeds the short-run revenue effect. Event study analysis (Sun-Abraham, §5b) should test whether d_in effects persist (absorbing treatment) rather than reverting after tariff removal.
  3. **Idea flows along trade networks are the overlooked channel.** Rivera-Batiz-Romer identify that in the KD model, it is IDEA FLOWS not goods flows that drive growth. For Chinese firms, the most important mechanism may not be the tariff on the physical goods but the disruption of learning relationships with foreign buyers (learning-by-exporting channel, discussed in §5b Atkin et al. 2017). Firms in capability blocks with strong upstream-downstream learning (e.g., electronics assembly with Japanese/Korean component suppliers) face BOTH goods market AND idea flow disruption from tariffs — doubling the growth rate suppression.

---

### Cross-paper synthesis (§5e)

**1. The three-mechanism framework (market size, business stealing, escape competition) applies to d_in/d_out.** Akcigit-Melitz provides the complete mapping: export market access (size effect) → d_in incentive; import competition or tariff pressure (business stealing + escape competition) → d_in effect depends on firm position; new export block entry (d_out) → strongest innovation response for new entrants. Each d_in/d_out move activates a specific subset of these three mechanisms.

**2. Tariff shocks combine NEGATIVE market size and AMBIGUOUS competition effects.** The net effect on d_in is: tariff↑ → market size↓ (unambiguously reduces d_in) AND competition↑ (escape-competition for neck-and-neck firms: may increase d_in; Schumpeterian for laggards: reduces d_in). Total: the sign depends on the firm's position in its capability block and the magnitude of the tariff. The project needs to test whether the market size effect dominates (d_in overall falls) or the escape-competition effect partially offsets it for frontier firms.

**3. Rivera-Batiz-Romer provides the permanent vs. transitory distinction.** Standard DiD/event study captures short-run effects. Rivera-Batiz-Romer shows that trade restrictions have PERMANENT growth rate effects (not just level effects) via scale of the research sector. The project's event study will capture the medium-term d_in/d_out response (2-5 year window) but not the permanent growth trajectory. A complementary analysis using longer-run productivity data would be needed to detect the permanent channel.

**4. The US-China pattern vs. EU-China pattern is explained by the framework.** Autor et al. (2020): US firms face negative innovation from Chinese competition (laggards with low profits = Schumpeterian dominant). Bloom et al. (2016): European firms face positive innovation from Chinese competition (neck-and-neck firms with escape-competition motive dominant). For Chinese firms facing US tariffs: Chinese firms in blocks where they are GLOBALLY COMPETITIVE (high BRIM fitness = neck-and-neck) → escape-competition effect → d_in increases; Chinese firms in blocks where they are MARGINAL (low fitness = laggards) → Schumpeterian effect → d_in decreases. This is exactly the fitness rank × tariff interaction predicted throughout §5d–§5e.

---

## §5f — Firm-Size Distortions, Regulatory Misallocation, and Weaponized Interdependence (Batch 5f)

*Papers read in full, 2026-06-05*

---

### Garicano, Lelarge & Van Reenen (2016) — "Firm Size Distortions and the Productivity Distribution: Evidence from France"
*American Economic Review 2016, 106(11): 3439–3479* — **Size-contingent regulations create a broken power law; welfare costs are 1.3–3.5% GDP, main losers are workers**

- **Research question and setting.** How do size-contingent labor regulations affect firm size, firm productivity, and aggregate welfare? France is the laboratory: when firms cross the 50-employee threshold they face a sharp jump in obligations (works council with 0.3% payroll budget, health-and-safety committee, union representative, profit-sharing plan, higher firing costs, monthly labor reporting, formal professional assessment for workers over 45). Figure 2 of the paper shows an unmistakable sharp fall in the number of firms at exactly 50 employees in 2000 — a "broken power law" in the employment size distribution. The US analog is the Affordable Care Act penalty for firms with more than 50 full-time employees that do not offer health coverage.

- **Theoretical model: Lucas (1978) + size-contingent tax.** The primitive is a distribution phi(α) of managerial ability α over [α_, α_max]. Each manager-entrepreneur with ability α hires n workers and produces y = α·f(n), with f'' < 0 (decreasing returns to managerial time). A tax on labor applies only for n > N (N = 49 in the main application), with variable component τ and fixed component F. Individual optimization yields:
  - n*(α) = f'^{-1}(w/α) for α ≤ α_c (small unconstrained)
  - n*(α) = N for α_c ≤ α < α_r (constrained at threshold)
  - n*(α) = f'^{-1}(τw/α) for α ≥ α_r (regulated, paying tax)

  The equilibrium partitions agents into four groups: workers (α < α_min), small unconstrained firms (α_min to α_c), constrained firms (α_c to α_r, bunched at N = 49), regulated large firms (α ≥ α_r, paying τ and F). The general-equilibrium wage w* FALLS because the regulation reduces demand for workers.

- **Proposition 1 (variable cost τ > 1, no F).** The introduction of τ: (i) reduces equilibrium w (incidence on workers); (ii) increases small-firm entry and makes small firms larger (lower w); (iii) creates a bulge at N and a valley [N, n_r]; (iv) reduces firm size proportionally for all regulated firms (α ≥ α_r). The broken power law: below N the distribution obeys χ(n) ∝ n^{-β} with slope parameter β = β_α(1−θ)+θ; after n_r the distribution also follows a power law with SAME slope but LOWER intercept (downward parallel shift of magnitude T = τ^{−β_α/(1−θ)}). The SHIFT identifies τ; the VALLEY WIDTH identifies F/w; the BULGE SMOOTHNESS identifies measurement error σ.

- **Empirical identification via ML on the size distribution.** Using power-law assumption phi(α) = c_α·α^{-β_α} and f(n) = n^θ, the firm size distribution is a known function of (β, θ, T, n_r, σ). Maximum likelihood on the universe of French manufacturing firms (FICUS, ~200,000 firms per year, 1995–2007) delivers:
  - β̂ ≈ 1.80 (power-law slope, stable)
  - n̂_r ≈ 59 (upper employment threshold)
  - σ̂ ≈ 0.12 (measurement error in employment)
  - **τ̂ − 1 = 2.3%** (baseline variable labor tax, robust to θ from 0.5 to 0.9: range 0.7%–5.9%)
  - F̂/w ≈ −0.94 (NEGATIVE fixed cost = small positive spillover from compliance information gathering, consistent with ERP adoption for tracking labor inputs)

- **Welfare and distributional results (Table 3).** With returns to scale θ = 0.80 and baseline F-US structural unemployment difference calibration (a = 0.70 partial wage rigidity):
  - Output loss = 0.022% GDP (tiny; wage adjustment offsets most distortion when wages are flexible)
  - Implicit tax (compliance costs not captured as government revenue) = 1.3% GDP
  - **Total welfare loss = 3.45% GDP** (baseline); falls to 1.3% GDP under fully flexible wages
  - Employment loss ≈ 140,000 workers (unemployment from partial wage rigidity)
  - **Distributional reversal**: workers lose 3.9% expected wage; large firms lose 3.3% profits; SMALL FIRMS GAIN 7.2% entry and 5.0% size increase (benefit from lower equilibrium wages WITHOUT bearing the regulatory tax). The regulation designed to protect workers HURTS them (via wage depression and unemployment) and enriches low-productivity small firms.

  Robust to: capital-labor substitution (CES, welfare loss ≈ 2.5% at partial rigid wages); industry heterogeneity (τ ranges 0.8%–3.5% by sector); dynamic model with AR(1) productivity and quadratic adjustment costs; alternative employment definitions (FICUS vs. DADS).

- **Comparison with Hsieh-Klenow (2009).** The Hsieh-Klenow (2009) approach to misallocation (MRPL dispersion) gives τ̂ ≈ 2.86% when applied to firms away from the French threshold — close to 2.3%, validating both approaches. Hsieh-Klenow (2009) used the same NBS Chinese firm-level dataset used in this project (see §5b Guariglia et al.) and found misallocation accounts for 25–40% of the US–China TFP gap. Garicano et al. provide a MECHANISM for one component: size-contingent regulations that prevent high-ability managers from scaling their capabilities.

- **Relevance to project.** Five direct implications:
  1. **Chinese labor regulations have analogous size-contingent thresholds.** The 2008 Chinese Labor Contract Law introduced substantial new obligations at 10+ and 25+ employee thresholds; informal enforcement thresholds at 50 and 100+ (social insurance contributions, union obligations). These create BRIM-block analogs: high-capability Chinese private firms are artificially held below optimal scale, suppressing d_in. The NBS panel (same as Guariglia §5b) contains the firm-level evidence: check for broken-power-law deviations around Chinese thresholds as a diagnostic for regulatory misallocation.
  2. **Tariff shock as ADDITIONAL distortion on top of existing regulatory constraint.** Garicano's model implies a complementarity: a firm already bunched at N = 49 (constrained below α_r) that faces a tariff-induced demand shock cannot GROW OUT of the constraint (cannot achieve d_in via scale) and is forced to survive within its current capability block. Tariff effects on d_in are predicted to be AMPLIFIED for firms near the size-contingency threshold — a testable interaction: regulatory-bunching × tariff.
  3. **Ownership × regulation interaction (links to §5b Guariglia).** Guariglia shows SOEs face soft budget constraints (effectively α_r → ∞); private firms face financial AND regulatory constraints (finite α_r). Garicano implies private firms near the 50-worker threshold face TRIPLE constraint (financial + regulatory + capability block) under tariff shocks. Predicted interaction in project data: private × near-regulatory-threshold × high-tariff → LARGEST d_in reduction.
  4. **Welfare decomposition maps onto tariff channels.** Dominant welfare cost = IMPLICIT TAX component (1.3% GDP), not output loss (0.02% GDP), when wages adjust. For the project: the dominant welfare cost of tariff shocks may be the CAPABILITY INVESTMENT forgone (d_in investments not taken = capability-destruction cost) rather than the contemporaneous output drop. Event studies should test whether d_in effects persist as an absorbing treatment, consistent with Rivera-Batiz-Romer's permanent growth effect (§5e).
  5. **Size distribution as a diagnostic for regulatory exposure.** The valley [N, n_r] contains firms that have crossed the threshold and are paying the regulatory tax. For Chinese firms: the share of employment in the valley = proxy for regulatory exposure. Firms in the valley AND exposed to high tariffs face the LARGEST capability reconfiguration incentives (d_out search for unregulated product-destination blocks).

---

### Farrell & Newman (2019) — "Weaponized Interdependence: How Global Economic Networks Shape State Coercion"
*International Security 2019, 44(1): 42–79* — **Hub-and-spoke network topology enables panopticon + chokepoint effects; supply chain dependence is the next frontier**

- **Research question.** How do global economic networks — rather than bilateral dyadic relationships — generate state coercive power? The standard liberal view (Keohane-Nye) holds that complex interdependence disperses power and generates reciprocal vulnerabilities. Farrell-Newman argue the opposite: globalization generates ASYMMETRIC hub-and-spoke topologies (power-law degree distributions) in which states with jurisdictional control over the hubs have structural coercive power over all other nodes. The key claim: structures that emerged from market actors pursuing efficiency and market power can be put to quite different coercive purposes by states.

- **Network topology: hub-and-spoke as structural fact.** Drawing on Barabási-Albert (1999) preferential attachment and Newman-Park (2003) social network theory:
  - **Preferential attachment**: New nodes attach disproportionately to already-connected nodes → rich-get-richer → power-law degree distribution. Statistical form (power-law, log-normal, stretched exponential) is secondary; the asymmetry is the structural fact.
  - **Network effects + increasing returns to scale** → winner-take-all dynamics (SWIFT, ICANN, Facebook, Google, AWS).
  - **Lock-in**: Challengers must coordinate a critical mass of defectors. Once established, "it is diffficult for economic actors to change or substantially displace" hub structures. Lock-in by historical events (Arthur 1989; David 1985) = same mechanism as BRIM capability block persistence.
  - Empirical facts: US+UK are exceptionally well-connected in global financial networks; 70% of global web traffic flows through Northern Virginia (AWS); 97% of intercontinental internet traffic through ~300 fiber optic cables; SWIFT serves 11,000+ financial institutions in 200+ countries.

- **Two mechanisms of weaponized interdependence.**
  1. **Panopticon effect**: Hub controllers extract information about all flows passing through the hub. Cases: (a) SWIFT/TFTP — US Treasury issued subpoenas against SWIFT's Virginia data center post-9/11; extracted global financial transaction data; became "Rosetta stone for US counterterrorism." (b) NSA/PRISM and upstream collection — AT&T's internet backbone used to intercept traffic from competitors; STELLARWIND and successors exploit US network centrality ("this is a home game for us" — NSA Director Hayden).
  2. **Chokepoint effect**: Hub controllers can cut adversaries off from the network entirely. Cases: (a) SWIFT/Iran — US Senate Banking Committee threatened to sanction SWIFT if it continued serving Iranian banks (January 2012); EU passed regulations banning SWIFT services to targeted institutions (March 2012); Iran's banks cut from global payment system → key bargaining chip in nuclear negotiations. SWIFT CEO: "disconnecting banks is an extraordinary and unprecedented step." (b) ZTE supply chain exclusion from US components → China forced to reconfigure semiconductor capabilities (firm-level d_out shock at macro scale).

- **Conditions for weaponized interdependence (necessary conjunction).** Not all states can exploit network position. Two prerequisites must hold JOINTLY:
  1. **Jurisdictional control over hub nodes** — physical presence or legal reach over the hub. US has this for SWIFT (Virginia mirror data center), internet (all major firms in US), dollar clearing. EU has partial control (SWIFT HQ near Brussels).
  2. **Appropriate domestic institutions** — regulatory capacity to compel hub actors and legal framework for extraterritorial reach. US has OFAC, post-9/11 surveillance laws, correspondent banking regulations. EU has fragmented financial regulation → can deploy SWIFT chokepoints ONLY by unanimous agreement under US prodding; BUT has strong privacy institutions → can leverage EU data protection for panopticon-type control in digital domain.

  This conjunction explains the empirical variation: SWIFT (US+EU → both effects available); internet (US panopticon only; no chokepoint because US lacks domestic institutional capacity to oblige e-commerce firms AND has strategic interest in open internet); oil markets (no single hub → no weaponization).

- **Limits and strategic responses (decoupling dynamics).** States exposed to weaponized interdependence respond by seeking autonomy:
  - Russia: threatened "without limits" response to SWIFT exclusion; explored blockchain-based alternatives for Eurasian Economic Union.
  - China: ZTE semiconductor exclusion → strategic push for domestic chip manufacturing; Huawei fears (US + allied suspicion of built-in backdoors). "As interdependence becomes increasingly weaponized, global supply chains may unravel." (p. 1415)
  - EU: Exploring alternative payment channels isolated from US financial system (INSTEX for Iran trade); German FM Maas publicly calling for European strategic autonomy in finance.
  - General logic: chokepoint threats → target states seek autarky or parallel hub construction → potential for NETWORK DECOUPLING along geopolitical lines.

- **Relevance to project.** Six direct implications:
  1. **RegDependency = firm-level chokepoint exposure.** The project's moderator RegDependency (UN COMTRADE bilateral import concentration = how much destination country d depends on China for product p) is the FIRM-LEVEL ANALOG of Farrell-Newman's chokepoint exposure. A firm exporting overwhelmingly to a single destination that simultaneously imposes tariffs faces both the direct tariff cost AND strategic chokepoint: the importer can threaten to cut off market access entirely. High RegDependency = high chokepoint exposure = stronger tariff effect on d_out (firms must diversify destinations = jump capability blocks to escape the chokepoint).
  2. **d_out as strategic autonomy response.** Farrell-Newman's key insight: the strategic RESPONSE to weaponized interdependence is network decoupling (building alternatives). For Chinese firms, d_out = the product-block-level analog of Russia building SWIFT alternatives or China developing domestic semiconductors. Firms with high d_out BEFORE the tariff shock are LESS vulnerable to chokepoint effects because they have pre-positioned in multiple blocks. Prediction: pre-shock d_out-diversified firms absorb tariff shocks with SMALLER d_in contraction than single-block firms — a testable heterogeneous treatment effect using baseline block diversification as a moderator.
  3. **BRIM blocks = supply chain hubs at the product level.** Farrell-Newman describe global supply chains as hub-and-spoke networks with preferential attachment and lock-in. The BRIM blocks ARE these hub structures at the firm-product level: each capability community is a dense self-reinforcing cluster (path-dependent accumulation; see Dosi §4b, Storper §4d). A tariff shock targeting one block's products functions as a CHOKEPOINT on the firms in that block. d_out = finding alternative blocks = the supply-chain rerouting described for ZTE.
  4. **Panopticon effect = asymmetric information channel.** The panopticon effect captures how hub-controlling actors gain information advantages over all participants. For Chinese exporting firms, selling into high-RegDependency destinations means those importers (US/EU buyers) have information advantage over the Chinese firms' production capabilities. This is the reverse learning-by-exporting channel. Post-tariff, this informational asymmetry persists and shapes which products Chinese firms can credibly redirect — a mechanism for why d_in (staying in known capability blocks with familiar buyers) is the defensive default response.
  5. **Ownership × RegDependency interaction (maps to Garicano + Guariglia).** Farrell-Newman show that institutional capacity moderates the ability to weaponize network position. For the project: SOEs (better institutional connectivity to the Chinese state = partial mitigation of chokepoint) × RegDependency (exposure to foreign hub) is the firm-level version. Prediction: SOE × high-RegDependency firms show LESS d_out response than private × high-RegDependency firms because SOEs can rely on state-mediated alternative channels (government-to-government trade agreements, Belt and Road destination diversification).
  6. **Geopolitical interpretation of RegDependency measure validates the moderator choice.** The Teti tariff data captures de jure applied MFN and preferential tariffs. Farrell-Newman show that REAL trade barriers include chokepoint threats BEYOND tariff lines (SWIFT exclusion, supply chain exclusion for ZTE). RegDependency proxies for TOTAL strategic exposure, including these non-tariff chokepoint channels. This justifies using RegDependency as a MODERATOR (not just a control): it captures the strategic dimension of bilateral trade dependence that goes beyond the tariff measure itself.

---

### Cross-paper synthesis (§5f)

**1. Two distinct mechanisms of capability suppression operate simultaneously: regulatory misallocation (Garicano) and strategic chokepoint (Farrell-Newman).** Garicano identifies SIZE-CONTINGENT REGULATIONS as a structural brake on productive firm growth: high-α firms held below optimal scale → d_in suppressed by regulatory bunching. Farrell-Newman identify STRATEGIC DEPENDENCE as a dynamic amplifier of trade shocks: chokepoint exposure makes otherwise-moderate tariff shocks catastrophic for firms without alternative network routes. Both mechanisms operate ON TOP OF the standard demand-side tariff effect (Amiti-Konings §5a). For the project, the BASELINE tariff coefficient (Sun-Abraham IW estimator) captures the demand channel; heterogeneity by regulatory position (valley-bunching) AND by RegDependency captures the structural and strategic channels respectively.

**2. Garicano + Guariglia (§5b) form a complete misallocation story for Chinese private firms.** Guariglia shows SOEs face soft budget constraints (financially unconstrained); private firms face self-financing constraints (financially constrained). Garicano adds a second layer: size-contingent REGULATORY constraints prevent private firms near the 50-worker threshold from scaling to absorb capability-adjacent products (d_in further suppressed). Predicted interaction in project data: private × near-regulatory-threshold × high-tariff → LARGEST d_in reduction; SOE × any-size × high-tariff → SMALLEST d_in reduction. This is a three-way interaction testable in the NBS panel.

**3. Farrell-Newman's decoupling prediction aligns with the project's event-study horizon.** The paper explicitly predicts that "global supply chains may unravel" as weaponized interdependence escalates. The project's data (2000–2015) covers the ORIGIN of this process: ZTE/Huawei concerns began visibly in this period; the 2018 US-China tariff war is the culmination of strategic tensions building throughout the sample. Pre-trend tests in the Sun-Abraham event study (§5b) should be ZERO if firms did not pre-position before the measured tariff shock. But if pre-trends in d_out turn POSITIVE in years immediately before the shock for high-RegDependency firms, this would signal strategic pre-decoupling consistent with Farrell-Newman — and would require interpreting the pre-period carefully to avoid contaminating the pre-trend test.

**4. The broken power law as a validation diagnostic for Chinese NBS data.** Garicano demonstrates a clean broken power law at N = 49 in French manufacturing. The NBS Chinese dataset should show analogous breaks at Chinese threshold sizes (10, 25, 50 workers). Replicating this diagnostic: (a) validates data quality; (b) identifies firms in the valley [N, n_r] as the regulatory-constraint group for heterogeneous treatment analysis; (c) calibrates an implicit regulatory tax τ for Chinese regulations via Garicano's ML method. This is a feasible secondary analysis given the NBS full-population data.

**5. Supply chain network topology = bipartite network topology.** Farrell-Newman argue that global supply chains have hub-and-spoke structures with lock-in and preferential attachment. The BRIM community detection finds exactly these hub-and-spoke structures in the firm-product bipartite network: each capability block is a dense community with internal nestedness (Solé-Ribalta §3b, Mariani §2e). Firms at the TOP of the within-block nested hierarchy (high d_in fitness rank) ARE the hub nodes in Farrell-Newman's sense: most connected within their capability block, greatest chokepoint exposure from destination-specific tariffs. This aligns with the within-block fitness rank × tariff interaction from §5d (Aghion 2005): frontier firms (neck-and-neck = network hubs) face the strongest d_in response — either escape-competition or defensive consolidation, depending on which mechanism dominates.

---

## §5g — Tariff Data, Rules of Origin, Product Vectors, and Trade Elasticities (Batch 5g)

*Papers read in full, 2026-06-05*

---

### Felbermayr, Teti & Yalcin (2019) — "Rules of Origin and the Profitability of Trade Deflection"
*Journal of International Economics 121 (2019): 103248* — **86% of FTA pairs have no profitable trade deflection; RoOs are systematically over-used**

- **Research question.** Are Rules of Origin (RoOs) in free trade agreements economically justified? RoOs exist to prevent "trade deflection" — routing third-country goods through a low-tariff FTA partner to access a high-tariff member at the preferential rate. If country i and j form an FTA and tij = 0 but ti,c > tj,c (country i's external tariff on third-country c exceeds j's), then goods from c could be transshipped through j to enter i cheaply. RoOs prevent this by requiring proof of substantial transformation in the originating FTA country. The paper asks whether trade deflection is empirically profitable in the first place.

- **Analytical framework.** Trade deflection from c through j to i is profitable iff:
  tick · τick > tijk · tjck · τijk · τjck (Eq. 2)
  i.e., the direct delivery cost (tariff + transport) exceeds the indirect route cost (FTA preferential tariff × partner's MFN tariff × double transport leg). The key insight: concave transport costs (τijk < τick · τjck by the triangle inequality under concavity) mean transshipment always incurs extra cost. The profitability condition becomes: tariff savings must EXCEED additional transportation costs.

- **Data.** Own-constructed global bilateral HS6 tariff dataset (applied MFN + preferential): 152 importer countries, all FTA and GSP arrangements, ~5,700 country-pairs, ~2,640 products, ~170 third countries c, for 2014. Transportation costs estimated from US Census CIF/FOB ratios (Schott 2008 data), regressed on bilateral distance at HS6 level: ln(τk_US,i) = ln(αk) + δk·ln(D_US,i) + u, then predicted out-of-sample for all country-pairs. Average estimated transport cost = 6%, consistent with Anderson-Van Wincoop (2004).

- **Main finding (Table 2).** For ALL country pairs in FTAs or GSPs:
  - 83% of country-pair × product × third-country combinations: trade deflection is NOT profitable even ignoring transport costs (equal or reversed tariffs)
  - 93% once transport costs are included (additional 10% of cases: tariff savings < transport premium)
  - For GSPs (unilateral preferences, rich→poor): **98%** of cases have no profitable trade deflection (developing-country MFN tariffs are typically HIGHER than developed-country MFN tariffs, making deflection through the developing country unattractive)
  - For FTAs: 86% unprofitable; for old FTAs: 94%; for new FTAs: 88%

- **Sector heterogeneity.** Products with highest deflection scope: agriculture, pulp and paper, works of art. LOWEST deflection scope: machinery and electrical equipment (HS 84-85), mineral products, optics — exactly the product categories that dominate Chinese export manufacturing.

- **Policy implication.** RoOs should be CONDITIONAL: require proof of origin only when tariff differentials exceed a product-specific threshold (determined by transportation costs). In GSPs, RoOs should activate only when the beneficiary country undercuts the donor's MFN tariff. The "spaghetti bowl" of unconditional RoOs imposes compliance costs (3-15% of final product prices per Anson et al. 2005) without economic justification in ~86-98% of cases.

- **Note on TETI authorship.** This is Feodora Teti's early work (with Felbermayr at ifo), directly preceding the Global Tariff Dataset (Teti_2024, §5a). The tariff data methodology here (bilateral MFN + preferential, HS6, imputed where missing, FTA-indexed) is the precursor to the GTD. Key finding for the project: Chinese exports primarily face MFN tariffs from most destinations (China is not party to most FTAs during 2000–2015). This confirms that the Bartik shift-share instrument exploits OVER-TIME variation in MFN tariffs applied to China — cross-sectional FTA heterogeneity is secondary.

- **Relevance to project.** Three direct implications:
  1. **RoOs as hidden barriers for input-intensive Chinese exporters.** Chinese firms that rely heavily on imported intermediates (exactly the Amiti-Konings §5a mechanism) may FAIL to qualify for preferential tariff rates under partner-country FTAs — because they cannot document sufficient value-added in China. When Chinese intermediate-input users export to EU/ASEAN partners with active FTAs, the RoO compliance cost (3-15% of price) can EXCEED the tariff savings, pushing them back to MFN rates. This means the Teti GTD's applied MFN tariff is the CORRECT measure for these firms (not the preferential rate).
  2. **Tariff data validation.** The paper's tariff dataset is a methodological precursor to Teti_2024's GTD. The finding that tariff data must account for ~500 FTAs (not just ~100 as in some competitors) and correct for missing data, phased tariffs, and tariff-line aggregation supports Teti_2024's superior quality claims. The project's tariff treatment variable is validated by this lineage.
  3. **Machinery/electrical equipment = low deflection risk = clean tariff variation.** HS 84-85 (machinery and electrical equipment) — a core Chinese export category and major tariff target in the 2018 US-China trade war — has the LOWEST scope for trade deflection and smallest tariff dispersion across destinations. This means that for these products, the Bartik tariff instrument is CLEAN: any tariff increase on Chinese machinery exports directly reduces trade flows without being partially offset by rerouting through third countries.

---

### Fontagné, Secchi & Tomasi (2018) — "Exporters' Product Vectors across Markets"
*European Economic Review 110 (2018): 150–180* — **LPVs are 80% zeros; firms have a stable core (TPV) under competition shocks; technological complementarity preserves the capability bundle**

*Note: Chiara Tomasi is at the Department of Economics and Management, University of Trento — Giovanni's institution.*

- **Research question and framework.** Multi-product exporting firms select different product bundles at each destination. How sparse, fickle, and stable are these bundles? The paper introduces three concepts:
  - **Global Product Vector (GPV_f)**: all products exported worldwide by firm f (ordered binary vector of 1s, dimension = N_products).
  - **Local Product Vector (LPV_fd)**: products exported to destination d (same length as GPV, with 1 if exported to d, 0 if NOT exported to d even though in GPV). The explicit inclusion of ZEROS is the key methodological innovation.
  - **Typical Product Vector (TPV_f)**: the MOST FREQUENT combination across destinations (among those exported to ≥ 2 markets).
  
  Key metrics: Levenshtein dissimilarity index (LevD) = share of zeros in LPV relative to GPV; Bray-Curtis similarity (BC) = accounts for both product identity AND market shares.
  
  Data: universe of Italian and French manufacturing exporters, 2000–2007, firm-product-destination level (ISTAT/Banque de France). Italy: 46,228 firms; France: 21,726 firms (restricted sample, ≥2 products, ≥2 destinations).

- **Finding 1: Sparsity.** Average LevD ≈ 0.80 for both Italy and France, stable across years: a firm exports on average only 20% of its GPV to any single destination. Even to the LARGEST destination: average LevD ≈ 0.70 (only 30% of GPV exported). Even to the destination with MOST products: average LevD ≈ 0.48 (52% of GPV). Regression (Table 3): LevD decreases with market size (β ≈ −0.007, p<0.01) and bilateral revenues (β ≈ −0.029, p<0.01); increases with market concentration (β ≈ +0.008, p<0.01) and quality (β ≈ +0.001, p<0.01). BUT: magnitudes are tiny — a 1-SD increase in revenues adds only ~0.5 products. Traditional determinants explain a small fraction of the sparsity.

- **Finding 2: Fickleness.** ~1/3 of French and Italian multi-product firms export a DIFFERENT product mix to each destination. Average pairwise LevD between LPVs from the same firm with the same product scope ≈ 0.52 (IQR: 0.27–0.78). Once zeros are properly included in Spearman rank correlations, the LPV-GPV correlation drops from ~0.68-0.76 (without zeros = biased upward, existing literature standard) to ~0.40 (correct). The "stable global product hierarchy" in Mayer et al. (2014) is a statistical artifact of omitting zeros: the Bray-Curtis similarity (BC ≈ 0.55, including zeros) shows that the hierarchy is much weaker than previously believed.

- **Finding 3: Stability (TPV).** Despite sparsity and fickleness, 65-69% of firms have a TPV. The TPV covers 44-47% of a firm's destinations on average and 67-68% of a firm's total export revenues. KEY: probability of exporting the TPV > probability of exporting any single TPV product alone (by first-order stochastic dominance test, p < 10^{-4}). The TPV is NOT a statistical artifact (random LPV benchmark gives only 40-43% of firms with a TPV). Moreover, 25-26% of TPVs contain products that are NOT the firm's highest-ranked by sales — the TPV is driven by COMPLEMENTARITY, not quality/efficiency sorting.

- **Key result (Table 7): TPV products are more resilient to competitive shocks.**
  - Baseline: TPV products are 7% LESS LIKELY to be dropped than non-TPV products (coefficient DTPV = −0.033, controlling for firm-product FE and year FE). Drop rate ≈ 45% for non-TPV products → TPV products have ~38% drop rate.
  - Sales interaction: TPV products are 30% LESS SENSITIVE to revenue changes (Sales × DTPV interaction = +0.006, attenuating the negative main effect −0.027). Quality interaction: similar pattern.
  - **Trade shock identification (Table 8, Panel A)**: Regress Drop_fp on China's world export share change × DTPV. Main effect of China competition: POSITIVE (more competition → more dropping). BUT for TPV products: REVERSED — higher Chinese competition → LESS likely to drop TPV products (China Share × DTPV = −0.362, p<0.01 for Italy).
  - **DiD identification (Table 8, Panel B)**: Post2002 × Quota_p × DTPV = −0.077 for Italy: after MFA quota removal (treated quota sectors, post-2002), firms are +18.7 pp more likely to drop products, but TPV-in-quota-sectors products are 7.7 pp LESS likely to be dropped than the non-TPV comparison. France: similar magnitude.

- **Technological complementarity mechanism (Table 9).** Intermediate inputs (BEC classification) in the TPV are retained even though they are marginally profitable. TPV × Intermediate interaction: firms are MORE likely to drop intermediate products in general, but LESS likely to drop them when they belong to the TPV (DTPV × Intermediate = −0.042, p<0.01). The Italian electric motors firm example: parts and components (1% market share) are co-exported with the motor products (52% + 11% market share) across all major European destinations = TPV. The parts are retained because they are technically necessary for the final goods, not because of their own quality or profitability.

- **Relevance to project.** Six direct implications:
  1. **GPV/LPV/TPV maps directly onto the BRIM framework.** GPV = full capability set (all products a firm can export with RCA > 1 globally); LPV_fd = products actively exported to destination d with RCA > 1; TPV = Share_core (the stable capability core). d_in = deepening the LPV-within-GPV allocation within a stable BRIM block; d_out = expanding the LPV to include products from a NEW BRIM block. The Fontagné-Secchi-Tomasi framework provides the multi-destination empirical precedent for the project's BRIM decomposition.
  2. **The stability (TPV consolidation) finding is direct evidence for d_in as the defensive response to trade shocks.** The China MFA removal result (Table 8) shows that competitive trade shocks cause firms to CONSOLIDATE around the TPV — precisely the d_in consolidation mechanism the project predicts for tariff shocks. The project extends this by: (a) using CAUSAL identification (Sun-Abraham IW estimator instead of China share proxy); (b) measuring within-BRIM-block vs. cross-block movement rather than just stable vs. unstable products; (c) testing whether the TPV-consolidation is stronger for firms with high within-block fitness rank (capability ladder analog).
  3. **Sparsity validates the EFC/BRIM measurement approach.** The 80% zeros in LPVs confirms that firm-product networks are inherently sparse. The RCA > 1 threshold (used in BRIM) correctly captures the active product portfolio — firms with many potential products only actually export 20% of them to any given destination. A firm-product bipartite matrix M_ipt = 1{RCA_ipt > 1} correctly codes this sparsity.
  4. **Fickleness provides an alternative mechanism for d_out.** 1/3 of firms naturally export different product mixes to each destination. Some of the measured d_out may reflect NATURAL DESTINATION-SPECIFIC FICKLENESS rather than capability development. The project should control for this baseline fickleness by measuring d_out relative to its pre-shock distribution within the firm.
  5. **Technological complementarity = capability block cohesion mechanism.** The retention of intermediate inputs within the TPV explains WHY capability blocks are stable. The BRIM community structure should include both final goods AND their input complements (parts & components) — and both should be retained under shocks (consistent with d_in = within-block consolidation).
  6. **Institutional connection: Tomasi at UniTrento.** This paper is co-authored by Chiara Tomasi (University of Trento), the same author behind the Le-Tomasi (2023) Vietnam paper (§5a) that is the project's closest methodological template. Giovanni should cite this paper prominently and consider using the GPV/LPV/TPV framework as a conceptual bridge to the De Stefano (2025) BRIM decomposition.

---

### Fontagné, Guimbard & Orefice (2022) — "Tariff-Based Product-Level Trade Elasticities"
*Journal of International Economics 137 (2022): 103593* — **Product-level ε̄ = −5.3 estimated from bilateral tariff variation; wide heterogeneity by product type; heterogeneous εk much more accurate than homogeneous ε̄ for predicting post-PTA import changes**

- **Research question and contribution.** Trade elasticity (how much trade flows respond to a 1% change in tariffs) is a CRUCIAL parameter for welfare evaluation of trade policy, yet estimates diverge widely (Head-Mayer 2014 survey: median 5.03, SD 9.3). Most estimates use price data subject to measurement error or focus on specific agreements. This paper estimates product-level (HS6) trade elasticities for 5,050 products entirely from BILATERAL TARIFF VARIATION, without using import prices. Panel: 152 importers × 189 exporters, years 2001, 2004, 2007, 2010, 2013, 2016 (six observations, non-consecutive). Tariff data: MAcMap-HS6 (CEPII), applied MFN + preferential at HS6. Trade data: BACI (CEPII), FOB values.

- **Empirical model (Eq. 5).** For each HS6 product k:
  X_{ijk,t} = exp[θ_{ik,t} + θ_{jk,t} + βk·ln(1+τ_{ijk,t}) + γk·ln(d_{ij}) + ζk·Z_{ij}] · ε_{ijk,t}
  
  Estimated by PPML (Santos-Silva and Tenreyro 2006) to handle zeros and heteroscedasticity. Exporter-year (θ_{ik,t}) and importer-year (θ_{jk,t}) FEs control for all unobserved country-product-year factors. Identification: CROSS-COUNTRY-PAIR variation in bilateral tariffs for each product k. Key finding from Table 3: between variation >> within variation for all HS sections. Distance elasticity γk can be recovered as ρk = γk/βk — average ρ = 0.155 (consistent with Hummels 2007: 0.151 maritime, 0.160 air).

- **Key results.**
  - Average trade elasticity (1% significant only, replacing insignificant with 0): **ε̄ = −5.3** (median −3.5)
  - Distribution: concentrated around −5, left tail cut at −25 (3% of products have |εk| > 25)
  - **Sector heterogeneity by HS section (Table 5)**:
    - Mineral products (HS V): ε̄ = −18.5 (homogeneous, highly elastic)
    - Textile and apparel (HS XI): ε̄ = −7.15
    - Machinery/electrical equipment (HS XVI): ε̄ = −6.08
    - Vehicles (HS XVII): ε̄ = −10.46
    - Footwear (HS XII): ε̄ = −3.61 (most differentiated, least elastic)
    - Base metals (HS XV): ε̄ = −9.59
  - **Product differentiation**: Homogeneous products (Rauch classification) have significantly larger |εk| and higher variance than differentiated products (Table 6, β = −6.55, p<0.01)
  - **Distance effect**: Higher average distance → LOWER |εk| (more elastic products trade locally; distant-market exporters are less price-sensitive)

- **TiVA-sector elasticities for welfare (Table 8)**: The project-relevant sectors:
  - Textiles, leather, footwear: ε = −4.71
  - Machinery and equipment nec: ε = −5.01
  - Computer, electronic, optical: ε = −5.14
  - Electrical machinery: ε = −4.11
  - Motor vehicles: ε = −8.92
  - Chemicals: ε = −10.56

- **Accuracy validation (ex-post test).** US-Chile FTA entered force January 2004. Average tariff cut: 93% (6.9% → 0.5%). Predicted vs. observed 2004-2007 Chilean imports from US: STRONG POSITIVE CORRELATION with heterogeneous εk (Table 7 columns 1-3: coefficient ≈ 1.95, p<0.01); NO CORRELATION with homogeneous ε̄ (coefficient near zero, insignificant). Conclusion: product-specific elasticities are empirically necessary for accurate predictions.

- **Endogeneity robustness.** Pre-trend test (Table 9): no correlation between pre-shock import growth and subsequent tariff change (no anticipation). IV strategy: bilateral product tariff instrumented by average tariff on same HS4-heading other products. OLS ≈ 2SLS (Figure 11): reverse causality not driving results.

- **Relevance to project.** Five direct implications:
  1. **Product-level εk for welfare quantification.** The project can directly use Fontagnè_2022's publicly-available elasticities (https://sites.google.com/view/product-level-trade-elasticity) to convert the Bartik tariff exposure measure into a welfare-equivalent trade flow impact. For a 10pp tariff increase on HS 84-85 (machinery: ε ≈ −6.08): predicted trade flow reduction = 6.08 × 0.10 = 60.8% (relative to original). This converts d_in/d_out changes from network movements into welfare-monetized terms via the ACR formula.
  2. **Heterogeneous εk as Bartik weights.** Standard Bartik instruments use uniform pre-period export shares as weights. A more accurate instrument would weight by εk (elasticity-adjusted Bartik): high-|εk| products contribute more to the firm's capability disruption because their trade is more sensitive to tariff changes. Products with ε ≈ −18.5 (minerals) lose 3× more trade per tariff point than products with ε ≈ −6 (machinery). The project's capability disruption measure should be weighted by εk to reflect actual market access loss.
  3. **Sectoral heterogeneity justifies industry-clustered standard errors.** The wide range of εk across HS sections (from −3.6 to −18.5) confirms that tariff shocks have very different impacts by sector. The project should cluster SEs at the firm × industry level (not just firm level) and include industry × year FEs. The Bartik Adão (2019) cross-section SE correction (§5b) is EVEN MORE IMPORTANT given this cross-sector heterogeneity.
  4. **Between-pair >> within-pair tariff variation (Table 3) confirms the Bartik shift-share design.** Most tariff variation is cross-sectional (between country pairs), not over time within a pair. For the Bartik instrument to work, the project needs to exploit the OVER-TIME component (changes in Chinese MFN tariffs at product level). The fact that within-pair variation is smaller but non-negligible (especially for textiles HS XI under MFA phaseout) means the instrument has genuine time variation, but the cross-sectional component may confound if Chinese export shares correlate with bilateral tariff levels.
  5. **PPML gravity as first-stage specification.** Eq. (5) with exporter-year and importer-year FEs is the theoretically-consistent first-stage gravity specification for the Bartik instrument. The project's first stage (tariff exposure → trade flow changes) should follow this structure, with the Bartik Adão (2019) SE correction for the shift-share correlation structure.

---

### Cross-paper synthesis (§5g)

**1. Teti (2019) + Teti (2024/§5a) complete the tariff data picture.** Teti_2019 establishes that (a) MFN tariffs dominate for China-destination pairs because China has few FTAs with major export destinations in 2000-2015; (b) tariff data requires careful construction to cover ~500 FTAs, handle phased-in schedules, and impute missing values; (c) RoOs reduce effective access to preferential rates for input-intensive Chinese exporters (Amiti-Konings §5a mechanism). Together with Teti_2024 (the full GTD), this confirms that the project's tariff treatment variable is the MFN applied rate from Teti's GTD, and this is the CORRECT measure for Chinese exporters in the project period.

**2. Fontagné_2018 + De Stefano (2025, destefano2025_synthesis) form a two-level hierarchy.** Fontagné_2018 operates at the firm-destination level (product sparsity within each destination), while De Stefano (2025) operates at the firm level across all destinations jointly (BRIM blocks). The TPV in Fontagné_2018 corresponds to the capability core (Share_core, d_in domain) in De Stefano; products exported to destination d but NOT in the TPV correspond to occasional exports (d_out candidates in De Stefano's terminology). The China MFA shock result in Table 8 of Fontagné_2018 provides DIRECT EMPIRICAL EVIDENCE that tariff shocks → TPV consolidation (d_in) + peripheral product dropping (d_out contraction), which is the project's main hypothesis. The key difference: Fontagné_2018 uses export value (a flow measure), while the project uses RCA-binarized network membership (a stock/structural measure). The structural measure may be more persistent and less subject to short-run fickleness.

**3. Fontagné_2022 provides the elasticity parameter that converts tariff changes to capability disruption magnitudes.** The project's outcome variables (d_in, d_out, Share_core) are NETWORK STRUCTURE measures, not trade flow magnitudes. But to connect the project to welfare analysis (ACR formula, Arkolakis et al. 2012), one needs to translate network structure changes into trade flow impacts, which requires εk. The elasticity heterogeneity (range −3.6 to −18.5 across sectors) means that the SAME TARIFF SHOCK generates very different capability disruptions by sector. This is a source of SECOND-ORDER HETEROGENEITY: beyond firm-level fitness rank (§5d), there is product-level elasticity heterogeneity that predicts WHICH products within a firm's portfolio are most disrupted.

**4. The three papers jointly validate the Bartik instrument design.** Teti (2019/2024): confirms MFN tariff variation is the right source of exogenous shock for China. Fontagné_2018: confirms that product-level trade flows respond to competition (validating the trade channel). Fontagné_2022: provides the key structural parameter (εk) linking tariff changes to trade flow changes (and hence capability disruption). Together: the Bartik = Σ_p ω_{ip,pre} × Δτ_{pdt} uses Teti GTD for Δτ, pre-period export shares ω for weights, and εk from Fontagné_2022 to convert tariff changes to trade flow-equivalent disruptions. All three papers are needed for a complete first-stage narrative.

**5. Fontagné_2018 + Aghion (2005, §5d) together explain the consolidation-vs-innovation trade-off.** Fontagné_2018 shows firms CONSOLIDATE around the TPV under competition; Aghion (2005) shows neck-and-neck firms INNOVATE to escape competition. These are complementary: TPV consolidation is the SHORT-RUN response (protect the core, drop marginal products) while escape-competition innovation is the MEDIUM-RUN response (invest in d_in adjacencies to stay ahead of competition). The project's event study should detect BOTH effects: d_in may FIRST decline (TPV consolidation by dropping marginal within-block products) and then REBOUND (escape-competition new capability acquisition) in a U-shaped pattern across the event-study horizon.

---

## §5h — The 2025 Trade War: Dynamic Welfare Simulation and Tariff Data Extension (Batch 5h)

*Paper read in full, 2026-06-05*

---

### Rodríguez-Clare, Teti, Ulate, Vasquez & Zarate (2025) — "The 2025 Trade War: Dynamic Impacts Across U.S. States and the Global Economy"
*CESifo Working Paper 12179 (October 2025)* — **GTD-U.S. Trade War Extension (2018–2025 daily); US real income −0.1% by 2028; trade elasticity is the pivotal parameter; China −0.3% vs Canada/Mexico −1.6%**

- **Research question and context.** The 2025 Trump tariff escalation raised average U.S. import tariffs from 1.5% (January 2018) to 4.8% (early 2025) to **25.4%** (mid-August 2025) — the highest since the 1930s Smoot-Hawley era. The paper uses a dynamic quantitative trade model (the Rodriguez-Clare-Ulate-Vasquez 2025 framework, extended with tariffs and cross-state fiscal redistribution) to assess the welfare consequences across 50 U.S. states, 59 countries, and 15 sectors. **Teti's central contribution** is the construction of the GTD-U.S. Trade War Extension (henceforth GTD-TW), the updated tariff database that forms the empirical spine of the exercise.

- **GTD-U.S. Trade War Extension: key dataset contribution.** Building directly on Teti (2024/§5a) methodology, the GTD-TW covers all U.S. tariff instruments at the TARIFF-LINE level at DAILY frequency, from January 2018 through August 15, 2025, then aggregated to HS6. This dataset is the most complete, granular, and methodologically consistent tariff database for the 2018-2025 period. Key features:

  - **Instruments covered** (with stacking rules in Appendix A.2):
    1. Baseline (MFN or preferential, or Column 2 for Cuba/North Korea/Russia/Belarus)
    2. Safeguards (Sec. 201): solar panels (30%), washing machines (20%), phased reductions
    3. Sec. 301 (China-specific "Unfair Trade Practices"): Lists 1-3 = $250bn at 25% (Jul-Sep 2018); List 4A = $120bn at 15% (Sep 2019) → 7.5% (Feb 2020); Biden extensions (EVs, batteries, solar, tungsten/wafers) Sep 2024 + Jan 2025
    4. Sec. 232 (National Security): steel 25% + aluminum 10% global (March 2018); all exemptions removed + aluminum raised to 25% (March 2025); both raised to 50% (June 2025); autos +25% (April 2025); car parts +25% (May 2025); copper +50% (August 2025)
    5. IEEPA: China +10% (Feb 2025) → +20% (Mar 2025); Canada/Mexico +25% non-USMCA (Mar 2025); Canada raised to 35% (Aug 2025); Brazil +40% (Aug 2025)
    6. Liberation Day (April 2025): flat +10% on ALL imports (stacked on Sec. 232, with carve-outs for pharma, semiconductors, energy)
    7. Reciprocal tariffs (August 2025): China escalation to +84/125% → rolled back to +10% (May deal); UK 10% + cars 7.5%; EU "15-MFN" formula; Vietnam/Indonesia/Philippines/Korea → 15-20% reciprocal + pledged 0% on US exports

  - **Stacking logic**: Sec. 232 + Sec. 301 + IEEPA stack cumulatively (e.g., Chinese steel in early 2025 = 25% MFN + 25% Sec. 301 + 25% Sec. 232 + 20% IEEPA → ~100% effective tariff). Liberation Day and Reciprocal tariffs replace each other (not stacked). Content-based tariffs apply only to material content (50% content share assumed for steel/aluminum/copper derivatives).

  - **Preference Utilization Rates (PURs)** used to adjust for USMCA compliance on Canada/Mexico (effective tariff = (1-PUR) × announced rate). This avoids overestimating the tariff burden on compliant trade flows.

  - **China retaliatory tariffs**: 6.2% (2018) → 15.3% (2025 start) → **26.9%** (August 2025), targeting US agricultural exports (soybeans, pork) and advanced manufacturing.

- **Quantitative model.** Dynamic multi-sector Armington model (Rodriguez-Clare-Ulate-Vasquez 2025) extended with:
  - 110 regions (50 US states, 59 countries, RoW), 15 sectors (12 manufacturing + services + agriculture + home production)
  - Input-output linkages (Cobb-Douglas production with intermediate inputs from all sectors)
  - **Downward Nominal Wage Rigidity (DNWR)**: Wi,s,t ≥ δ × Wi,s,t-1 (δ = 1, nominal wages cannot fall). Creates involuntary unemployment when sector-level labor demand falls faster than wages can adjust.
  - Forward-looking mobility with Gumbel idiosyncratic shocks (inverse elasticity of mobility ν = 0.55 from RUV)
  - Tariff revenue redistribution: tariff revenue collected by US states redistributed to all states proportional to population (novel matrix equation solving for TRR = flexible cross-state fiscal mechanism)
  - Nominal anchor: world nominal GDP in dollars grows at γ = 3%/year (post-pandemic inflation baseline)
  - **Dynamic exact-hat algebra** (Caliendo et al. 2019): quantifies effects without knowing initial levels of technology or iceberg costs; matches 2024 base-year data.
  - Trade elasticity: σ = 6 (standard) in baseline.

- **Baseline results (σ = 6, 4-year shock, minimal retaliation).**
  - **U.S. aggregate real wages**: −0.7% by 2028
  - **U.S. aggregate real income** (inclusive of tariff revenue rebates): **−0.1%** by 2028 (tariff revenue partially offsets wage loss)
  - **Manufacturing employment/value added**: +3.7% peak (temporary; reverses when tariffs end → 0.5% unemployment in 2029 due to DNWR)
  - **Service employment/value added**: −1.6% by 2028 (unprotected by tariffs, hit by intermediate input cost increases)
  - **Agriculture**: +1.4% value added (modest gains from protection)
  - **Labor force participation**: −0.25% aggregate (home production becomes more attractive while market sector real wages fall)
  - **Cross-state heterogeneity** (Figure 5-6): CA, TX, IL, MI (high import exposure to China/trade partners) → real income loss −1.4%; WY, OK, SD, WV (energy/resource states, minimal China trade) → real income GAIN +1.9%. Exposure measure (expenditure share × tariff change) explains 77% of cross-state income variation.
  - **Cross-country** (Figure 11): Canada −1.6%, Mexico −1.6%, Vietnam −1.1%, Ireland −0.8%, China −0.3%. Some countries GAIN (UK, Saudi Arabia) due to reduced competition in US markets.

- **Key sensitivity results (Table 1).**
  - **Trade elasticity σ is the single most critical parameter**:
    - σ = 6 (baseline): −0.11% US real income
    - σ = 3.12: +0.51% (US GAINS — has sufficient monopoly power to improve terms of trade)
    - σ = 2.44: +0.72%
    - σ = 1.76: +1.01%
    - At σ below ~3, the US is a monopsonist large enough to extract terms-of-trade gains despite welfare losses in other countries.
  - **Duration**: 4 years → −0.11%; 12 years → +0.04%; 16 years → +0.09% (longer = better for US because home production sector provides a constant utility floor that eventually dominates)
  - **Retaliation** (mirror = all partners impose equal tariffs back): 0% mirror → −0.11%; 33% mirror → −0.29%; 100% mirror → −0.56%. More retaliation = worse for US, but ALSO reduces the manufacturing-wage-spike that causes DNWR unemployment when shock ends.

- **Key economic mechanisms.**
  1. **Input cost amplification**: Higher US import tariffs raise intermediate input costs for US manufacturing (Amiti-Konings §5a at the macro level). For low σ (inelastic demand), firms substitute less from foreign to domestic inputs → higher input costs per unit → larger negative effect on manufacturing competitiveness per tariff dollar. This explains why low σ reduces the manufacturing employment BOOST.
  2. **Terms-of-trade effect**: For large countries (US monopoly power), tariffs improve terms of trade (foreigners' export prices fall in dollar terms). Only relevant when σ is low enough that US market power exceeds the deadweight loss.
  3. **DNWR asymmetry**: Tariffs RAISE manufacturing wages during the shock → DNWR is non-binding (wages rise freely). When shock ends, wages face downward pressure → DNWR BINDS → involuntary unemployment. The DNWR thus creates an IRREVERSIBILITY in the labor market: gains during the shock are partly reversed through unemployment at the exit.
  4. **Fiscal redistribution**: Tariff revenue collected at import-intensive states (CA, TX, IL) is redistributed proportional to population → implicit cross-state transfer from trade-exposed coastal states to interior states. This explains why 34 of 50 states GAIN despite aggregate US real income falling.
  5. **Service sector crowding out**: Manufacturing expansion under protection absorbs labor from services (which cannot be protected by tariffs) → service sector shrinks. Since services dominate employment, aggregate labor participation falls.

- **GTD-TW stacking rules as methodological reference.** The paper's Appendix A contains the definitive stacking algorithm for effective tariff construction — the most transparent public documentation of how to correctly combine multiple overlapping tariff instruments. This is directly relevant for any researcher using US import tariff data in the 2018-2025 period.

- **Relevance to project.** Seven direct implications:
  1. **GTD-TW validates and extends the project's tariff treatment variable (Teti_2024/§5a).** The project uses Teti (2024)'s GTD for the 2000-2015 sample period. Teti_2025 demonstrates that the SAME methodology (MFN + preferential assignment, imputation algorithm, FTA coverage) correctly captures the baseline tariffs that the 2018-2025 tariff changes stack upon. For the project, this confirms: (a) the GTD is the authoritative baseline from which China's EXPORT tariffs (τ_{pdt} in Teti_2024) are correctly derived; (b) the 2018 Section 301 tariffs are clearly identifiable as OUT-OF-SAMPLE shocks relative to the project's 2000-2015 window, but they validate the GTD methodology that was applied retrospectively to construct the project's treatment variable.
  2. **China's −0.3% real income loss is MUCH SMALLER than Canada/Mexico −1.6%**. The asymmetry is explained by: (a) China is a larger economy with more diversification; (b) China has higher domestic market share in manufacturing (less trade-exposed share of expenditure); (c) China retaliates (26.9% tariffs on US exports), partially offsetting US leverage. For the project: Chinese FIRMS are heterogeneous in their exposure — firms with HIGH RegDependency (concentrated exports to US) face a shock comparable to Canada/Mexico's aggregate shock, not China's average −0.3%. This STRONGLY supports RegDependency as the key moderator: high-RegDependency Chinese exporters lose 5-10× more than the average Chinese firm.
  3. **Trade elasticity (σ) is THE pivotal uncertainty parameter — calibration from Fontagnè_2022.** The paper shows that σ determines whether the US gains or loses from tariffs (Table 1). For the PROJECT's Bartik first stage, the same elasticity heterogeneity (Fontagnè_2022 §5g: ε ranging from −3.6 to −18.5) governs how much each Chinese firm's trade is disrupted by a given tariff shock. Firms in elastic-product sectors (minerals, ε ≈ −18.5) face LARGER capability disruption per tariff point than firms in inelastic-product sectors (footwear, ε ≈ −3.6). The project should use product-level εk from Fontagnè_2022 as the first-stage weight in the Bartik, rather than uniform weights.
  4. **DNWR creates an asymmetric adjustment path that mirrors Chinese capability adjustment.** In the US: tariffs → manufacturing wages rise → DNWR non-binding during shock → when shock ends, DNWR binds → unemployment. In China: tariff shocks on exports → firms must restructure capabilities → sunk costs in d_in investments → CANNOT easily revert capabilities after tariff removal → CAPABILITY LOCK-IN. This is the Chinese-side analog: the adjustment costs for firms that invested in new capability blocks (d_out) during the tariff shock period are irreversible (sunk costs of network position, see Storper §4d, Dosi §4b). The event-study pre-trends (if pre-trends in d_out persist or grow after tariff removal) would confirm this lock-in.
  5. **Service sector crowding out maps to d_out suppression.** In the US model, tariffs crowd out services in favor of manufacturing. For China: tariff shocks on export-oriented manufacturing → resource reallocation from manufacturing to domestic services (Chinese government's ongoing "rebalancing" from export-led to domestic-led growth). This manifests as d_out from export-facing capability blocks toward domestic-market capability blocks — a testable prediction in the project data (do firms in heavily export-dependent sectors show MORE d_out to domestically-oriented products post-shock?).
  6. **GTD-TW stacking rules → the project's tariff variable construction matters.** The paper shows that correctly specifying the EFFECTIVE tariff requires: (a) choosing the correct baseline (MFN vs preferential); (b) stacking additional instruments correctly; (c) accounting for PURs and content rules; (d) handling nomenclature changes (HS 2017 → HS 2022). For the project's 2000-2015 period, the tariff variation is simpler (primarily MFN changes from WTO/GATT negotiations), but the same care is required when constructing the Bartik Δτ_{pdt}. Specifically: some destination countries already had preferential agreements with China by 2000-2015 (ASEAN+China FTA, signed 2002, in force 2005-2010 phased); for these pairs, the project should use PREFERENTIAL rates (which are the Teti GTD's applied tariff = min(MFN, preferential)).
  7. **Quantitative welfare framework for the paper's contribution section.** The project measures capability reorganization (d_in, d_out) but does not calculate welfare magnitudes. Teti_2025 provides the CALIBRATED GE welfare framework that could be adapted: given the project's d_in/d_out estimates, one can use the ACR formula (Arkolakis et al. 2012 via Fontagnè_2022 §5g) to convert network structure changes into welfare-equivalent trade flow reductions. A 1-unit decrease in d_in (one fewer within-block product active) → using Fontagné_2022 εk and Teti_2025's domestic expenditure shares → welfare cost in GDP percentage terms.

---

### Cross-paper synthesis (§5h)

**1. Teti (2019) + Teti (2024/§5a) + Teti (2025) form a complete tariff data genealogy.** Teti_2019 established the methodology (bilateral HS6 applied tariffs, own-constructed, imputed missing data). Teti_2024 applied it globally to construct the GTD (1988-2021, all country pairs). Teti_2025 extends the GTD through 2025 at daily frequency with all tariff instruments stacked. For the project: the treatment variable (MFN applied tariffs on Chinese exports from Teti GTD) is methodologically consistent with the most careful tariff data available; the extension to 2025 validates that the 2018+ shock regime is a structural break relative to the 2000-2015 sample.

**2. Teti_2025 CONFIRMS that China is the PRIMARY target of the trade war, not a bystander.** Average US tariff on China: 2.9% → 16.1% → 54.4%. This compares to Rest of World: 1.1% → ~1.6% → ~4-5% (excluding China-specific measures). The project's sample (2000-2015) captures the PRE-ESCALATION period, but the POST-2018 shock regime shows what a LARGE tariff shock does: China −0.3% real income overall but with massive cross-sector heterogeneity. The project's identification exploits WITHIN-SAMPLE tariff variation in MFN tariffs, which is far smaller in magnitude — but the DIRECTION and MECHANISM are the same. The Teti_2025 results provide the UPPER BOUND on what the project's tariff shock would produce at the macro level.

**3. The DNWR unemployment mechanism in Teti_2025 = the capability lock-in mechanism in the project.** Teti_2025: US manufacturing expands during tariffs → wages rise → DNWR prevents adjustment when tariffs end → unemployment. Project: Chinese firms acquire d_in capabilities during tariff adjustment → sunk costs → capabilities cannot be easily reversed. Both mechanisms create IRREVERSIBILITY. The project should test whether d_in effects persist even after tariff levels return to baseline (absorbing treatment in event study). Teti_2025 shows that the adjustment asymmetry IS a real quantitative effect (0.5% unemployment in 2029), not just a theoretical possibility.

**4. Cross-country heterogeneity in Teti_2025 validates RegDependency as the key moderator.** Canada/Mexico (high US trade share, small countries) → −1.6%. China (diversified, large, retaliates) → −0.3%. This heterogeneity IS the firm-level analog of RegDependency: Chinese firms concentrated in the US market (high RegDependency) face Canada/Mexico-style shocks, not China-average shocks. The cross-country model results provide QUANTITATIVE BENCHMARKS for how large the heterogeneous firm-level effects should be — high-RegDependency Chinese firms should show 5-10× larger capability disruption than the average Chinese firm.

**5. Fontagnè_2022 (§5g) + Teti_2025 create a two-step welfare link.** Step 1: tariff shock → trade flow reduction (Fontagnè_2022 εk governs magnitude per unit tariff). Step 2: trade flow reduction → welfare change via ACR formula (Teti_2025 calibrates the sectoral domestic expenditure shares and uses multi-sector σ). The project's d_in/d_out changes sit in between: they are the INTERMEDIATE RESPONSE of the capability network to the initial trade flow shock. A full welfare calculation would require: (a) using εk to convert Bartik tariff exposure to trade flow disruption; (b) using d_in/d_out changes to measure the structural capability adjustment; (c) using the ACR formula with updated domestic expenditure shares to compute the welfare cost of the permanent capability reduction (Rivera-Batiz-Romer §5e: permanent growth rate suppression).

---

## §5i — EU Strategic Dependencies, Open Strategic Autonomy, and the SPOF Methodology (Batch 5i)

*Papers read in full, 2026-06-05*

---

### Fontana & Vannuccini (2024) — "How to Institutionalise European Industrial Policy (for Strategic Autonomy and the Green Transition)"
*LEAP Working Paper 7/2024 (March 2024)* — **Dependency-strategic logic requires permanent EU industrial policy; no strategic autonomy without fiscal autonomy; Ding-Dafoe three logics taxonomy for strategic assets**

- **Research question and argument.** How can industrial policy for the green transition and strategic autonomy be made PERMANENT (institutionalised) in the EU, rather than remaining a series of temporary exceptions to competition rules? The paper argues that the current polycrisis/permacrisis — climate emergency, geopolitical rivalries, deglobalisation pressures — makes European industrial policy not just desirable but structurally necessary. The EU faces a fundamental institutional tension: competition policy is a federal competence (Article 107 TFEU), while industrial policy must route through national State Aid exemptions. Without fiscal autonomy (own resources at EU level), this tension cannot be resolved.

- **Three logics of strategic assets (Ding-Dafoe 2021).** This framework is central to the paper's rationale for intervention. Strategic assets combine:
  1. **Cumulative-strategic logic**: High entry barriers + sunk costs + scale and learning economies + time required to build capabilities (aircraft, semiconductors). State intervention needed because private actors cannot recoup the upfront investment.
  2. **Infrastructure-strategic logic**: Coordination failure + large externalities as they facilitate distribution and circulation (railways, radar, internet infrastructure). Public investment needed to solve the coordination game.
  3. **Dependency-strategic logic**: Few substitutes + lack of input markets (rare earths, critical raw materials, photovoltaic cells). Dependency on a foreign monopolist creates vulnerability; intervention needed to diversify or build domestic capacity.
  
  Assets that satisfy ALL THREE logics are "truly strategically vital" (Figure 1). The current EU policy focus is primarily on (3): products where strategic dependency is high. But assets in sectors like semiconductors and batteries satisfy all three simultaneously.

- **Polycrisis context and the new industrial policy rationale.** Empirical data from Evenett et al. (2024): 2,850 industrial policy records in 2023 — 28% motivated by climate change, 15% by supply chain resilience, ~20% by national security/geopolitical tensions. Bown (2023): "curbing competition from China" is the dominant real motive beneath stated rationales. Key observation (Vicard-Wibaux): "it is not the underlying structure of dependencies that has changed but the perceived risks associated with them because of the concentration of imports from China, which is now considered less aligned geopolitically to the EU." The dependencies formed over a decade ago; their strategic salience is new.

- **EU dependency landscape.** European Commission (2021a): 137 products in sensitive ecosystems dependent on few suppliers (mainly China 52% by value, Brazil, Vietnam). Arjona et al. (2023) extends this to 204 products. EU Commission (2024) OSA assessment: EU exposure more at the TECHNOLOGY level than industrial ecosystem level (except digital). EU Sovereignty Index (EUSI 2022): EU ranks "poor" in technology, "satisfactory" in climate, "good" only in economy and health. Strong disconnect between commitments and capabilities, especially in technology.

- **Current EU industrial policy instruments and their limitations.** Five phases of European industrial policy (Pellegrin et al. 2015): ECSC (1950s), EEC sectoral planning (1957-1970s), competition priority (1990s), external pressure/globalisation return (2000s), re-industrialisation/smart specialisation (2015+). Current instruments:
  - **IPCEIs** (Important Projects of Common European Interest): 7 approved projects (Table 1), €27.9bn public + €51.4bn private leverage, 22 countries, 227 companies, 274 projects. Sectors: microelectronics, batteries (×2), hydrogen (×2), ICT/cloud. But: participation uneven (France, Germany, Italy in all IPCEIs; Central/Eastern Europe excluded); still predominantly national delivery + financing = "pan-European public good" not "pure European public good."
  - **NGEU/RRF**: Temporary (expiring 2026); only 5% of green investments needed by 2030; legal basis (Art. 122 TFEU) technically requires emergency justification.
  - **STEP** (Strategic Technologies for Europe Platform): Only €10bn in rationalised existing instruments; no substantial new financing; "European Sovereignty Seals" as signalling, not funding.
  - **InvestEU**: Closed cyclical investment gap but NOT structural gaps (net-zero, digitalisation, social infrastructure).
  - **Innovation Fund**: 41 of 70 high-scoring large-scale project proposals couldn't be funded due to budget constraints.

- **Proposals for institutionalisation.** Framework fund modeled on NGEU + ESF concept ("Climate and Strategic Investments Fund"): (1) Tier 1: upgraded IPCEIs evolving into pure European public goods (EU delivery + EU financing); (2) Tier 2: strengthened centrally managed programmes (InvestEU, Innovation Fund). Legal basis: Art. 122 TFEU emergency clause (polycrisis justification). Financing: new EU own resources (environmental, profit-sector levies, gambling/tobacco/financial sectors). Key principle: **no strategic autonomy without fiscal autonomy.**

- **Relevance to project.** Five direct implications:
  1. **Ding-Dafoe taxonomy maps onto BRIM capability block types.** The three logics classify strategic assets in a way that maps directly onto the project's capability block structure: (a) Cumulative-strategic sectors (semiconductors, batteries, aircraft) = capability blocks with HIGH d_in intensity, where firm capabilities compound over time (Dosi §4b: technological regimes with Schumpeterian entry barriers). Tariff shocks on these sectors → LARGEST persistent capability disruption. (b) Infrastructure-strategic sectors (ICT infrastructure, energy networks) = network hub products in the bipartite matrix (intermediate goods connecting many other products' production chains). Tariff disruptions ripple through via the input-output linkages (Teti_2025 §5h mechanism). (c) Dependency-strategic sectors (rare earths, photovoltaics, mobile phones) = products where Chinese firms have near-monopoly export shares = HIGH RegDependency. These are precisely the products where the chokepoint effect (Farrell-Newman §5f) is most potent.
  2. **EU strategic dependency = demand-side mirror of RegDependency.** The EU's dependency on China for 204 products (Arjona §5i) IS the demand-side manifestation of the project's RegDependency moderator. From the EU's perspective: CDI1 (high concentration of imports from China) = the destination d concentrates its imports from China. From the Chinese firm's perspective: high export concentration to destination d = high RegDependency. These are the SAME underlying trade relationship measured from opposite sides. The CDI thresholds (HHI ≥ 0.4, extra-EU share ≥ 50%, imports > EU exports) provide concrete benchmarks for what constitutes HIGH RegDependency in the project.
  3. **OSA and d_out dynamics.** The EU's Open Strategic Autonomy (OSA) policy agenda explicitly aims to REDUCE dependency on China by: (a) diversifying import sources (find alternative suppliers), (b) building internal EU production capacity. From the Chinese exporters' perspective, this is a demand shock to their high-RegDependency markets. Chinese firms that rely heavily on EU markets for dependency-strategic products (photovoltaics, batteries, rare earth magnets) face a structural reduction in EU market access — a long-run version of the tariff shock in the project. These firms must EITHER consolidate their capability advantage (d_in = become more technologically advanced to remain indispensable) OR diversify to alternative destinations (d_out = shift to non-EU markets like Southeast Asia, Africa, Latin America). The project's framework captures exactly this dynamic.
  4. **IRA/EU Green Deal = tariff-equivalent shocks outside the project's sample.** The Inflation Reduction Act's local-content requirements (clean energy equipment must have US-made components to qualify for tax credits) function as tariffs on Chinese solar panels and batteries. The EU Chips Act similarly aims to relocate semiconductor production away from Asia. These policies operate on the same MECHANISM as the project's tariff treatment variable but are post-2022 (outside the 2000-2015 sample). The project's identification strategy GENERALIZES to these policy-equivalent mechanisms: the same capability reorganization logic applies.
  5. **"No strategic autonomy without fiscal autonomy" = the fiscal-capability link.** Fontana-Vannuccini argue that EU industrial capability development requires permanent fiscal capacity. For the project: Chinese REGIONAL fiscal capacity (coastal vs. inland provinces' ability to subsidize firm adaptation) is the Chinese analog of EU fiscal capacity heterogeneity. SOEs receive state subsidies regardless of fiscal capacity (Guariglia §5b), but private firms in low-fiscal-capacity regions face the LARGEST capability adjustment costs when tariff shocks hit. The EUSI's pattern — large countries with fiscal capacity (France, Germany) in all IPCEIs; small low-capacity countries excluded — directly parallels the pattern in China: coastal private firms in high-fiscal-capacity provinces (Guangdong, Zhejiang) are better positioned to execute d_out than inland firms.

---

### Arjona, Connell & Herghelegiu (2023) — "An Enhanced Methodology to Monitor the EU's Strategic Dependencies and Vulnerabilities"
*European Commission DG GROW Single Market Economics Papers WP2023/14* — **204 strategic dependent products; CDI methodology; ~19% face Single Point of Failure risk; China = 64 products (>50% by value)**

- **Research question.** Improving the European Commission's (2021b) benchmark methodology for identifying EU strategic product dependencies. The paper introduces three upgrades: (1) re-export-corrected trade data; (2) dynamic 4-year window rather than single-year snapshot; (3) complementary threshold + top-10% rank approach rather than thresholds alone. Applies to ~5,400 HS6 products, focusing on strategic industrial ecosystems.

- **Core Dependency Indicators (CDIs).** Three indicators applied to the TRADE-FIGARO-EUROSTAT database (corrects for re-exports, HS6 level):
  - **CDI1 = HHI of EU imports by source country**: CDI1 = Σ(si)², where si = market share of extra-EU country i in EU imports of product k. Threshold: 0.4 (equivalent to ≤2.5 effective suppliers). Captures: LOW import diversification.
  - **CDI2 = extra-EU imports / total EU imports**: Captures how important foreign sources are for the EU = EU scarcity index. Threshold: 0.5 (≥50% from outside EU).
  - **CDI3 = extra-EU imports / total EU exports**: Captures whether EU production capacity can substitute for imports. Threshold: 1.0 (imports exceed EU total export value = domestic production insufficient). Captures: LOW substitutability.
  
  Products classified as dependent if BOTH: (a) satisfy all three CDI thresholds AND (b) appear in the top 10% of an aggregate rank combining all three CDIs.

- **Dynamic identification rule.** Product classified as EU-foreign-dependent if it appears in the dependency list in 2020 AND/OR in 2 of the 3 prior years (2017, 2018, 2019). This ensures STRUCTURAL (persistent) dependencies are captured, not one-off disruptions.

- **Results: 204 strategically dependent products.** From 564 total foreign-dependent products (across all ecosystems), 360 are filtered out (agri-food, non-strategic textiles, construction materials, luxury goods), leaving 204 in sensitive strategic ecosystems:
  - **By HS section**: Chemicals/allied industries 43%, Mechanical appliances/electrical equipment 14%, Base metals 12%, Mineral products 11%, Precision/medical instruments 6%.
  - **By ecosystem**: Energy-intensive industries (manganese, nickel, aluminium, chromium, rare earths, molybdenum, borates, silicon, permanent magnets, uranium); Health (heterocyclic compounds, vitamins, alkaloids, amino-acids, medical instruments, surgical gloves); Renewables (photovoltaic cells, LED lamps, raw materials for batteries); Digital (laptops, mobile phones, monitors, projectors); Defence (navigational instruments, radio receivers, generators).
  - **By origin**: China = source for 64 products (31% by number), accounting for **>50% of the import value** of all 204 dependent products. US = 38 products (19%), 9% by value. Russia = 15 products (7%), 3% by value.

- **Single Points of Failure (SPOF) methodology.** For each of the 204 dependent products, the global SPOF risk is assessed using two indicators:
  1. **Weighted outdegree centrality std. dev.**: C_k^SD = std(C_i,k^w) where C_i,k^w = Σ_j(w_{ij,k}/w̄_j^k) / (n-1). Measures risk from having few CENTRAL exporters dominating the global trade network for product k.
  2. **HHI of world exports**: Global production concentration for product k.
  
  Combined into a single average rank → products distributed into deciles. ~19% of 204 products are in the highest SPOF risk decile (decile 10): antibiotics, laptops, parts of computers, mobile phones, radio broadcast receivers, LED lights, medical apparatus, tents/blankets. Only 6% in the lowest SPOF decile.

- **Key finding: SPOF risk is not uniformly distributed.** Products in the highest SPOF decile are those where Chinese production is most globally concentrated AND China is most central to global trade networks for that product. These are exactly the products where: (a) alternative suppliers are fewest (CDI1 high); (b) Chinese exports substitute for EU production capacity (CDI3 high). The SPOF metric = the global supply network version of the BRIM block's centrality measure.

- **Methodological genealogy.** Cites Korniyenko et al. (2017) — who defined the original SPOF methodology using network outdegree centrality — as the primary predecessor. Korniyenko_2017 (Batch 5j) is the next paper to read and directly precedes this methodology.

- **Relevance to project.** Five direct implications:
  1. **CDI methodology = formal operationalization of RegDependency.** The project's RegDependency measure (UN COMTRADE bilateral import concentration = how much destination d depends on China for product p) is structurally equivalent to the EU-focused CDI methodology:
     - CDI1 (import concentration at destination = HHI of sources) corresponds to RegDependency's concentration component
     - CDI2 (share of imports from outside vs. total) corresponds to the dependence intensity component
     - CDI3 (imports vs. domestic production capacity) corresponds to the substitutability component
     Together, the Arjona CDI framework provides THEORETICAL GROUNDING for the project's RegDependency construction: a destination d has HIGH RegDependency on China if the same three conditions hold (concentrated imports from China, high external reliance, low domestic substitutability).
  2. **SPOF metric = capability block centrality.** The SPOF risk measure (outdegree centrality std. dev. + HHI of world exports) captures how central a product is in GLOBAL trade networks AND how concentrated its production is. Products in decile 10 (highest SPOF) are those where Chinese firms' BRIM capability blocks have the highest global network centrality. In the bipartite firm-product network, these are products where firm-level RCA = 1 is most concentrated among Chinese high-capability firms. The project should test: do products with HIGH global SPOF risk show LARGER d_in responses to tariff shocks (firms consolidating their central position) or LARGER d_out (firms diversifying away from their exposed specialty)?
  3. **204 dependent products define the scope of HIGH RegDependency.** The EU's identified 204 strategic dependent products — 43% chemicals, 14% machinery/electrical equipment, 12% base metals — ARE the products where Chinese firms have highest RegDependency toward EU destinations. By construction (CDI1 ≥ 0.4 means ≤2.5 effective suppliers), these are products where China is the near-monopoly supplier. For the project: Chinese firms exporting these 204 products to EU destinations are the HIGH-RegDependency subgroup. The project can USE the Arjona product list to construct a categorical version of RegDependency (high = Arjona listed, low = not listed) as a robustness check on the continuous RegDependency measure.
  4. **Re-export correction = important for tariff measure accuracy.** Arjona shows that not treating re-exports leads to an ~27% underestimation of EU dependencies. The same re-export bias affects tariff measurement: if Chinese goods are routed through intermediate countries (e.g., Vietnam, Taiwan) to avoid tariffs or to obtain preferential access, the OBSERVED tariff rate in the Teti GTD may not reflect the EFFECTIVE tariff on the ultimately Chinese-origin product. The Arjona methodology alerts the project that Chinese exports routed through third countries may artificially REDUCE apparent RegDependency (imports appear to come from Vietnam, not China). This is exactly the "trade deflection" issue studied in Teti_2019 (§5g). For the project: constructing RegDependency using raw COMTRADE data may systematically understate true Chinese market dependence for products where Chinese firms route exports through third countries.
  5. **Dynamic 4-year methodology → structural vs. transitory dependencies.** Arjona's requirement that a product appear as dependent in the 2020 snapshot AND/OR in 2 of 3 prior years ensures only STRUCTURAL dependencies are captured. This is the supply-side analog of the project's BRIM partition stability criterion: firms whose BRIM block membership is stable across years (not just in one cross-section) are the ones with genuine, entrenched capabilities. The project should similarly distinguish: (a) STRUCTURAL capabilities (firms persistently in the same BRIM block across ≥3 years pre-shock) vs. (b) MARGINAL capabilities (firms in a block only 1-2 years). Structural capabilities should show STRONGER d_in consolidation under tariff shocks (harder to break) and weaker d_out (less incentive to search for alternatives).

---

### Cross-paper synthesis (§5i)

**1. Fontana_2024 + Arjona_2023 + Farrell-Newman (§5f) form a complete framework for understanding strategic trade dependencies.** Farrell-Newman (§5f) provides the geopolitical MECHANISM (weaponized interdependence via hub-and-spoke networks). Arjona (§5i) provides the EU-perspective EMPIRICAL MAPPING of which products are strategically dependent and on which suppliers (China dominant at >50% by value). Fontana (§5i) provides the POLICY RESPONSE framework (what EU does to reduce dependency = OSA agenda). For the project: all three perspectives converge on the same trade relationship, measured from different angles. The Farrell-Newman chokepoint effect + the Arjona SPOF risk + the Fontana OSA-driven d_out pressure all point to the SAME set of high-RegDependency Chinese firms as the most affected by trade policy shocks.

**2. Ding-Dafoe three logics + BRIM capability blocks = a joint classification system.** The Ding-Dafoe three-logic framework (cumulative, infrastructure, dependency-strategic) provides a THEORETICAL BASIS for classifying BRIM capability blocks by their strategic nature:
  - **Cumulative-strategic BRIM blocks** (high-tech manufacturing: electronics, machinery, pharmaceuticals) → d_in is the dominant response to shocks (defend the capability advantage that took years to build)
  - **Infrastructure-strategic BRIM blocks** (intermediate inputs: chemicals, base metals, rare earths) → tariff shocks propagate through input-output linkages (Teti_2025 input amplification mechanism); d_in consolidation + supplier diversification
  - **Dependency-strategic BRIM blocks** (products with few global substitutes: photovoltaics, permanent magnets, specific APIs) → d_out necessity is largest (when Western markets impose tariffs on your monopoly products, diversify to new markets) AND d_in consolidation (maintain technological edge to stay indispensable)
  This classification predicts HETEROGENEOUS d_in/d_out responses across blocks beyond just within-block fitness rank × tariff (from §5d Aghion).

**3. CDI methodology + RegDependency = complementary measures of the same structural dependency.** Arjona measures it from the EU importer's perspective (how concentrated is the EU's import basket?); RegDependency measures it from the Chinese exporter's perspective (how concentrated is the firm's export basket at the destination?). In equilibrium, these should be correlated — EU high-CDI products are Chinese high-RCA products. The project can validate its RegDependency construction by checking: do Chinese firms exporting Arjona's 204 products to EU destinations show higher measured RegDependency than firms exporting non-listed products? This is a direct out-of-sample validation test.

**4. Re-export bias in Arjona (27% underestimation) + Teti_2019 trade deflection finding = measurement challenges for the Bartik instrument.** Both papers highlight that tariff/dependency measures based on raw bilateral trade data may misattribute the origin of goods when third-country routing is used. For the Bartik instrument: if Chinese firms route exports through Vietnam or Taiwan to avoid US/EU tariffs, the OBSERVED tariff on Chinese exports understates the TRUE tariff shock facing Chinese firms. This creates ATTENUATION BIAS in the first stage of the Bartik instrument. The project should: (a) use Teti GTD's corrected effective tariffs (which account for preferential access via FTAs more carefully); (b) check robustness by restricting to products where Teti_2019 showed trade deflection is unlikely (machinery/electrical equipment: lowest deflection scope).

**5. Fontana's OSA + Rivera-Batiz-Romer (§5e) + Teti_2025 (§5h) = the long-run capability consequences of geopolitical trade policy.** Rivera-Batiz-Romer showed that trade restrictions have PERMANENT growth effects via the scale of the R&D engine. Teti_2025 quantified that trade war costs are small in the short run (−0.1% US real income) but could compound if made permanent. Fontana shows that the EU's strategic autonomy agenda is explicitly designed to BE PERMANENT — not a temporary exception but an institutionalised framework for technology sovereignty. For Chinese firms: the EU's OSA agenda is NOT a reversible tariff shock but a structural reduction in market access for dependency-strategic products. Rivera-Batiz-Romer's permanent growth suppression mechanism applies. The project's event study window (2-5 years post-shock) captures only the short-run adjustment; the long-run welfare costs predicted by Rivera-Batiz-Romer would require a much longer time series.

---

## §5j — Supply-chain bottlenecks, trade network fragility, and the new industrial policy wave (Batch 5j)

*Papers read in full 2026-06-05: Korniyenko, Pinat & Dew (2017) "Assessing the Fragility of Global Trade: The Impact of Localized Supply Shocks Using Network Analysis"; Evenett, Jakubik, Martín & Ruta (2024) "The return of industrial policy in data."*

Batch 5j closes the supply-chain / strategic-dependence arc opened in §5f (Farrell-Newman, Garicano) and §5i (Fontana, Arjona). Korniyenko et al. operationalise *where* global trade is structurally fragile — which products are genuine chokepoints — using network analysis on the full BACI trade matrix. Evenett et al. document *what governments are doing about it* — the NIPO dataset catalogues the 2023 wave of new industrial policy with motive tagging, instrument taxonomy, and tit-for-tat dynamics. Together they provide the supply-side fragility map and the policy-response measurement tool that the project needs to move from theoretical chokepoint exposure (Farrell-Newman) to empirically tractable treatment variation.

---

### Korniyenko, Pinat & Dew (2017) — "Assessing the Fragility of Global Trade: The Impact of Localized Supply Shocks Using Network Analysis"
*IMF Working Paper WP/17/30*

- **Main contribution.** The paper develops the first systematic, product-level measure of global trade fragility grounded entirely in network topology. Rather than measuring vulnerability through trade volumes or geographic concentration alone, the authors characterise each product's trade network by three structural properties: the presence of dominant central players (star-shaped exporters), the tendency to cluster (regionally compartmentalised trade), and low international substitutability (product differentiation making alternative sourcing costly). A k-median classification assigns each of 3578 intermediate and capital goods to four risk tiers, with the riskiest tier (Group 4) averaging 655 products per year. The approach inverts the conventional dependence-through-concentration lens: a product can be fragile even if trade value is not concentrated, if the network is topologically star-shaped and geographically segmented.

- **Data and method.**
  - *Database:* BACI bilateral trade data, HS2002 6-digit, 2003–2014; 5224 products and 223 countries before cleaning. Final products dropped to 3578 after excluding consumer goods (760 BEC products), final food/beverages (429 products), HS reclassification mismatches (416 products), and products not continuously observed. Crude and refined oil excluded.
  - *Component 1 — Presence of central players.* For each product-year, a weighted bipartite export network is constructed. **Weighted outdegree centrality** measures a country's export intensity to all its partners (exports to partner / partner's total imports of the product). The standard deviation of weighted outdegree centrality across countries in the product network captures how star-shaped it is: high SD = one or a few dominant exporters, low SD = flat (fully connected). Higher SD = higher fragility on this dimension.
  - *Component 2 — Tendency to cluster.* Two measures are combined: (i) the **weighted average local clustering coefficient** — the probability that trade partners of a country for this product also trade the product among each other (captures regional trading blocs); and (ii) the **network diameter** — the maximum geodesic distance (in hops) between any two countries in the network. The product of the two quantities captures both the tightness of clusters and their isolation from the rest of the world. Larger product → more fragile (harder to find a substitute source outside the cluster when a shock hits the cluster's dominant node).
  - *Component 3 — International substitutability.* Proxied by a **Revealed Factor Intensity (RFI)** measure adapted from Shirotori, Tumurchudur & Cadot (2010). The dispersion of human capital levels across a product's exporters proxies the heterogeneity of production methods. A wide human-capital distribution means that potential alternative suppliers are dissimilar, making substitution technically and institutionally costly. Higher dispersion = lower substitutability = higher fragility.
  - *Classification.* k-median procedure applied to standardised scores of all three components. One cluster emerges naturally as scoring high on all three dimensions simultaneously — defined as Group 4 (risky). Products in other clusters fail at least one dimension (e.g., high clustering but low centrality, or central but easily substitutable).

- **Key findings.**
  1. **655 products consistently risky; 421 persistently so over 2003–2014.** The 421-product persistent core spans machinery and mechanical appliances (HS 84, 85), transport equipment (HS 87, 88), pharmaceutical products (HS 30), rubber articles (HS 40), and precision instruments (HS 90). Together these sectors account for >38% of the risky group but only ~17% of the full sample — strong overrepresentation of capital goods and manufactures in the fragile set.
  2. **Top-10 risky products by import value include computer storage units (0.96% of world imports), aeroplane parts (0.76%), motor vehicle body parts (0.72%), antisera/blood fractions (0.67%), diesel engines, static converters, turbojet parts, and medical instruments.** These are not niche products — they are central to manufacturing supply chains globally.
  3. **Country-level import vulnerability is highly heterogeneous.** Average: 25% of imports are fragile products. Supply-chain countries, which import intermediates for assembly and re-export, exceed 30%: Mexico (37%), Hungary (36.2%), Romania (34.2%), Slovakia (34%), Czech Republic (33.9%), Germany (30.8%). Many of Italy's peer Central-Eastern European export competitors sit in this high-vulnerability tier.
  4. **Risky product exports are hyper-concentrated.** G8 countries export 59.7% of globally fragile products; the top four are the US (13.1%), Germany (13.0%), Japan (8.6%), and China (7.9%). The remaining countries exporting meaningful shares are all upper-middle or high income. Africa is represented only by South Africa, Egypt, Tunisia, and Morocco combined at <1%.
  5. **Case-study validation (Japan 2011, Thailand 2011).** The Japan earthquake disrupted diesel engines (HS 840890), aluminium capacitors (HS 853229), and LCD screens (HS 901380). The methodology correctly classified two of three products as Group 4 one year before the disaster. In Japan's case the diesel-engine network literally *lost its Japanese cluster* in 2011 (visible in the network visualization), and French automakers delayed launches due to missing components. Thailand floods disrupted hard drives (HS 847170), semiconductors (HS 854121), and pickup trucks (HS 870421) — all three classified Group 4 one year prior; hard drives and semiconductors scored in the top percentiles on all three dimensions.
  6. **Cross-country panel regression: risky imports from disaster-struck countries ↔ own export growth.** Specification: within-group estimation, ln(export growth) as dependent variable; key regressor = share of total imports constituted by fragile goods from countries suffering a large natural disaster in period t-1 (RMIC). Sample: 2003–2014, 169 countries. **A 1 percentage point increase in RMIC is associated with a 0.7% decrease in the affected country's own exports in period t** (significant at the 15% level). The effect is robust to controlling for REER, total imports from impacted country, and share of risky imports generally. Crucially, importing risky goods from a non-impacted country shows no effect; importing non-risky goods from an impacted country also shows no significant effect — isolating the joint fragility × disruption channel.

- **Theoretical implications.** The paper gives network science content to the Farrell-Newman (§5f) concept of "chokepoint." Farrell-Newman's hubs in weaponized interdependence are exactly Korniyenko et al.'s high-SD outdegree centrality nodes. The addition of clustering (geographic compartmentalisation) and substitutability (human-capital heterogeneity) operationalises two dimensions of chokepoint quality that Farrell-Newman discuss qualitatively: *geographic concentration* of production and *technical barriers to substitution*. Together: a product is a chokepoint iff it is simultaneously hub-shaped, regionally compartmentalised, and technically non-fungible. The Arjona (§5i) CDI three-part test (supplier concentration, demand concentration, re-export correction) is a close conceptual relative; the key difference is that Korniyenko et al. are measuring *network topology* rather than *bilateral concentration ratios* — they capture fragility arising from structure (star shape + diameter), not just from current trade shares.

---

### Evenett, Jakubik, Martín & Ruta (2024) — "The return of industrial policy in data"
*The World Economy, 47: 2762–2788 (DOI: 10.1111/twec.13608)*

- **Main contribution.** The paper introduces the **New Industrial Policy Observatory (NIPO)** dataset — the first systematic, product-level inventory of new industrial policy (NIP) measures across 75 jurisdictions (94% of global GDP), covering January 2023. NIPO extends the Global Trade Alert (GTA) database in four key respects: (i) it distinguishes between strategic plans, policies/regulations, and firm-specific interventions; (ii) it records the officially stated government motive (national security, geopolitics, resilience, strategic competitiveness, climate change); (iii) it maps interventions to pre-specified strategic product groups at HS6-digit level; (iv) it expands the GTA's instrument taxonomy to include technology-specific trade and investment restrictions. The paper's empirical contribution is a set of PPML regressions establishing that IP usage in 2023 correlates with RCA (not market failures), prior IP by others (tit-for-tat), elections (political economy), government effectiveness, export concentration, and real exchange rate appreciation — patterns inconsistent with the pure market-failure efficiency rationale for IP.

- **Data and method.**
  - *NIPO database.* 2580 records covering measures announced or implemented since 1 January 2023; 71% are trade-distorting (1800 measures). Three levels: industrial plans/strategies (3.8%), policies/regulations (56.2%, 95.8% implemented), and firm-specific interventions (40.0%, 99.2% implemented). Coverage: 75 jurisdictions tracked by the GTA team (G20 core + additional countries); measures updated monthly.
  - *Inclusion criteria.* A measure enters NIPO if it satisfies at least one of: (a) stated motive is national security, geopolitics, security of supply (non-food), strategic competitiveness, or climate; (b) it affects products in the NIPO strategic product groups (low-carbon tech, dual-use, critical minerals, advanced tech, semiconductors, medical products, IT/digital services); (c) it is a multi-year industrial strategy or plan.
  - *IP determinants regressions.* **Sectoral specification (Eq. 1):** PPML of measures count (or dummy) at jurisdiction × HS6 level on log RCA (own sector), count of measures by other countries in the same sector in 2022 (tit-for-tat), with progressive country and country×HS2 fixed effects. **Country-level specification (Eq. 2):** PPML of measure count at jurisdiction × HS6 level on political economy (election year, government effectiveness, ideology), structural (export HHI, debt/GDP, private sector credit, sovereign debt rating, log GDP), and cyclical (GDP growth, REER growth) country-level variables, with HS6-digit fixed effects.

- **Key findings.**
  1. **2500+ NIPs in 2023; 71% trade-distorting.** Advanced economies (AEs) account for 70.9% of distortive measures; China, EU, and US jointly for 47.7%. The AE dominance is consistent with the 2009–2020 record from Juhász et al. (2023).
  2. **Instrument mix differs sharply by income group.** AEs use direct financial grants, state loans, and other state aid (heavy fiscal outlays). EMDEs use state loans, import tariffs, and tax relief — instruments that do not require direct fiscal expenditure. The gap likely reflects fiscal space constraints in EMDEs.
  3. **Sectoral focus in 2023: military/civilian dual-use (25.7%), advanced tech + semiconductors (20.6%), low-carbon technology (15.3%), steel and aluminium (10.1%), critical minerals (3.0%), medical products.** The medical sector dominated early in 2023 (COVID-era carry-over) but was overtaken by dual-use and advanced tech by mid-year.
  4. **Stated motives: strategic competitiveness (37.0%), climate (28.1%), supply chain resilience (15.2%), national security + geopolitics (19.7%).** AEs predominantly cite climate and geopolitics; EMDEs cite strategic competitiveness. The instrument of choice for climate is domestic subsidies; national security motives are addressed with a more varied mix including trade measures and procurement.
  5. **At least 21.6% of global imports are affected by inward distortive measures (lower bound).** Of the 474 measures with stated motives, strategic competitiveness covers the largest import value (8.6%), followed by climate (5.8%), supply chain resilience (4.6%), and national security/geopolitics (3.2% + 0.4%). The lower-bound nature is explicit: only measures with identifiable HS codes are counted (882 of 1576 inward measures).
  6. **Tit-for-tat dynamics: 73.8% probability of matching within 1 year.** Averaging over all six bilateral permutations of China, EU, and US, the probability that a subsidy by one major economy is matched by a subsidy in the same product by another within 12 months is 73.8%. Within 24 months this exceeds 80% in most permutations. The PPML regressions (Table 7) confirm a statistically significant positive coefficient on "measures by others in the same sector in 2022" across all fixed-effect specifications.
  7. **RCA positively correlated with IP intensity.** Governments systematically target sectors where their economy already has revealed comparative advantage — consistent with political economy capture (established producers lobby for defence of their position) rather than targeting sectors with market failures or growth potential. This replicates the Juhász et al. (2023) finding for 2009–2020 with fresh data.
  8. **Country-level determinants: elections, government effectiveness, export concentration, REER appreciation.** Countries facing elections in 2023 or 2024 use significantly more IP. Higher government effectiveness (administrative capacity) → more IP. Higher export concentration (higher HHI) → more IP. REER appreciation → more IP (competitiveness-defensive response). Counterintuitively, poorer sovereign debt ratings are positively correlated with IP use (the fiscal space argument predicts the opposite; the authors note this may reflect that indebted governments use subsidies as an easier political instrument than fiscal consolidation).

- **Theoretical implications.** The NIPO data establish that the current wave of industrial policy is not primarily driven by market failures — the pattern of which sectors are targeted (high RCA = established industries, not nascent ones) and which countries act (those facing elections, not those with the most market distortions) strongly suggests political economy capture and tit-for-tat dynamics dominate. This has a direct implication for the project: the Teti GTD tariff shocks are not occurring in a stable policy environment but in one where every major economy is matching others' interventions within months. The "treatment" in the project's event-study design is therefore not a single t-1 shock but a sequence of escalating shocks. Evenett et al. provide the tool to characterise this escalation at the sector-country level.

---

### Cross-paper synthesis (§5j)

**1. Korniyenko fragility index + Evenett NIPO = the supply-chain shock lifecycle.** Korniyenko et al. identify *where* the structural chokepoints are (products where star-shape topology + clustering + non-substitutability combine). Evenett et al. document *what governments do once they know* — they impose industrial policies targeting exactly the strategic sectors that correspond to Korniyenko's fragile products (machinery, electrical equipment, advanced tech, semiconductors, medical). The two papers together define a lifecycle: (a) trade network fragility creates dependence → (b) governments weaponize dependence (Farrell-Newman §5f) → (c) industrial policy measures proliferate (Evenett NIPO) → (d) firms face not just one tariff shock but an escalating policy environment. For the project, this means the Teti GTD shock variable captures only the first layer of a multi-round policy process; the Evenett tit-for-tat finding implies the shock will intensify over the event-study window.

**2. Korniyenko's Group 4 products overlap substantially with Arjona's CDI-dependent products.** Arjona (§5i) identified 204 EU-dependent products (by supplier concentration and single-point-of-failure logic). Korniyenko's consistently fragile 421 products are a superset that adds network topology to the concentration test. The intersection — products that are both CDI-dependent AND topologically fragile — defines the highest-chokepoint goods: where the dependence is structural (concentrated supplier) AND the structure is brittle (star-shaped, clustered, non-substitutable). For the project: Chinese firms exporting this intersection set face the most severe combination of: western import restrictions (strategic competitiveness motives, Evenett) + permanent EU OSA agenda (Fontana §5i) + genuine lack of alternative markets (RegDependency high, Korniyenko substitutability low).

**3. Evenett's RCA → IP correlation implies the project's heterogeneous treatment is not randomly assigned.** The finding that governments target high-RCA sectors means Chinese firms in high-capability sectors (top BRIM blocks in the EFC framework) face MORE intense industrial policy pressure than low-capability firms. This creates a capability-dependence channel that confounds identification: the most capable firms (highest complex-product share, highest EFC fitness) are both the firms the project expects to consolidate d_in (they have the most to protect) AND the firms targeted most aggressively by Western IP (because they export high-RCA, high-BRIM-fitness products). An IV approach using the Evenett election-cycle variable (or the matched tit-for-tat structure) could instrument the IP-driven component of the tariff shock separately from the ordinary trade policy component.

**4. Korniyenko's 0.7% export suppression effect + Teti_2025's −1.6% threshold calibrate the magnitude range.** Korniyenko find that a 1pp increase in risky imports from a disaster-struck country reduces the *importing* country's own exports by ~0.7% — this is a pure network-transmission effect with no policy intervention. Teti_2025 finds that Canadian and Mexican firms with high regulatory dependence experienced −1.6% real income effects from 2018 tariffs. These two estimates bracket the expected magnitude of the project's d_out response: supply-shock network effects alone generate ~0.7%; policy-driven tariff shocks to high-RegDep firms can generate ~1.6% or more. The project's baseline estimate for d_out should fall in this 0.7–1.6% range for moderate RegDependency, scaling up for the highest-exposure firms.

**5. The NIPO motive taxonomy operationalises the Ding-Dafoe three logics (§5i) as policy instruments.** Ding-Dafoe (§5i) distinguished three logics of capability blockade: cumulative, infrastructure, and dependency-strategic. The Evenett NIPO motive taxonomy maps onto these:
  - **Cumulative-strategic blocking** corresponds to "strategic competitiveness" and "national security" motives in NIPO → targets Chinese firms with high technological RCA in advanced manufacturing (semiconductors, precision machinery).
  - **Infrastructure-strategic blocking** corresponds to "supply chain resilience" motives → targets critical minerals, basic materials, industrial inputs.
  - **Dependency-strategic blocking** corresponds to "geopolitical concerns" → sanctions, export controls, FDI screening targeting Chinese entities in dual-use products.
This three-logic to three-motive mapping means the NIPO motive variable can be used to split the sample of tariff shocks in the Teti GTD into theoretically grounded sub-types, allowing the project to test whether the capability response (d_in vs. d_out) differs across blockade logic — a direct test of the Ding-Dafoe taxonomy.

---

## §5k — Strategic Dependencies: EU-Level Mapping and In-Depth Reviews

### European Commission (2021) — "Strategic Dependencies and Capacities"
*Commission Staff Working Document SWD(2021) 352 final, Brussels, 5 May 2021. Accompanying COM(2021) 350 final — Updating the 2020 New Industrial Strategy.*

- **Main contribution.** The document provides the European Commission's first systematic, product-level quantification of EU strategic dependencies, combining a bottom-up trade-flow mapping (5,000+ HS6-digit products) with in-depth technology and sector reviews. Three conceptual innovations define its contribution to the literature:
  (i) **The Core Dependency Indicators (CDI) framework** — a formal, replicable three-indicator methodology to identify foreign dependencies, which becomes the methodological precursor to the Arjona (§5i) operationalisation;
  (ii) **The distinction between external and internal dependencies** — external (dependence on third-country suppliers) vs. internal (Single Market concentration at firm level), with different policy implications for each;
  (iii) **The concept of Open Strategic Autonomy (OSA)** — the EU should remain open to trade and GVCs while building targeted strategic capacity in a narrow set of sectors where dependence creates unacceptable vulnerability. This concept defines the EU's policy posture in subsequent legislation (Critical Raw Materials Act, EU Chips Act, Net-Zero Industry Act) and provides the political economy frame within which the project's tariff shocks unfold.

- **Data and method.**
  - *Universe:* Full BACI database, HS6-digit level, all bilateral trade flows; ~5,000 products across 14 industrial ecosystems.
  - *CDI1 — Supplier concentration:* HHI on extra-EU import shares. Threshold: HHI > 0.4 (implying effective import base ≤ 2.5 countries). Note: more conservative than the standard HHI > 0.25 threshold used in competition economics.
  - *CDI2 — Extra-EU import intensity:* extra-EU imports / total EU imports > 0.5 (majority of supply from outside EU).
  - *CDI3 — Substitutability with EU production:* extra-EU imports / total EU exports > 1 (EU exports cannot cover import volume — EU production is structurally insufficient or structurally different).
  - *Step 1:* Apply all three CDIs to full 5,000-product universe → ~390 dependent products.
  - *Step 2:* Restrict to "sensitive ecosystems" (energy-intensive industries, health, renewables, digital/electronics, aerospace & defence) → 137 dependent products.
  - *Step 3:* Qualitative stratification of strategic nature → case-by-case expert assessment.
  - *Vulnerability screen (Chapter 2.4):* Of 137, identify a "high-vulnerability" subset using (a) world-level HHI > 0.4 for exports of the product (low diversification potential) AND (b) price gap between EU exports and extra-EU imports ≥ 30% (low substitution potential) → **34 especially vulnerable products**.
  - *In-depth sector reviews (Chapter 5):* Qualitative + firm-level data (FactSet supply chain database) for six priority areas: critical raw materials, active pharmaceutical ingredients (APIs), Li-ion batteries, hydrogen, semiconductors, cloud/edge computing.

- **Key findings.**
  1. **137 products in sensitive ecosystems are EU-dependent; these represent ~6% of extra-EU import value.** In terms of processing stages: 16% raw materials, 57% intermediate goods, 27% final goods. This distribution reveals that strategic vulnerability is primarily an intermediate-goods problem — not a raw-material problem alone.
  2. **China dominates: ~52% of EU import value for dependent products; top-3 supplier for 54% of them.** Vietnam and Brazil are the next-largest sources, both far behind. For the project: Chinese firms are the dominant export-side counterpart of exactly these 137 dependent products — they face the maximum concentration of EU demand and the maximum EU interest in reducing that dependence.
  3. **34 most-vulnerable products: near-zero substitutability and near-zero diversification potential.** These include specific APIs (alkaloids, heterocyclic compounds), ferro-alloys (ferro-tungsten, ferro-niobium), precision products (turbo-propellers), and COVID-related goods. These are the highest-severity end of the RegDependency distribution in the project's framework.
  4. **Reverse and common dependencies (Box 4): EU and US share many dependencies on China.** Using CDI1 and CDI3 (without CDI2, which is EU-specific), the analysis shows that both the EU and US depend on China for health ecosystem goods (vitamins, antibiotics, hormones) and green/digital transition products (permanent magnets, electric accumulators, mobile phones, radio receivers). This shared dependence explains the observed US-EU policy coordination: the Teti tariff shocks from both blocs target the same product set because both face the same structural vulnerability.
  5. **Critical raw materials: China supplies 98% of EU rare earth elements, Turkey 98% of borates, South Africa 71% of platinum group metals.** Export restrictions on cobalt, rare earths, and tungsten covered >70% of global production as of 2018. EU produces just 1% of battery raw materials despite planning for 400 GWh domestic demand by 2028.
  6. **Active pharmaceutical ingredients (APIs): China provides ~45% of extra-EU API import volume; 80% comes from China, US, UK, Indonesia, India.** 93 out of 554 APIs with valid EU quality certificates (CEPs) have no European production at all. For APIs with CEPs, two-thirds of holders are Asian, and for more than half of marketed APIs there are only 1–5 manufacturers globally holding a CEP.
  7. **Li-ion batteries: EU held 3% of global Li-ion cell production in 2018 (China: 66%, South Korea+Japan+others: ~30%).** EU needs 7–18× more lithium and 2–5× more cobalt by 2030 (low-demand scenario). Asia accounts for 84% of processed battery materials and components.
  8. **Semiconductors: EU accounts for ~10% of global revenues; ~6% in computing and communications.** No EU foundry manufactures below 22nm; in 2020 only TSMC (Taiwan) and Samsung (South Korea) produce at 5nm. EU strength lies in automotive/industrial micro-controllers (37% global share), power electronics, and sensors. Full structural dependence on US for chip design tools (electronic design automation); full dependence on TSMC/Samsung for leading-edge fabrication.
  9. **Cloud/edge computing: top-4 non-EU hyperscalers (AWS, Microsoft Azure, Google Cloud, Alibaba) control >80% of global cloud revenues.** Largest EU provider holds <1% of European market. Annual EU–competitor investment gap: EUR 11 billion. Only 36% of EU enterprises used cloud services in 2020; less than half of those use advanced cloud. Vendor lock-in, interoperability gaps, and foreign-jurisdiction data-access risks are identified as the structural drivers of the dependency.
  10. **Technology assessment (Chapter 3): EU is strong in advanced manufacturing and selected green technologies (hydrogen electrolysers, offshore wind), but falling behind in AI, big data, cloud, cybersecurity, industrial biotech, micro-electronics, and robotics.** China overtook EU in top-1% highly cited publications in 2015; Chinese BERD has caught up in monetary terms (EU BERD ~200 bn EUR in 2019, but US BERD 45% higher). In software & internet, US has 8.8× more R&D-active firms and 12× higher R&D investment than EU.

- **Methodological contribution: the CDI framework and its relationship to Arjona (§5i).**
  The Arjona CDI methodology (three indicators: CDI-concentration, CDI-demand, CDI-substitutability) is directly derived from this document — indeed the Arjona paper cites EUC_2021 as its methodological precursor. The key refinements Arjona introduces over EUC_2021 are: (a) adding a re-export correction to CDI3 (EU exports include re-exports that should not count as domestic production capacity); (b) tightening the HHI threshold from 0.4 to a stricter cutoff; (c) updating to more recent data years. For the project: EUC_2021 is the original EU official quantification of the product space within which the Teti tariff shocks occur; Arjona (2023) is the refined academic operationalisation of the same product space. The 137 EUC products and the Arjona 204 CDI-dependent products are overlapping but not identical — EUC_2021 is more conservative (HHI threshold 0.4, sensitive ecosystems only), Arjona is more comprehensive in scope but uses refined substitutability logic.

- **Theoretical implications.**
  The document's most important contribution to the project is the concept of **Open Strategic Autonomy (OSA)** as the policy frame that generates the EU's industrial policy response. OSA differs from pure protectionism in a precisely defined way: the EU does not seek to exit GVCs but to reduce dependence on *specific* products from *specific* suppliers where (a) concentration is high (CDI1), (b) extra-EU sourcing dominates (CDI2), and (c) internal substitution is structurally impossible (CDI3). This framing implies that EU industrial policy — and therefore the Teti tariff shocks — is targeted: not a blanket trade war but a product-specific response calibrated to CDI scores. For the project this means RegDependency is not a continuous covariate but effectively a treatment intensity that the EU has explicitly quantified: Chinese firms exporting products in EUC_2021's 137 list face an EU policy apparatus that has formally identified them as targets for dependency reduction. The OSA frame further implies that the EU's preferred policy tool is not tariffs alone but a mix of tariffs + reshoring subsidies + diversification partnerships — which means the Teti GTD tariff variable captures only one instrument in a coordinated multi-instrument policy response. For the project's interpretation of treatment-effect heterogeneity, firms producing the EUC-identified dependent products face both a tariff shock AND a structural EU demand-reduction incentive (OSA reshoring target), while firms outside the 137-product set face only ordinary trade policy.

---

### Cross-paper synthesis (§5k)

**1. EUC_2021 CDI methodology → Arjona CDI → project RegDependency variable: the methodological chain.** EUC_2021 defines the three CDIs and applies them to identify 137 dependent products. Arjona (2023) refines the methodology and narrows to 204 CDI-dependent products with the re-export correction. The project's RegDependency variable operationalises firm-level exposure to the Arjona product list: for each Chinese firm, the share of its export basket that falls in the Arjona dependent product set (or the EUC-137 set, depending on data vintage). The full chain from EU official policy document → academic refinement → firm-level exposure variable is thus established.

**2. EUC_2021's 137 products ∩ Korniyenko's 421 fragile products ∩ Evenett NIPO strategic sectors = the extreme-RegDependency cell.** These three product sets overlap non-trivially. The intersection defines firms that are simultaneously: (a) in products where EU has officially declared strategic dependence and is actively reshoring (EUC); (b) in products with star-shaped network topology and low substitutability (Korniyenko); (c) in sectors where 73.8% of industrial policy measures are matched within 12 months (Evenett). Chinese firms whose export basket concentrates in this intersection face the most structurally hostile export environment — the hypothesis that they would undergo the sharpest d_in consolidation and/or the largest d_out contraction follows from this triple-overlap classification.

**3. EUC_2021's "common dependencies" finding explains why US-EU trade policy coordination amplifies the shock.** Box 4 of EUC_2021 shows that the EU and US share a large set of China-dependencies. This means the Teti GTD captures correlated shocks from multiple blocs rather than independent bilateral shocks. For identification: if US tariffs and EU CDI-driven reshoring actions are both triggered by the same underlying product-level exposure to China, then the Teti variable is likely correlated with a broader "Western-bloc strategic concern" factor. An instrumental variable for the Teti tariff (the project considers Bartik-style Fontagné weights) must account for this correlation structure — the tariff is not randomly assigned across products but follows the EUC CDI score.

**4. The CDI3 substitutability indicator operationalises the "lock-in" mechanism in Farrell-Newman (§5f).** CDI3 > 1 means EU domestic production cannot replace imports even if it were fully redirected to the dependent product. This is the quantitative expression of Farrell-Newman's vulnerability condition: weaponisation works precisely because the target cannot rapidly substitute domestically. The 34 "most vulnerable" products (CDI3 >> 1 AND world HHI > 0.4) are the ones where weaponisation threat is most credible — these are the products where EU is structurally captive even in the medium run. For Chinese firms: these 34 products are simultaneously the highest-value leverage products (EU cannot exit dependence quickly) and the highest-risk export products (EU has the strongest political motivation to reduce dependence regardless of cost).

**5. EUC_2021's semiconductor findings position the project's BRIM community detection in the technology landscape.** The document shows EU's competitive strength is in automotive micro-controllers and power electronics (not leading-edge processors or design tools). These are exactly the product categories that appear in the EFC product space's mid-complexity clusters — complex enough to require accumulated capabilities (Bell, March, Dosi) but not so frontier that only TSMC or Samsung can produce them. Chinese firms with BRIM community memberships in mid-complexity manufacturing (HS chapters 84–85) are in the sweet spot: products where EU depends on China (CDI-dependent), EU has some domestic capacity but below import volume (CDI3 modestly above 1), and EU's reshoring strategy (IPCEI, Raw Materials Alliance) aims to close the gap over 5–10 years. The event-study window in the project (2016–2022) covers precisely the period when EU-OSA policy was being formulated (EUC_2021) but before full reshoring capacity came online — which implies the tariff shocks during this window created maximum uncertainty about future demand conditions for Chinese firms in these sectors.

---

## §5l — OSA Foresight: Scenarios, Political Economy Rationale, and 2040 Trajectories

### Cagnin, Muench, Scapolo, Störmer & Vesnic-Alujevic (2021) — "Shaping and Securing the EU's Open Strategic Autonomy by 2040 and Beyond"
*JRC Science for Policy Report. EUR 30802 EN, JRC125994. Publications Office of the European Union, Luxembourg, 2021. doi:10.2760/414963.*

**Note on filename:** This document is filed as `JRC_2025.pdf` in the project's Papers folder, but the publication date is 2021. The report accompanies the same 2021 Commission foresight agenda that produced EUC_2021 (SWD(2021) 352). These two documents are companion pieces: EUC_2021 provides the quantitative product-level mapping; this JRC report provides the qualitative foresight, conceptual framing, and scenario analysis.

- **Main contribution.** The report provides the **political economy rationale and conceptual vocabulary** for the EU's Open Strategic Autonomy (OSA) policy agenda — the policy frame within which all tariff shocks, industrial policy measures, and FDI restrictions studied in the project are embedded. Three contributions stand out:
  (i) **OSA as managed interdependence, not autarky**: OSA is explicitly defined as "a means to an end, or to attaining the EU's long-term objectives. A process rather than an end-point." This framing distinguishes it from protectionism and explains why the EU's policy response is targeted rather than comprehensive — consistent with EUC_2021's 137-product mapping rather than a blanket trade war.
  (ii) **Four foresight scenarios for 2040** capturing the full range of possible EU-China trajectories, from continued interdependence (Complex Prosperity) to near-full decoupling (Retreat Inwards). These scenarios directly bracket the long-run expected treatment intensity facing Chinese exporters in the project's event-study window.
  (iii) **Delphi prioritisation (241 experts)** of OSA policy actions, revealing that "supply chain reconfiguration," "FDI screening/IPR control," and "level playing field in global trade" rank as the top economic priorities — confirming that the EU's policy arsenal extends well beyond tariffs into the multi-instrument treatment environment documented by Evenett (§5j) and Fontana (§5i).

- **Method.** Qualitative foresight process, not an econometric study. Methods include: (a) systematic desk research across five OSA dimensions (geopolitics, technology, economy, environment, society); (b) Oxford Scenario Planning Approach with multiple participatory workshops (November 2020–March 2021) involving European Commission services and external experts; (c) Online Delphi survey (241 experts scoring statements on impact, urgency, EU capacity, and likelihood); (d) Semi-structured expert interviews to validate findings. The report explicitly disclaims predictive validity — scenarios are "plausible" not "probable."

- **Key findings.**

  **1. EU's declining relative economic weight creates urgency for OSA.** EU27 GDP share: 18% in 2019 → 12.4% by 2040 (OECD projection at current prices). E7 economies (China, India, Indonesia, Russia, Brazil, Mexico, Turkey) will account for 41.2% of global GDP by 2040, growing 2× faster annually than G7. China alone projected to reach 22% by 2040. EU's economic power base for regulatory leverage is structurally eroding — the window for deploying market power to impose OSA conditions is closing, creating urgency for the 2021–2025 wave of industrial policy captured in the Teti GTD.

  **2. US-China rivalry is "cooperative rivalry" — fragmentation is likely but full decoupling is not.** Three possible world orders: (a) multipolar fragmentation with rules-based cooperation undermined; (b) two distinct US- and China-centric blocs with thin overlap; (c) continued interdependence with competition on specific issues. The report argues scenario (c) is most plausible in the near term — US and China are "too interconnected to split." This places an upper bound on how far Chinese firms actually exit Western markets in response to tariff shocks (partial equilibrium d_out, not full decoupling).

  **3. China's "dual circulation strategy" creates an independent push toward d_in consolidation.** The report cites China's strategy of "reducing export-dependence of its economy" and building domestic consumption as a growth driver. The EU analysis explicitly states: "The role of China as the EU's second biggest export market risks diminishing" as China reaches high-income country status by 2025. For the project: Chinese firms face simultaneous pressure from both sides — Western tariffs reduce the attractiveness of foreign markets, while Chinese domestic policy incentivises redirecting toward the domestic market. Both pressures independently predict d_in consolidation and d_out contraction.

  **4. Four scenarios for 2040 bracket the event-study treatment space:**
    - **Green Leadership** (~30% of world economy in like-minded clean-tech bloc): Chinese firms in carbon-intensive sectors face EU market exclusion; EU imports of Chinese intermediates drop as reshoring succeeds in batteries, wind turbines, and hydrogen. Maximum d_out contraction for Chinese firms in green-adjacent manufacturing sectors (HS 84, 85, 87).
    - **Complex Prosperity** (multilateral world, US+China lead, EU lags in innovation): EU remains structurally dependent on Chinese supply chains in most areas; tariff shocks are moderate and offset by continued GVC participation; d_out contraction is partial and d_in consolidation is gradual. This is the modal scenario for the 2016–2022 event-study window.
    - **Economic Growth Above All** (private interests dominate, global trade booms): EU-Africa-India alliances for raw materials; China under demographic/debt pressure but still dominant in rare earths (lithium demand 60× over 20 years); EU-China trade continues because economic growth overrides OSA concerns. Tariff shocks are negotiating tools rather than decoupling mechanisms — d_out is maintained but at lower margins.
    - **Retreat Inwards** (deglobalization; China explicitly limits rare earth exports in the late 2020s; "splinternet"): China weaponizes supply-side dependencies (the reverse of the project's treatment direction — China → EU rather than EU → China); EU-China decoupling accelerates; Chinese firms face permanent d_out contraction across all EU-exposed product categories. This scenario validates the Farrell-Newman weaponization prediction applied to China's strategic resources.

  **5. The EU's comparative advantage in OSA instruments is regulation and standards, not military power.** The report identifies EU's key strengths as: regulatory power (450M consumers), multilateral soft power, rules-based governance model. It explicitly identifies military power as the EU's weakest OSA dimension. This asymmetry explains the Evenett finding (§5j): the EU systematically uses trade and industrial policy (the one instrument where it has comparative advantage) rather than security measures. For the project: the treatment variable (tariffs + FDI screening + CDI-driven reshoring subsidies) is the EU's primary available instrument for OSA implementation, not one among many equivalent tools.

  **6. Five-dimension Delphi priorities confirm the multi-instrument treatment environment.** The 241-expert Delphi identifies the following top economic OSA priorities: supply chain reconfiguration, FDI screening and IPR protection, level playing field in global trade, and design of a new sustainable economic model. These map to four distinct policy instruments — tariffs (Teti GTD), FDI restrictions (EFSIR regulation), reshoring subsidies (IPCEIs, Raw Materials Alliance, Chips Act), and regulatory standards (CBAM, EU AI Act). Chinese firms in RegDependency-exposed sectors face all four instruments simultaneously. The Teti tariff variable captures only one of the four, implying attenuation bias in reduced-form estimates.

  **7. EU's digital and technology dependence creates a domestic pressure for OSA that parallels the trade shock.** EU has no foundry below 22nm (confirmed in EUC_2021); cloud: top-4 non-EU hyperscalers control >80% of revenues with €11B annual EU investment gap; AI: US has 43 unicorns vs EU aggregate much smaller. The report frames this as "technology dependence → future strategic dependency → urgency to act now." For the project: this domestic political economy pressure (EU electorates demanding action on technology sovereignty) is a supply-side driver of EU industrial policy that is orthogonal to any bilateral Chinese provocation — it would have happened regardless of whether China acted aggressively. This strengthens the case for treating the Teti tariff shocks as plausibly exogenous from the perspective of individual Chinese firms' behavior.

- **Theoretical implications.**
  The JRC foresight report provides three key inputs to the project's identification and interpretation strategy:

  **(a) Identification:** The report shows that EU OSA policy is driven by structural long-run concerns (declining relative economic weight, technology dependence, CRM concentration) that pre-date and are independent of any specific Chinese firm's export behavior. This supports treating the Teti tariff shocks as supply-side policy shocks rather than responses to Chinese firm-level competitiveness changes — a necessary condition for the event-study design's validity.

  **(b) Scenario-based treatment heterogeneity:** The four scenarios imply that treatment intensity is expected to vary systematically across product types. Firms in green/digital sectors face maximum long-run treatment (Green Leadership, Retreat Inwards); firms in non-strategic sectors face moderate treatment (Complex Prosperity). This product-sector heterogeneity can be operationalised as an interaction between the Teti tariff variable and the EUC_2021 CDI classification, generating a heterogeneous treatment design.

  **(c) Partial equilibrium ceiling on d_out:** The "cooperative rivalry" framing implies that neither the EU nor China will fully decouple in the project's event-study window. Chinese firms therefore face a partial adjustment — they reduce d_out but do not exit EU markets entirely. This creates the asymmetric response prediction: d_in consolidation (retrenchment to core BRIM capabilities) is more likely than full d_out exit, because some Western market access has strategic option value as a hedge against scenario uncertainty.

---

### Cross-paper synthesis (§5l)

**1. EUC_2021 (§5k) + JRC foresight (§5l) = the complete EU OSA system: measurement + rationale.** EUC_2021 answers "which products?"; JRC answers "why act?" and "what could happen?". The full reading of both documents establishes that the EU's strategic dependency response is (a) targeted at a specific product set (137 CDI-dependent goods), (b) driven by structural multi-dimensional concerns (geopolitics, technology, economy, environment, society — not just trade), (c) designed to be proportionate rather than comprehensive (OSA as managed interdependence), and (d) expected to intensify over the 2020–2040 horizon as EU's economic weight declines. For the project: the treatment is not a one-time tariff shock but the beginning of a permanent policy regime shift.

**2. The four JRC scenarios operationalise the Ding-Dafoe blockade logics (§5i) as distinct possible futures.** The Ding-Dafoe taxonomy (cumulative-strategic, infrastructure-strategic, dependency-strategic blockade) maps onto JRC scenarios: Green Leadership deploys cumulative-strategic blocking (targeting Chinese manufacturing capabilities through export controls and standards exclusion); Retreat Inwards manifests dependency-strategic blocking (both sides weaponise supply dependencies); Economic Growth Above All is the baseline where blockade logics fail to materialise because economic interdependence prevails. The scenario analysis thus turns the Ding-Dafoe taxonomy from a static classification into a dynamic process model.

**3. China's dual circulation strategy + EU OSA = bilateral convergence on reduced interdependence, independent of tariffs.** The JRC report notes China reducing export-dependence; EUC_2021 documents EU reducing import-dependence; Evenett (§5j) confirms 73.8% tit-for-tat escalation. All three converge on the prediction that Chinese firms in strategic sectors will face permanently reduced Western market access whether or not tariffs are specifically the mechanism. For identification purposes: the tariff shock (Teti GTD) is the observable event, but the underlying force is a bilateral policy regime shift. Firms that respond to the tariff shock (the project's treatment) are responding to the first measurable signal of a long-run process, not to a transient shock. This implies treatment effects should persist and potentially grow in magnitude in post-treatment periods — a testable implication in the event study.

**4. The JRC's "managed mutual interdependence" framing calibrates the expected magnitude of d_out.** If OSA is about reducing ONE-SIDED dependence rather than achieving full independence, then the EU's optimal policy generates moderate d_out (not full exit). Firms that drop below some threshold of European market exposure become irrelevant to EU strategic concerns — they lose leverage. Firms that remain above the threshold face continued policy pressure. This predicts a non-linear response: d_out drops sharply for firms with very high EU exposure (who face the strongest OSA pressure) and less sharply for firms with moderate exposure (who remain below the strategic concern threshold). The project should test for non-linearity in the RegDependency × tariff interaction.

---

## §5m — Firm-Level Response to Trade Restrictions: Extensive Margin and Export Diversity

### Crozet, Hinz, Stammann & Wanner (2021) — "Worth the Pain? Firms' Exporting Behaviour to Countries under Sanctions"
*European Economic Review 134 (2021) 103683. doi:10.1016/j.euroecorev.2021.103683*

- **Main contribution.** The paper provides the first firm-level causal analysis of how sanctions affect the **extensive margin of trade** — the probability that a firm continues to serve (or enters) a sanctioned market. Unlike aggregate-level studies, the firm-level approach allows identification of who exits, who stays, and why. Four episodes are studied: sanctions on Iran (January 2012) and Russia (August 2014), and the lifting of sanctions on Myanmar (May 2012) and Cuba (January 2015). The estimation uses a dynamic probit with three-way fixed effects (firm-time, destination-time, firm-destination) and bias-corrected average treatment effects on the treated (ATTs), drawing on the Hinz, Stammann & Wanner (2020) analytical bias correction for the incidental parameter problem in dynamic nonlinear models.

- **Data and method.**
  - *Data:* French customs data, monthly frequency, universe of French exporting firms, January 2009–December 2016. For each episode: two-year window before and after the sanctions event. ~35M observations per episode; ~150,000 firms exporting to up to 223 destinations over 48 months.
  - *Dependent variable:* Binary (0/1) indicator of whether firm ω exports to market j in month t. Zeros are constructed for firm-destination pairs where the firm was active in the market at least once over the sample and exported to any market in the same month.
  - *Three-way FE specification:* firm × time (λωt), destination × time (ψjt), firm × destination (μωj). Absorbs unobservable firm competitiveness, market attractiveness, and pair-specific bilateral barriers. The destination × time FE absorbs the average sanctions effect — identification of the overall ATT requires a two-way variant where an estimated counterfactual destination-time FE (from structural gravity on aggregate flows, purged of sanctions effects) replaces the saturated ψjt.
  - *Dynamic extension:* Lagged dependent variable (max export activity in past 12 months) captures entry costs — the model distinguishes fixed costs of staying in a market from one-time entry costs.
  - *Heterogeneity:* Firm-level interactions for (a) trade finance dependence (share of exports using documentary credit), (b) prior country experience, (c) crisis-country specialization, (d) consumer vs. intermediate goods, and (e) firm size.
  - *Bias correction:* Analytical correction following Hinz et al. (2020) for the three-way incidental parameter bias, particularly the firm-destination FE whose bias is of order 1/T (with T = 48 months, this correction matters materially).

- **Key findings.**
  1. **ATT: Iran −39%, Russia −23%, Myanmar +11% (small), Cuba ~0%.** Sanctions against Iran and Russia significantly lowered the monthly probability of serving those markets by 39 and 23 percentage points, respectively, for French firms that were active in those markets at least once during the sample. The lifting of sanctions on Myanmar produced only a small and gradual positive response (+11%), not symmetric with the large negative response to imposition. Cuba showed no significant response to the US embargo relaxation — French firms were largely insulated from extraterritorial US provisions.
  2. **Strong state dependence — entry costs are real.** The lagged dependent variable is highly significant across all episodes. Implied entry cost factors: 23% higher fixed costs for Iran, 19% for Russia (i.e., firms that were not active in the previous 12 months face significantly higher costs to start serving the sanctioned market). This implies sanctions effects are dynamic: they work partly by raising the "re-entry" threshold, not just by increasing variable costs.
  3. **Trade-finance-dependent firms are disproportionately affected.** Firms with a higher pre-sanctions share of exports covered by trade finance instruments (documentary credits, letters of credit) experienced larger drops in market participation probability in both Iran and Russia. This reflects the financial sanctions channel: SWIFT disconnection (Iran) and restricted access to EU financial markets (Russia) specifically impaired trade finance availability, disproportionately affecting firms that relied on these instruments.
  4. **Prior country experience substantially softens the blow.** Firms already active in Iran or Russia in the pre-sanctions period were significantly less likely to exit than new potential entrants. The ATT change (experienced vs. inexperienced) is positive and significant: established relationships — through prior knowledge, local networks, and sunk investments — provide partial immunity against sanctions-driven exit. This is the sunk-cost / hysteresis channel from Roberts & Tybout (1997), operating here in a sanctions context.
  5. **Crisis-country specialists are partly immune.** A subset of French exporters are specialised in serving politically unstable or sanctioned markets (a "crisis portfolio" strategy). These firms show a significantly smaller sanctions effect — they appear to price in elevated political risk ex ante and maintain business continuity through pre-existing workarounds, diversified risk contacts, and tolerance for uncertain payment terms.
  6. **Suggestive evidence for sanctions avoidance via neighboring countries.** Firms that had prior exports to neighboring countries of the sanctioned market (Turkey, Georgia, the UAE for Iran; Belarus, Kazakhstan for Russia) showed smaller drops in direct exports to the sanctioned country — consistent with trade diversion through non-sanctioning third countries (also documented by Haidar 2017 for Iranian exporters).
  7. **Asymmetry of sanctions imposition vs. removal.** The Myanmar and Cuba cases show that the trade-reducing effects of sanctions (large and immediate) are not mirrored by symmetric trade-inducing effects when sanctions are lifted (small and gradual). This asymmetry is consistent with the sunk-cost interpretation: once a bilateral relationship is destroyed (firm × destination pair dormant), re-establishing it is costly even after the legal barrier is removed.

- **Theoretical implications.**
  The paper provides the cleanest micro-analogue to what the project studies for Chinese firms under tariff shocks: sanctions are the most extreme form of a trade policy shock to the extensive margin, and this paper identifies who exits (trade-finance-dependent, inexperienced, non-specialist firms) and who stays (experienced, large, crisis-country specialist firms). For the project, the findings imply:
  - **d_out as a dynamic decision:** The probability that a Chinese firm exits a RegDependency-exposed market after a tariff shock depends on its prior experience in Western markets, its financial structure (trade-finance dependence), and whether it specialises in high-political-risk destinations. The project's heterogeneous treatment analysis should include these firm characteristics.
  - **Hysteresis in d_out:** Given strong state dependence, firms that exit Western markets after a tariff shock face higher re-entry costs when/if tariffs are reversed — creating a permanent d_out reduction even from a transient shock. This is the capability-trap prediction from Dosi (§4b) operationalised at the trade margin.
  - **Financial constraint as amplifier:** Chinese NBS firms that are financially constrained (private, non-SOE — Guariglia §5b) are more likely to rely on trade finance and therefore face amplified extensive-margin responses to tariff shocks, over and above the productivity channel identified by Amiti-Konings (§5a). The triple interaction (tariff × RegDependency × financial constraint) is theoretically grounded.
  - **Asymmetry predicts treatment persistence:** The lift-off asymmetry finding means that even if the US-China tariff war is de-escalated post-event-study, Chinese firms' d_out contraction is unlikely to reverse symmetrically. The treatment effects are permanent in a non-trivial sense.

---

### Crozet, Fernandes, Mayer, Milet & Taglioni (2025) — "Phyloeconomic Trade Diversity: A Study of the Impact of Diversification on Firms' Export Volatility for 64 Developing Countries"
*Working paper, April 2, 2025. Authors: Université Paris-Saclay, World Bank, Sciences Po, HEG-Genève, World Bank.*

- **Main contribution.** The paper introduces a new measure of firm-level export diversification — the **phyloeconomic diversity index Φ** — inspired by biodiversity metrics (Leinster & Cobbold 2012), and uses it to answer the question of whether export diversification reduces export volatility. The innovation over existing HHI-based measures is that Φ explicitly captures the **disparity** dimension of export portfolios: not just how many markets and how evenly sales are spread, but how **dissimilar** those markets are (measured by geographic distance or business-cycle correlation). The paper finds that more destinations and more even distribution reduce volatility (confirming the standard hedging logic), but conditional on these, **more dissimilar destinations *increase* volatility** — a counter-intuitive result explained by the fact that distant/dissimilar markets carry higher idiosyncratic demand variance.

- **Data and method.**
  - *Data:* World Bank Exporter Dynamics Database — firm-level customs declarations for 64 emerging and developing countries, aggregated at HS2 × firm level. ~915k firm-product pairs; 1996–2019; unbalanced panel (coverage varies by country).
  - *Diversity index Φ:* Leinster-Cobbold (2012) generalization (q = 2): Φ = [Σ_c Σ_{c'} p_c z_{cc'} p_{c'}]^{-1}, where p_c is market c's share of firm exports and z_{cc'} ∈ [0,1] is bilateral similarity between countries c and c'. Two versions of z: (a) geographic — z^dist_{cc'} = exp(−dist_{cc'}/mean_dist); (b) business cycle — z^bc_{cc'} = (1 + corr(g_c, g_{c'}))/2. Under the geographic version, Φ = (HHI + Σ_{c≠c'} p_c z_{cc'} p_{c'})^{-1} — decomposing cleanly into an evenness component (HHI) and a disparity component (the cross-term sum). About 50% of the variance in Φ is orthogonal to HHI and number of destinations — the disparity component has independent empirical content.
  - *Volatility measure:* Detrended coefficient of variation: firm-specific linear trend removed, then RMSE normalized by average exports over 3-year periods (baseline T=3; robustness at T=5 and T=7).
  - *Specification:* ln(Vol_{i,T}) = α + β ln(Φ_{i,T0}) + δ ln(HHI_{i,T0}) + γ ln(#Dest_{i,T0}) + FE + ε. Between estimates (FE = country×product×period); within estimates adding firm FE for clean within-firm identification.
  - *Simulations:* Melitz-type model (Crozet et al. 2012; Bas et al. 2017) with multiple heterogeneous-firm demand shocks. Calibrated to match empirical findings — requires assuming that firm-destination demand shock variance increases with geographic distance from home country.

- **Key findings.**
  1. **Φ alone → negative and significant (more diverse = less volatile): β̂ ≈ −0.62 (between) / −0.23 (within).** When all three dimensions of diversification load onto Φ, diversified firms are less volatile — as standard hedging theory predicts.
  2. **Conditional on HHI and #destinations, Φ flips positive: β̂ ≈ +0.51 (between) / +0.18 (within), significant at 1%.** This is the central finding. Controlling for the number of markets and the evenness of sales, exporting to a more *dissimilar* set of countries RAISES volatility by roughly half a percent per 1% increase in Φ. The result is robust across geographic and business-cycle similarity measures, to alternative periods (5-year, 7-year), within-firm changes, and is positive and significant for 36 of 59 countries in country-specific regressions (median coefficient 0.66).
  3. **Mechanism (simulations): distant markets are intrinsically riskier.** Demand shock variance increases with distance — firms exporting to far-away, dissimilar markets face higher idiosyncratic demand volatility in those markets. When a firm diversifies by adding dissimilar markets, it reduces the covariance across destinations (good for hedging) but simultaneously increases the average variance in each new market (bad for stability). The net effect is negative — the variance-raising effect of harder markets dominates the covariance-reducing effect of dissimilarity.
  4. **A global geographic constraint creates the positive relationship.** Two countries that are both close to the exporting country also tend to be close to each other. So to reach markets that are dissimilar to each other (low z_{cc'}), a firm must also reach markets that are far from home. Firm exports to far markets face higher variance. Thus, higher Φ is mechanically associated with higher average variance of firm-destination demand shocks.
  5. **Distributional findings.** 70% of firm-HS2 pairs in the sample export to only one destination (Φ = 1). For multi-destination exporters: chemical products exporters are the least diversified by Φ; agricultural and manufacturing exporters are most diversified. Country-level average Φ correlates 0.59 with distance to world markets (remoter countries have more diversified firm portfolios — consistent with the logic that distant countries must serve dissimilar markets to have any foreign demand).

- **Theoretical implications.**
  The paper directly extends the Vannoorenberghe (§5c) and Barbieri (§5c) findings from the project's existing review, providing both a formal measure and a causal mechanism. For the project:
  - **d_out structure and volatility:** The paper distinguishes two routes to geographic diversification: (a) adding more destinations with similar profiles (classic hedging, reduces volatility) and (b) adding dissimilar/distant destinations (disparity-driven, increases volatility). Post-tariff-shock, Chinese firms forced to substitute EU markets for more distant or dissimilar alternatives (e.g., African or LatAm markets) face HIGHER export volatility, not lower — even if they successfully maintain total export value (d_out maintained but noisier). This creates an important welfare asymmetry: firms that preserve d_out by diversifying into dissimilar markets face heightened macro-shock exposure.
  - **d_in as the low-volatility strategy:** If adding dissimilar destinations raises volatility, the risk-minimizing response to losing a familiar, high-Φ export cluster (e.g., EU markets for a Chinese firm with BRIM community membership in EU-aligned product space) is to consolidate d_in (retreat to domestic market, where demand variance is lower and correlation with existing revenue streams is high). This provides a firm-theory mechanism complementary to the capability-conservation argument from Penrose/Dosi: d_in consolidation is not just about preserving knowledge; it is also the variance-minimizing portfolio strategy after a high-Φ exit.
  - **The phyloeconomic index as a measure of market portfolio riskiness.** Φ can be adapted as a measure of the "riskiness" of a firm's geographic exposure portfolio. For Chinese firms in the project's sample, a high pre-treatment Φ (exporting to many dissimilar Western and non-Western markets) combined with a tariff shock on the Western component should predict larger d_out volatility (not just lower levels) in post-treatment periods — a testable prediction distinguishing portfolio rebalancing from capability destruction.
  - **Import-side extension (marginal note in paper).** The authors note (and the user's annotation on the PDF asks about this) that Φ could be adapted to characterise import portfolio diversity. For the project: Chinese firms' import diversification Φ (sourcing from diverse intermediate suppliers) would capture supply-chain resilience; tariff shocks that reduce import Φ (by cutting off complex intermediate suppliers from specific regimes) should amplify d_in contraction beyond what is predicted by output tariffs alone.

---

### Cross-paper synthesis (§5m)

**1. Crozet_2021 (sanctions/extensive margin) + Crozet_2025 (diversity/volatility) = a two-part micro-theory of how firms restructure d_out under external trade shocks.** The first paper shows WHICH firms exit a market under a severe trade policy shock (financially constrained, inexperienced, non-specialist) and that exit is largely permanent (hysteresis). The second paper shows WHAT HAPPENS to the surviving firms' portfolio volatility when they compensate by diversifying into more dissimilar destinations. Together they predict: (a) financially constrained, inexperienced Chinese firms exit Western markets post-tariff (Crozet_2021); (b) firms that survive and re-diversify toward non-Western markets face higher export volatility if those new markets are more dissimilar (Crozet_2025); (c) the safest firm response is therefore d_in consolidation (retreat to domestic + core familiar markets) rather than d_out substitution.

**2. The sanctions asymmetry (Crozet_2021) + the OSA regime-shift logic (JRC §5l) = treatment effect persistence.** Crozet_2021 shows that sanctions removal does not produce symmetric trade recovery. JRC §5l shows that the EU's OSA agenda is designed as a permanent regime change, not a temporary measure. Combining: even if US-China tariffs are eventually reduced, Chinese firms' d_out contraction in EU-strategic sectors is unlikely to reverse — both because of re-entry costs (Crozet_2021 mechanism) and because the EU is building domestic capacity through IPCEIs and reshoring (reducing demand for Chinese exports structurally, independent of the tariff). The project's event-study coefficients therefore measure a durable, not transient, treatment.

**3. Phyloeconomic Φ + BRIM community structure = a joint measure of capability-portfolio riskiness.** Crozet_2025's Φ captures the dissimilarity of a firm's destination portfolio. The project's BRIM block membership captures the complexity and coherence of a firm's capability portfolio (d_in). High Φ + high d_in complexity = a firm that is both capability-rich and geographically exposed to dissimilar markets — the highest-risk configuration when tariff shocks hit. For the project: the triple interaction (tariff shock × high Φ destination portfolio × high BRIM block fitness) should identify which firms face maximum d_out volatility increases and maximum d_in consolidation pressures simultaneously.

**4. Trade-finance dependence (Crozet_2021) + Chinese private-firm financial constraints (Guariglia §5b) = an amplification channel.** Guariglia finds that private Chinese NBS firms have the highest financial constraints (α_1 ≈ 1, near-full self-financing). Crozet_2021 finds that trade-finance-dependent firms exit sanctioned markets more sharply. Combining: private Chinese firms (high financial constraint) that relied on trade finance to serve Western markets face a double amplification — the tariff shock raises the costs of serving those markets, AND reduces their ability to finance continued participation through trade credit. This interaction predicts heterogeneous treatment effects by ownership type (SOE vs. private) in the project's baseline specification, over and above the baseline productivity differential.

