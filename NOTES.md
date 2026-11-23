# DSI 2026 — v2 Presentation Deck: Presenter Notes

A NEW presentation deck built from MK's **25-slide academic PDF**
(`ADAM_DSI_2026_Academic_25_Slides_Improved.pdf`), as a SEPARATE GitHub
Page called **dsi2026v2**. This is a **different deck** from
`~/workspace/projects/dsi2026/` (v1, 33 cards, built from the older 20-slide
deck + 30-slide microlearning PDF) — v1 was read only as the pattern
reference for the presenter engine and was **not modified**. The other three
projects (financial-disclosure-intelligence, financial-disclosure-basics,
financial-disclosure-presentation) were likewise untouched.

- Working copy: `~/workspace/projects/dsi2026/index.html` → here:
  `~/workspace/projects/dsi2026v2/index.html`
- Live: new repo `mindsyourai/dsi2026v2`,
  https://mindsyourai.github.io/dsi2026v2/
- Source of truth: `~/workspace/user/files/ADAM_DSI_2026_Academic_25_Slides_Improved.pdf`
  (25 pages, verified via pdfinfo) and the full text extract
  `~/workspace/projects/dsi2026v2/SLIDES25_EXTRACT.txt`
- Engine: v1's proven presenter engine, reused unchanged in behaviour —
  one card at a time, keyboard (→ / ← / Space / Home / End), tap/click
  zones, on-screen Prev/Next, progress bar + "Card N of 27" counter,
  section labels, fullscreen button, presenter-notes toggle (hidden by
  default), swipe on touch, print stylesheet showing all cards. Works
  offline except the Google Fonts link (system fallbacks included).
- Presenter notes: **one short note per card** (27 notes in the deck's
  NOTES dict, no section-opener fallback needed) — results cards carry
  row-by-row elaboration cues.

## Card list (27 cards) — one card per PDF slide, in PDF order

