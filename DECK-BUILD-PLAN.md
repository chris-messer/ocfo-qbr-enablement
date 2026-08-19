# Walkthrough deck — build plan (shipped)

**Skill:** customer-walkthrough-deck  
**Sources:** `slide-guide-ocfo-qbr.md` · [Selling to CFOs Field Guide v2.0](https://docs.google.com/document/d/11J4Bdh5_cBlE-NoZ9b_W4acO__hGWqgo2vBIrzSpWGo) (Hayley Horn) — see `appendix-sources.md`  
**Audience:** Internal HLS QBR (~80 · AE / BDR / SA / DSA / leaders)  
**Brand line:** `Databricks HLS · Office of the CFO`  
**Slug / sync:** `ocfo-qbr-enablement`  
**Ship to:** `hls/qbr-cfo-enablement/presentations/`  
**Files:** `ocfo-qbr-enablement-walkthrough.html` + `ocfo-qbr-enablement-speaker-notes.html`  
**Runtime:** ~45 min main narrative (slides 0–15) · **21 slides total** (16 main + 5 appendix)  
**Chrome:** Open speaker notes · navigation rail · keyboard nav · no live demo CTA · no calculator  

---

## Density rules

- On-slide: headline + one lead + visual. **No paragraph walls.**
- SOX exact language: **memo/page facsimile** (slide 4)
- SOX primer: **broadsheet clipping facsimile + four-step arc** (slide 2) — short section-primer title, visual carries the point; differentiated from the slide 4 memo facsimile and never adjacent to it
- Calendar / demo / tools / discovery: **interactive selectable states** with fixed geometry
- Visible slides: no `talk track` / `objection` / `ask them` / presenter meta
- Compete / cooperate / augment language on tool posture slides — not “objection handling”

---

## Slide list + composition map

| # | On-screen title (descriptive) | Eyebrow | Layout type |
|---|------------------------------|---------|-------------|
| 0 | Selling to the Office of the CFO | — | Minimal title |
| 1 | August 5 gave you the play; this hour is how finance decides to buy it | Framing | Before/after split |
| 2 | Why SOX exists | Vocabulary | Newspaper-clipping facsimile + cause/effect arc |
| 3 | HIPAA protects the record; SOX protects the integrity of the reported number | Vocabulary | Two halves with central hinge |
| 4 | Databricks supports SOX-compliant workloads; no cloud provider holds a SOX certification | Client need | Document facsimile |
| 5 | Run SOX as their control environment on Unity Catalog, with Audit in the room | Recommendation | Numbered sequence (3) + reference panel (static) |
| 6 | A CPA hears “ask anything in plain language” as a control failure | Problem space | Persona quote bubbles (4, alternating sides) |
| 7 | Seller vocabulary arrives in finance as unreviewed numbers and metric anarchy | Vocabulary | Three-column say → hear → should-say |
| 8 | Every Office of the CFO demo must prove the number is defined, traceable, reconciled, and controlled | Framing | Proof / status grid |
| 9 | Finance opens four different doors a month: flash-to-close, forecast, board, and audit | Framing | Persistent visual, selectable states |
| 10 | Land Finance Transformation, pass the Controller’s exam, then earn the CFO mandate | Options | Architecture flow |
| 11 | One four-beat demo contract you can run tomorrow on margin or PMPM | Recommendation | Selectable standard cards + stage cues |
| 12 | Most finance variance is operational, and the planning model cannot reach that data | Problem space | Selectable example cards over a two-lane hinge stage |
| 13 | Where to feed the finance stack, and where to leave the workflow alone | Options | Persistent visual, selectable states |
| 14 | Translate a line-of-business win you already have into an Office of the CFO ask | Recommendation | Document facsimile, click-to-reveal boxes |
| 15 | Trust before wow. SOX without the myth. Their calendar. The demo contract. | — | Minimal close |
| 16 | Finance outcomes organize as compress, multiply, and defend | Appendix | Rule-block grid (3) |
| 17 | Lead with scorecard units — days, dollars, basis points — not platform nouns | Appendix | Boundary / glossary grid |
| 18 | Discovery that maps to their scorecard, not our feature list | Appendix | Selectable states + fixed panel |
| 19 | ERP and EPM stay as systems of record; Databricks is the governed intelligence layer | Appendix | Rule-block grid (3) |
| 20 | Eight questions this room asks after the hour, and the answers that hold up | Appendix · what the room asks | Selectable question rail + fixed answer panel |

### Required additions (shipped)

- **A) SOX primer (Enron framing)** → slide 2 (main arc, opens SOX block after Frame)
- **B) HIPAA vs SOX** → slide 3 (main arc, before exact answer)
- **C) Compete/coop EPM tools** → slide 13 (replaces plain pushbacks)
- **Demo consolidation** → slide 11 combines the four-beat standard with live screen/sentence cues; the redundant poster slide was removed
- **Operational variance wedge** → slide 12 opens the Field block: why the variance finance argues about is operational, three verticals (medtech gross margin, payer PMPM, pharma gross-to-net), and why both sides of the join already live in one place
- **Field Guide appendix** → slides 16–19 (pillars, vocab, discovery bank, stack cooperate)
- **Q&A prep** → slide 20 closes the appendix: eight anticipated field questions with say / then / never lines; two overflow questions and the vertical variations live in the notes only

