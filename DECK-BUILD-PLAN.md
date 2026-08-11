# Walkthrough deck — build plan (shipped)

**Skill:** customer-walkthrough-deck  
**Sources:** `slide-guide-ocfo-qbr.md` · [Selling to CFOs Field Guide v2.0](https://docs.google.com/document/d/11J4Bdh5_cBlE-NoZ9b_W4acO__hGWqgo2vBIrzSpWGo) (Hayley Horn) — see `appendix-sources.md`  
**Audience:** Internal HLS QBR (~80 · AE / BDR / SA / DSA / leaders)  
**Brand line:** `Databricks HLS · Office of the CFO`  
**Slug / sync:** `ocfo-qbr-enablement`  
**Ship to:** `hls/qbr-cfo-enablement/presentations/`  
**Files:** `ocfo-qbr-enablement-walkthrough.html` + `ocfo-qbr-enablement-speaker-notes.html`  
**Runtime:** ~45 min main narrative (slides 0–13) · **18 slides total** (14 main + 4 appendix)  
**Chrome:** Open speaker notes · navigation rail · keyboard nav · no live demo CTA · no calculator  

---

## Density rules

- On-slide: headline + one lead + visual. **No paragraph walls.**
- SOX exact language: **document facsimile**
- Calendar / demo / tools / discovery: **interactive selectable states** with fixed geometry
- Visible slides: no `talk track` / `objection` / `ask them` / presenter meta
- Compete / cooperate / augment language on tool posture slides — not “objection handling”

---

## Slide list + composition map

| # | On-screen title (descriptive) | Eyebrow | Layout type |
|---|------------------------------|---------|-------------|
| 0 | Selling to the Office of the CFO | — | Minimal title |
| 1 | August 5 gave you the play; this hour is how finance decides to buy it | Framing | Before/after split |
| 2 | A CPA hears “ask anything in plain language” as a control failure | Problem space | Rule-block grid (4) |
| 3 | Seller vocabulary arrives in finance as unreviewed numbers and metric anarchy | Vocabulary | Side-by-side comparison |
| 4 | Every Office of the CFO demo must land definition, lineage, reconciliation, and action | Framing | Proof / status grid |
| 5 | Databricks supports SOX-compliant workloads; no cloud provider holds a SOX certification | Client need | Document facsimile |
| 6 | HIPAA protects the record; SOX protects the integrity of the reported number | Vocabulary | Two halves with central hinge |
| 7 | Run SOX as their control environment on Unity Catalog, with Audit in the room | Recommendation | Boundary / parameter matrix |
| 8 | Finance opens four different doors a month: close, forecast, board, and audit | Framing | Persistent visual, selectable states |
| 9 | Land Finance Transformation, pass the Controller’s exam, then earn the CFO mandate | Options | Architecture flow |
| 10 | One four-beat demo contract you can run tomorrow on margin or PMPM | Recommendation | Selectable standard cards + stage cues |
| 11 | Planning and close platforms stay; we feed the governed truth they never see | Options | Persistent visual, selectable states |
| 12 | Translate a line-of-business win you already have into an Office of the CFO ask | Recommendation | Document facsimile, click-to-reveal boxes |
| 13 | Trust before wow. SOX without the myth. Their calendar. The demo contract. | — | Minimal close |
| 14 | Finance outcomes organize as compress, multiply, and defend | Appendix | Rule-block grid (3) |
| 15 | Lead with scorecard units — days, dollars, basis points — not platform nouns | Appendix | Boundary / glossary grid |
| 16 | Discovery that maps to their scorecard, not our feature list | Appendix | Selectable states + fixed panel |
| 17 | ERP and EPM stay as systems of record; Databricks is the governed intelligence layer | Appendix | Rule-block grid (3) |

### Required additions (shipped)

- **A) HIPAA vs SOX** → slide 6 (main arc, near SOX block)
- **B) Compete/coop EPM tools** → slide 11 (replaces plain pushbacks)
- **Demo consolidation** → slide 10 combines the four-beat standard with live screen/sentence cues; the redundant poster slide was removed
- **Field Guide appendix** → slides 14–17 (pillars, vocab, discovery bank, stack cooperate)

### Rail OUTLINE

```js
const OUTLINE = [
  ['Frame',    [['Open', [0, 1]]]],
  ['Trust',    [['Buy', [2, 3, 4]]]],
  ['SOX',      [['Answer', [5]], ['Contrast', [6]], ['Playbook', [7]]]],
  ['Land',     [['Timing', [8]], ['Champion', [9]]]],
  ['Demo',     [['Contract + run', [10]]]],
  ['Field',    [['Tools', [11]], ['Expand', [12]]]],
  ['Close',    [['Standards', [13]]]],
  ['Appendix', [['Pillars', [14]], ['Vocab', [15]], ['Discover', [16]], ['Stack', [17]]]],
];
```

---

## Interactive specs (fixed geometry)

| Slide | States | Pinned |
|---|---|---|
| 8 Calendar | close · forecast · board · audit | timeline + detail panel height |
| 10 Demo | Surface · Explain · Prove · Act | standard card rail + 288/168 screen/sentence stage tracks |
| 11 Tools | BlackLine · FloQast · Adaptive · Anaplan · Planful · OneStream · Oracle EPM · HFM | 2×2 matrix (protect↔truth-layer × consumption) + fixed detail panel |
| 12 Worksheet | 4 boxes reveal on click (+ Reveal all / Reset) | 132px box min-height; 82px meeting-ask strip |
| 16 Discovery | Close · Forecast · Cash · Spend · Controls · Wins | 320px panel; Q count from data |

---

## Notes strategy

- Port say / purpose / transition / discovery from `slide-guide-ocfo-qbr.md`
- Slide 5 notes: full SOX never-say + verbatim highlights
- Slide 13 notes: BDR / AE / SA / DSA week actions + leader deal-review asks
- Appendix notes: Field Guide attribution + expanded banks / ROI anchors
- Discovery distributed across main notes (3, 4, 7, 8, 12) + full bank on slide 16

---

## Status

- [x] Skill + design system read  
- [x] Source guide + SOX verbiage locked  
- [x] Field Guide fetched and appendixed  
- [x] Composition map (≥6 layouts, no adjacent repeats in main arc)  
- [x] Build deck + notes  
- [x] Validation: composition / language / titles / sync count  