| # | Section | Title | PDF slide |
|---|---------|-------|-----------|
| 1 | Title | From Model Disagreement to Disclosure Intelligence + authors (Kazim Topuz presenter, Jessica Bedson, Tally Ferguson, Thomas Kim, TU, DSI 2026) + core idea + LinkedIn | 1 |
| 2 | Roadmap | The research story in four steps | 2 |
| 3 | Background | What is a 10-K — and where does ADAM look? (Form 10-K, Item 1A, Item 7) | 3 |
| 4 | Audience check | Item 1A or Item 7? — interactive vote (Passage A → 1A, Passage B → 7) | 4 |
| 5 | Motivation | Why narrative disclosures are hard to analyze (volume / repetition / interpretive difficulty) | 5 |
| 6 | Background | From word counts to contextual models (2011 LM → 2019 FinBERT → Today LLM → ADAM) | 6 |
| 7 | Method 1 · LM | Loughran–McDonald: a finance-specific dictionary + net-tone formula + Henry warning (−0.091 is NOT LM's) | 7 |
| 8 | Method 1 · LM | **Interactive: Count like LM** — 50-word passage, tap-to-cycle, live counters + live net tone, Check my selection, Reset | 8 |
| 9 | Method 1 · LM | LM reveal: Positive 5, Negative 6, net −0.02; what LM still cannot see | 9 |
| 10 | Method 2 · FinBERT | FinBERT: contextual sentiment (illustrative 0.62 / 0.30 / 0.08) | 10 |
| 11 | Method 2 · FinBERT | **Interactive: Read FinBERT's output** — tap class + confidence, then reveal | 11 |
| 12 | Method 2 · FinBERT | FinBERT reveal: Negative, 0.62, routes to review below 0.80; still missing: new? repeated? peer-common? firm-specific? | 12 |
| 13 | Conceptual pivot | Why disagreement can be useful evidence (LM NEGATIVE vs FinBERT NEUTRAL) | 13 |
| 14 | Research design | Four questions, four design requirements (RQ1–4, DR1–4) | 14 |
| 15 | ADAM | ADAM: a six-layer decision-support architecture | 15 |
| 16 | ADAM | Three agents — deliberately non-equivalent roles | 16 |
| 17 | ADAM | What the Context & Quality Agent adds | 17 |
| 18 | ADAM | Adjudication separates tone, economics, informativeness, and uncertainty + six discrepancy diagnoses | 18 |
| 19 | Empirical setting | Data and sample flow: 179,623 → 143,372 → 300; 55 firms, 11 sectors, 550 10-Ks 2016–2025; 32,407 historical | 19 |
| 20 | Results | Human reference set table (21/66/13, 25/64/11, 32/54/14; Fleiss κ .08/.12/.16) | 20 |
| 21 | Results | Evaluation: separate model performance from architectural contribution (benchmarks vs nested tests) | 21 |
| 22 | Results | Sentiment table: LM 37.3%/0.320, FinBERT 60.7%/0.529, Ensemble 58.7%/0.384, ADAM 82.7%/0.745; direction 83.3%/.689, informativeness 71.4%/.607 | 22 (part 1) |
| 23 | Results | Direction + informativeness table (ADAM): direction 83.3%/.689/P 0.757/R 0.647; informativeness 71.4%/.607/P 0.631/R 0.649 | 22 (part 2) |
| 24 | Results | Disagreement table: 162/300 = 54%; LM 25.3%, Ensemble 64.8%, FinBERT 68.5%, ADAM 76.5%; both-wrong 77 → 89.6% | 23 (part 1) |
| 25 | Results | Ablation table (informativeness Macro-F1): Judge only 0.453, Base 0.469, Full ADAM 0.607; ΔF1 +.138/+.154 | 23 (part 2) |
| 26 | Results | Decision-support table: flag 81.0%/69.9% vs FinBERT-negative proxy 19.5%; 56% routed, 92.3% errors captured, 97.0% automated accuracy | 24 |
| 27 | Finish | Takeaways: 3 contributions + boundaries + next + Questions/LinkedIn | 25 |

Section breakdown: Title 1 · Roadmap 1 · Background 2 · Audience check 1 ·
Motivation 1 · Method 1 · LM 3 · Method 2 · FinBERT 3 · Conceptual pivot 1 ·
Research design 1 · ADAM 4 · Empirical setting 1 · Results 7 · Finish 1 =
**27 cards**.

## ⚠️ Card count — 27, not 28 (flagged, not silently resolved)

The brief's card plan says "25 slides + 3 extra split cards = 28 cards",
but the splits as specified add only **2** extra cards: slide 22 → 2 cards
(+1) and slide 23 → 2 cards (+1). Slides 20 and 24 each become one card, as
specified. 25 + 2 = **27**. No card was invented to reach 28; the deck
follows the specified mapping exactly. If MK wants a 28th card, the natural
candidate is splitting slide 20 (human-agreement table) from the evaluation
design — but slide 21 already is the evaluation card, so that would
duplicate content. MK to confirm 27 is correct.

## ⚠️ The 179,623 / 143,372 flow — read this before presenting (for MK to confirm)

This PDF presents the data flow as:

> **179,623 extracted focal paragraphs → 143,372 ADAM-eligible narrative
> paragraphs → 300 human-reference paragraphs**

Card 19 shows exactly that, with the on-card line: "179,623 is the
extracted count before eligibility filtering; 143,372 is the ADAM-eligible
set." The card-19 presenter note carries the same reading.

**Conflict with the old rule:** the earlier decks carried a rule
"179,623 must never appear", because the OLD 20-slide deck presented
179,623 as the focal total, contradicting its own 143,372 headline (its
table said Item 1A 94,031 + Item 7 85,592 = 179,623). On 2026-11-21 MK
decided the site and the v1 deck use 143,372 focal with no per-item split,
and 179,623 / 94,031 / 85,592 were removed from all learner-facing content.

This PDF presents 179,623 **differently** — as the extracted count *before*
eligibility filtering, not as the focal total — so it is not the same
contradiction. Per MK's "use pdf as the main", v2 follows the PDF. But the
old rule is not silently discarded: **MK should confirm this reading**
before presenting. If he disagrees, card 19 is the only place 179,623
appears (plus its presenter note) and it is a one-line fix.

What v2 does NOT do: present 179,623 as the focal total; use the old
94,031 / 85,592 per-item split anywhere (0 occurrences — this PDF gives no
per-item split of the focal set, only the 144/156 split of the 300); write
173k anywhere (0 occurrences). The sum 143,372 + 32,407 = **175,779** is
shown on card 19 labelled as the arithmetic sum, not as a deck figure.

## ⚠️ Disagreement-subset Macro-F1 — removed after PDF verification (for MK to confirm)

The v1 deck's disagreement table showed FinBERT Macro-F1 **0.606** and ADAM
**0.703** on the disagreement subset (from the old deck's slide 16, verified
against the PPTX). **This PDF's slide 23 reports accuracy only** on that
subset (76.5 / 68.5 / 64.8 / 25.3) — 0.606 and 0.703 occur **0 times** in
the whole PDF text (checked by grep over a fresh pdftotext dump), and slide
23 contains no chart image that could hold them (the PDF's only images are
on pages 1 and 25). Card 24 therefore shows "—" for Macro-F1 on all four
rows, with the footnote "Macro-F1 is not reported for any method on the
disagreement subset (slide 23 reports accuracy only)". If MK wants the
0.606 / 0.703 restored from the earlier deck, that is a one-line change to
card 24 — but they would then be old-deck figures, not PDF figures.

## Numbers the presenter should treat carefully

- **All ADAM results are PRELIMINARY — VALIDATION ONGOING.** Cards 20,
  22–26 carry the pill; cards 20, 22–26 carry the "Research still ongoing —
  confirmatory validation, confidence intervals, and paired significance
  tests to come in the final paper" line. Card 21 (evaluation design) has
  no numbers and no pill. Do not present any ADAM number without that label.
- **Ablation (card 25) is informativeness only.** The PDF reports the
  nested-configuration comparison for disclosure informativeness only
  (F1 0.453 → 0.469 → 0.607). It gives **no** sentiment or direction figures
  for Judge-only / Base / Full ADAM — the v1 deck's "Judge-only already
  82.0% sentiment / 84.0% direction" honest-boundary line is NOT in this
  PDF and is not in v2. Do not quote it from this deck.
- **"Both declines are statistically significant"** is the PDF slide 23's
  exact wording for the ΔF1 +.138 / +.154 result (i.e. removing context
  drops informativeness F1). The card renders it as "both statistically
  significant".
- **LM net tone (cards 7–9):** LM's own formula is (Pos−Neg) ÷ total
  words = −0.02 in the worked example; Henry's (Pos−Neg)/(Pos+Neg) = −0.091
  is a different measure — card 7 carries the warning.
- **FinBERT example probabilities (cards 10–12) are illustrative teaching
  values**, not a real model run — labelled on card 10 ("illustrative
  probabilities shown here") and in the PDF ("illustrative probabilities
  shown here").
- **Human agreement (card 20):** unanimous agreement 21% sentiment / 25%
  direction / 32% informativeness is a finding about task difficulty, not
  a failure of the reviewers. Fleiss κ .08 / .12 / .16.
- **No 60/75/90-day filing deadlines anywhere** — the PDF has none and v2
  adds none (grep-verified, 0 occurrences).

## The interactives (cards 4, 8, 11)

- **Card 8 — LM word-selection (centerpiece).** The 50-word passage is
  rendered as 50 tappable word buttons. Tap cycles neutral → Positive
  (green) → Negative (red) → neutral. Live counters (Positive = N,
  Negative = N) and a live net-tone calculation ((Pos−Neg)/50) plus the
  per-1,000 figure update with every tap. "Check my selection" freezes the
  board and marks each word: correct picks get ✓, wrongly marked words get
  ✗ (red), LM words the user missed get a dashed outline in their correct
  colour — and the reveal panel shows the correct 5 positive (strong,
  improve, efficient, benefit, success) / 6 negative (decline, loss, risk,
  volatility, weak, burden) with net −0.02, −20 per 1,000. Reset clears
  everything. **No answer leak on cold load:** the idle hint reads "Total
  words: 50. Tap once for Positive, twice for Negative, three times to
  clear — then check your selection." (v1's leak — an idle hint stating the
  answer — was fixed in v1 and is not reintroduced here; the answer key
  lives only in the script, not in the DOM.) "Exactly right" appears only
  when the user's own selection matches the key exactly.
- **Card 4 — Item 1A / Item 7 vote.** Tap A or B per passage (selects
  without revealing correctness), then "Reveal the answers" marks
  correct/wrong and shows the one-line reason each: A → Item 1A (a threat
  that *could* raise costs or limit sales); B → Item 7 (this year's
  performance — revenue, volumes, costs, liquidity). Reset clears.
- **Card 11 — FinBERT challenge.** Tap the predicted class (Negative /
  Neutral / Positive) and the confidence value (0.62 / 0.30 / 0.08), then
  reveal: Negative, 0.62, routes to review below 0.80 — plus the "what
  FinBERT still can NOT answer" line (new? repeated? peer-common?
  firm-specific?). Reset clears.

