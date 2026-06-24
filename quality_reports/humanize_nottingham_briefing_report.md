# `/humanize` report — `paper/nottingham_briefing.tex`

**Date:** 2026-06-24
**Prose audited:** ~1,800 words (body prose + keyboxes + captions; tables, math, and the reference list excluded).
**Mode:** detect-and-flag. No edits made — the author applies changes.

---

## Headline

**HIGH findings: 0 per 1,000 words → light cleanup, mostly cosmetic.**

The high-signal tells that referees actually pattern-match on are **absent**: no boilerplate
transitions (`Moreover`, `Furthermore`, `It is important to note`), no hedging stacks
(`might potentially`, `could possibly suggest`), no cliché lexicon (`delve`, `shed light`,
`navigate the landscape`, `tapestry`, `play a crucial role`), and no sycophantic /
promotional framing (`groundbreaking`, `novel approach`). The first-person, problem-first
voice reads as authored.

What remains is a **stylistic fingerprint**, not a content problem: a pervasive em-dash
habit and a high density of hyphenated compounds. Both are MED, both are cheap to thin out.

---

## Per-category counts

| # | Category | HIGH | MED | LOW |
|---|----------|:----:|:---:|:---:|
| 1 | Boilerplate transitions | 0 | 0 | 1 |
| 2 | AI-cliché lexicon | 0 | 1 | 2 |
| 3 | Em-dash / punctuation overuse | 0 | 1 | 0 |
| 4 | Symmetric paragraph shapes | 0 | 0 | 1 |
| 5 | Tricolon abuse | 0 | 0 | 1 |
| 6 | Hedging stacking | 0 | 0 | 0 |
| 7 | "Not only X, but also Y" | 0 | 0 | 0 |
| 8 | Formulaic openers | 0 | 0 | 1 |
| 9 | Hyphenation excess | 0 | 1 | 0 |
| 10 | Sycophancy / self-importance | 0 | 0 | 1 |

---

## Most concentrated paragraphs (top 3)

1. **§3 "The hard part — turning a static map into a panel" (lines 323–345).** ~5 em-dashes
   across the two bullets, plus a dense hyphen run (`temporal-coupled`, `right-hand-side`,
   `look-ahead`, `460k-firm`, `pre-shock`). The single most stylistically "AI-shaped" block.
2. **§1 Retrenchment/Reinvention bullets (lines 95–105).** Hyphen-chain density:
   `Sunk-cost`, `re-entry-cost`, `variance-minimisation`, `within-cluster`,
   `competition-to-coherence`, `product-vector`, `frontier-firm`, `moderate-shock`.
3. **§2 γ-resolution paragraph (lines 188–202).** Contrastive `Some is meaningful: … Some is
   mechanical: … The point is that …` cadence + two em-dashes; mild but the closest thing to
   a symmetric shape.

---

## Per-finding table

| line | category | severity | current text | suggested action |
|---|---|---|---|---|
| 158 | 1 boilerplate | LOW | "Crucially the data-driven partition is \emph{not} a relabelling…" | drop "Crucially," — the sentence is emphatic on its own |
| 113 | 2 cliché | LOW | "carry geopolitical \textbf{leverage}" | term-of-art (Farrell–Newman) — acceptable; if you want zero detector hits, "geopolitical chokepoints" |
| 279 | 2 cliché | MED | "The \textbf{robust} message:" | "robust" is on the cliché-adjacent list → "The message that survives:" / "The durable message:" |
| 239 | 2 cliché / 10 | LOW | "the single most \textbf{important} input to the panel design" | soften → "the fact that most shapes the panel design" |
| 323–345 | 3 em-dash | MED | "(a) … attractive --- capabilities really do evolve --- but … Worse, … depends on $t{+}1$ --- a look-ahead …" | convert 2–3 of the `---` to commas or parentheses; target ≤2 per paragraph |
| 301–302 | 3 em-dash | LOW | "The causal question --- does … push the firm toward $\din$ or $\dout$? --- needs" | fine as a pair, but you already use this parenthetical-dash move ~10×; vary a few |
| 188–202 | 4 symmetric | LOW | "Some is \emph{meaningful}: … Some is \emph{mechanical}: … The point is that …" | fine once; just don't repeat the "Some is X: Some is Y:" cadence elsewhere |
| 84 | 5 tricolon | LOW | "kept, dropped, or newly entered" | keep — natural |
| 95–105 | 9 hyphenation | MED | bullet text (8 hyphen-compounds) | most are technical (keep); relax discretionary ones only if a sentence stalls |
| 155–157 | 9 hyphenation | LOW | "machinery-and-electrical \emph{generalist} block" | "machinery and electrical generalist block" (drop the chained hyphens) |
| 403 | 5 tricolon | LOW | "the complexity of the products \emph{dropped}" (within a 2-dash clause) | fine |
| 239, 282, 323, 351 | 8 formulaic | LOW | repeated demonstrative openers: "This distributional fact…", "This is what tells me…", "This is the crux…", "This single choice is the thing…" | vary 1–2; e.g. "That distributional fact…" / "Which is why…" |
| 271 | 10 self-framing | LOW | "\paragraph{A new fact:" | mild novelty claim; "A second pattern:" reads less promotional |
| 348 | 10 self-framing | LOW | "the option I find most \textbf{elegant}" | keep if sincere; "the option I'm most drawn to but least sure of" avoids the aesthetic self-praise |

---

## Recommendation

**Cosmetic pass, not a rewrite.** Two mechanical edits capture ~80% of the value:

1. **Thin the em-dashes.** You lean on the `--- clause ---` parenthetical and the
   `--- clause-joiner` in nearly every paragraph. Pick the 6–8 least load-bearing and swap to
   commas/parentheses. Start with §3 "The hard part."
2. **Relax the 3–4 *discretionary* hyphen-compounds** (`machinery-and-electrical`,
   `big-revenue`, `cheapest-to-cut`); leave the technical terms (`out-of-block`,
   `shift-share`, `distributed-lag`, `parallel-trends`) — those are correct.

Everything else is a one-token swap (`Crucially`, `robust message`) or optional. The
document is in good shape on the tells that matter for referee credibility.