### Rail OUTLINE

```js
const OUTLINE = [
  ['Frame',    [['Open', [0, 1]]]],
  ['SOX',      [['Primer', [2]], ['Contrast', [3]], ['Answer', [4]], ['Playbook', [5]]]],
  ['Trust',    [['Buy', [6, 7, 8]]]],
  ['Land',     [['Timing', [9]], ['Champion', [10]]]],
  ['Demo',     [['Contract + run', [11]]]],
  ['Field',    [['Variance', [12]], ['Tools', [13]], ['Expand', [14]]]],
  ['Close',    [['Standards', [15]]]],
  ['Appendix', [['Pillars', [16]], ['Vocab', [17]], ['Discover', [18]], ['Stack', [19]], ['Questions', [20]]]],
];
```

---

## Interactive specs (fixed geometry)

| Slide | States | Pinned |
|---|---|---|
| 9 Calendar | close · forecast · board · audit | timeline + detail panel height |
| 11 Demo | Surface · Explain · Reconcile · Govern | standard card rail + 288/168 screen/sentence stage tracks |
| 12 Variance | Medtech gross margin · Payer PMPM · Pharma gross-to-net | 112px card row; one 1280×320 stage viewBox; gap figure computed from plan/actual |
| 13 Tools | BlackLine · FloQast · Adaptive · Anaplan · Planful · OneStream · Oracle EPM · HFM | 2×2 matrix (protect↔truth-layer × consumption) + fixed detail panel |
| 14 Worksheet | 4 boxes reveal on click (+ Reveal all / Reset) | 132px box min-height; 82px meeting-ask strip |
| 18 Discovery | Close · Forecast · Cash · Spend · Controls · Wins | 320px panel; Q count from data |
| 20 Questions | 8 question cards (stack · SOX · Genie · seat · IT · demo · private · Audit) | 8-row rail at equal height; 96px head + 3 fixed answer rows |

---

## Notes strategy

- Port say / purpose / transition / discovery from `slide-guide-ocfo-qbr.md`
- Slide 2 notes: Enron opener + one-minute SOX mental model for non-finance sellers
- Slide 4 notes: full SOX never-say + verbatim highlights
- Slide 5 notes: cue order 01–03 matches the on-slide numbered moves; the control map is reference for move two, and the SoD / warehouse-access question is asked inside move three
- Slide 8 notes: Databricks proves definition, lineage, reconciliation, and control; the customer owns the business action
- Slide 11 notes: separate reconciliation evidence from governed-access evidence; stop before claiming the customer action
- Slide 12 notes: the plan / actual figures are illustrative shapes, not benchmarks; this is not a compete slide against EPM — the feed play is the next slide
- Slide 15 notes: BDR / AE / SA / DSA week actions + leader deal-review asks
- Appendix notes: Field Guide attribution + expanded banks / ROI anchors
- Slide 20 notes: one cue group per question plus the two overflow questions (Aug 5 differentiation, Salesforce / UCO tagging), provider vs payer vs biotech variation, and the “I don’t know — I’ll get you the exact language” fallback
- Discovery distributed across main notes (5, 7, 8, 9, 12, 14) + full bank on slide 18

---

## Status

- [x] Skill + design system read  
- [x] Source guide + SOX verbiage locked  
- [x] Field Guide fetched and appendixed  
- [x] Composition map (≥6 layouts, no adjacent repeats in main arc)  
- [x] Build deck + notes  
- [x] SOX education reorder: primer → HIPAA vs SOX → exact answer → playbook  
- [x] Section order: Frame → SOX → Trust → Land → Demo → Field → Close → Appendix  
- [x] Validation: composition / language / titles / sync count  