## Presenter timing guidance (~20–22 minutes)

| Section | Cards | Minutes | Notes |
|---------|-------|---------|-------|
| Title + roadmap | 1–2 | ~2 | Open with the problem, not the technology. |
| Background + vote + motivation | 3–6 | ~3 | Card 4 is the first vote — quick. |
| LM Dictionary | 7–9 | ~3 | **Spend the most time here.** Card 8 is the slow-down moment — let the room count along. |
| FinBERT | 10–12 | ~3 | Card 11 is the second vote; card 12 is the pivot to ADAM. |
| Conceptual pivot + research design | 13–14 | ~2 | The thesis, then the design-science spine. |
| ADAM | 15–18 | ~2 | Layers → agents → context → adjudication. |
| Empirical setting | 19 | ~1 | The flow; be ready for the 179,623 question (see note above). |
| Results | 20–26 | ~4 | Card 20 first (humans disagree too), then one table per card. Keep the PRELIMINARY label on every number. |
| Finish + questions | 27 | ~1 | Close with the design insight, not the accuracy number. |
| **Total (talk)** | **1–27** | **~20–22** | |

If running short, compress cards 2, 6, 14 to one sentence each; do not cut
the LM worked example (card 8), the votes (cards 4, 11), or the headline
results (card 22). If running long, cut the LM check to the answer only
(skip the live counting).

## Sources

- `~/workspace/user/files/ADAM_DSI_2026_Academic_25_Slides_Improved.pdf`
  (25 slides; extracted to
  `~/workspace/projects/dsi2026v2/SLIDES25_EXTRACT.txt`)
- Presenter engine + results-table patterns adapted from
  `~/workspace/projects/dsi2026/index.html` (v1, 33 cards — read only,
  not modified). v1's LM game was **not** copied as-is: v1 auto-marks a
  tapped word by its hidden key, so its "reveal" was trivial; v2 uses
  tap-to-cycle with a separate Check step, per the v2 brief. v1's
  adjudicator A/B/C vote was not carried over (no such slide in the 25-slide
  PDF); the vote and FinBERT games are new, built for PDF slides 4 and 11.
- Numbers cross-checked against the v1 deck's verified results tables
  (NOTES.md "Results rebuild" section) — every cell that also appears in
  this PDF matches; the two cells that do not appear in this PDF
  (disagreement-subset Macro-F1 0.606 / 0.703) were removed, see above.

## Self-check summary (build, 2026-11-23)

- Card count is 27 (grep `class="card"` — 27 sections; counter reads
  "Card 1 of 27"). Section breakdown matches the PDF order (see table
  above). The brief's expected 28 is addressed in the count note above.
- No "173" and no "94,031" / "85,592" anywhere in `index.html`
  (grep-verified, including the rendered text in a headless-Chromium run).
  "179,623" appears 4× — twice on card 19 (flow + explanatory line) and
  twice in the card-19 presenter note — all as the PDF's "extracted"
  reading, never as the focal total.
- "175,779" appears on card 19 (labelled as the arithmetic sum) and in the
  card-19 presenter note.
- Cards 20, 22, 23, 24, 25, 26 carry the PRELIMINARY pill; cards 20,
  22–26 carry the "Research still ongoing" line.
- LM passage token-counted by hand from the PDF: 50 tokens; positive =
  strong, improve, efficient, benefit, success (5); negative = decline,
  loss, risk, volatility, weak, burden (6); (5−6)/50 = −0.02; −20 per 1,000.
- Numbers recomputed (all pass): 55 × 10 = 550; 144 + 156 = 300;
  143,372 + 32,407 = 175,779; 162/300 = 54%; 69/77 = 89.6%;
  0.607 − 0.469 = +0.138; 0.607 − 0.453 = +0.154;
  (5−6)/50 = −0.02; (5−6)/50 × 1,000 = −20;
  Henry (5−6)/(5+6) = −1/11 ≈ −0.091; 0.62 + 0.30 + 0.08 = 1.00;
  agreement rows sum to 100% (21+66+13; 25+64+11; 32+54+14);
  56% of 300 = 168 routed to review.
- `node --check` on the extracted inline JS: OK.
- Headless-Chromium pass (see review log below): 63 assertions, 0 failures.

## Review-pass log

- [x] Review pass 1 (facts / numbers / sources, card-by-card vs the PDF
  extract): 2026-11-23, builder (see limitation note below).
  - Order verified card by card against SLIDES25_EXTRACT.txt: 27 cards,
    PDF slides 1–25 in order, splits exactly as specified (22 → 2, 23 → 2).
  - Verbatim checks passed: passages A/B, core idea, LinkedIn, pivot
    sentence, LM categories, FinBERT sentence, RQ2 wording, agentic line,
    data-flow line, takeaway boundaries.
  - Every results-table cell re-verified against PDF slides 20–24
    (fresh pdftotext dump, not just the stored extract): agreement rows,
    sentiment table, direction + informativeness, disagreement accuracies,
    ablation F1s, decision-support figures — all match.
  - FINDING FIXED (1): disagreement-subset Macro-F1 0.606 / 0.703 were
    carried over from the v1 deck but occur 0 times in this PDF (slide 23
    reports accuracy only; no chart image on the slide could hold them —
    the PDF's only images are pages 1 and 25). Removed from card 24
    (now "—" on all rows) and from the card-24 presenter note; footnote
    updated. See the dedicated note above — MK to confirm whether to
    restore them from the earlier deck.
  - LM passage hand-counted token by token from the PDF (50 tokens; 5
    positive / 6 negative as listed above); the key in JS matches exactly.
  - No other findings. The "Fleiss κ" string check initially flagged a
    miss that turned out to be a `<strong>` tag interrupting the literal
    text — the κ values are present on card 20.
- [x] Review pass 2 (live browser: keyboard, interactives, mobile,
  print): 2026-11-23, REAL headless Chromium (Playwright, cached
  Chromium build). Script: `/tmp/pwtest-v2/test.mjs` — 63 assertions,
  0 failures on the final run (after the card-24 fix; re-run clean).
  - Keyboard 1→27→1: ArrowRight ×26 → "Card 27 of 27", Next disabled,
    ArrowRight clamps; End/Home; ArrowLeft clamps at 1; section-label
    sequence matches the plan on all 27 cards.
  - Overflow: scrollWidth vs viewport measured on EVERY card at 1280×800
    and at 390×844 — no horizontal overflow on any card at either width.
  - LM game (card 8, desktop): 50 word buttons; cold load shows 0/0 and
    a hint with no answer leak; tap cycles neutral → pos → neg → neutral
    (Strong: Pos 1 / net +0.02, then Neg 1 / −0.02, then cleared); all 11
    correct taps → Positive 5 · Negative 6, net −0.02, −20 per 1,000,
    "Exactly right" hint; Reset → 0/0; wrong tap ("expects") + Check →
    1 of 11 right, 1 wrongly marked, 10 missed, reveal shown with the
    correct lists and −0.02; Reset clears all marks. Mobile tap also
    verified (Strong → Positive 1 at 390px).
  - Vote game (card 4): wrong pick for A + right pick for B → A red,
    B green, reveal shown naming A → Item 1A / B → Item 7 with reasons;
    Reset clears.
  - FinBERT game (card 11): wrong class (Neutral) + right confidence
    (0.62) → Neutral red, Negative green, 0.62 green, reveal shown
    (Negative, 0.62, routes to review below 0.80, four unanswered
    questions); Reset clears.
  - Notes toggle: hidden by default; toggle shows/hides; card-19 note
    carries the 175,779 reconciliation.
  - Fullscreen: enters and exits on button clicks (headless Chromium).
  - Tap zones: visible (display flex) at 1280px; zone clicks advance/retreat.
  - Swipe: CDP touch swipe left advances (390px viewport).
  - Print: emulated print media shows all 27 cards.
  - JS errors: 0 console errors, 0 pageerrors across all loads. (The only
    failed requests are the Google Fonts fetches blocked by the sandbox
    egress proxy — ERR_TUNNEL_CONNECTION_FAILED on the font hosts only,
    the same known sandbox behaviour as the v1 review; the deck's
    system-font fallbacks rendered and no layout/overflow check was
    affected. Fonts load normally live.)
  - Test-harness artefacts found and corrected during the pass (not deck
    bugs): the "10 missed" count (11 − 1 right = 10, the first expectation
    of 9 was miscounted); a double `.reverse()` in the section-sequence
    comparison; a swipe test that bypassed the deck's internal card index
    by toggling classes directly.
- [ ] Independent-reviewer limitation: the brief asked for the two review
  passes to be done "with a second subagent as independent reviewer". This
  build ran as a depth-2 subagent, which cannot spawn subagents
  (`can_spawn=no`), so both passes above were done by the builder, with
  the content pass done as a separate re-read against fresh pdftotext
  output (which is what caught the 0.606/0.703 issue). A genuinely
  independent re-check by another agent before presenting is still open
  and recommended — the parent agent can arrange it.

## Push + live check (2026-11-23)

- Repo did not exist (check → 404). Created via API POST /user/repos
  (mindsyourai is a User account, not an org): `mindsyourai/dsi2026v2`,
  public, default branch main, no auto-init (repo id 1469143949).
- Helper's `init` NOT used — it writes a hardcoded turkic-fest README.
  First commit via Contents API PUT of index.html itself (the Git Data API
  push refuses an empty repo with 409, as the connector doc warns):
  commit `0d8b01a1af5856208efa6b60dd04d39c365c1de2`, index.html at root.
  NOTES.md committed separately: `cb9dd1e1a447d1f53540286659780807729f7ba3`.
- Pages enabled: POST /pages → 201, source main / root,
  https://mindsyourai.github.io/dsi2026v2/.
- Live check (curl, cache-busted, ~45 s after Pages enable): HTTP 200,
  65,478 bytes, **byte-identical to local** (cmp clean), "Card 1 of 27"
  present, 179,623 present, tables present. Independent browser.open fetch
  confirms the live text: all 27 cards in order, including the corrected
  disagreement table (Macro-F1 "—" on all rows) and the decision-support
  table. No stale-copy lag on the first check.
- NOTES.md push-section update committed after the live check (this file's
  own update is pushed separately, so the repo copy stays current).
