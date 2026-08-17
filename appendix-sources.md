# Appendix sources — OCFO QBR enablement deck

## Document pulled

| Field | Value |
|---|---|
| Title | Selling to Chief Financial Officers: The Databricks Field Guide |
| Author / version | Hayley Horn · 2026-05-03 · v2.0 |
| Doc ID | `11J4Bdh5_cBlE-NoZ9b_W4acO__hGWqgo2vBIrzSpWGo` |
| URL | https://docs.google.com/document/d/11J4Bdh5_cBlE-NoZ9b_W4acO__hGWqgo2vBIrzSpWGo/edit |
| Fetched | Via Google Docs API (ADC / google_auth) |

## What the doc contained (brief)

1. **Why CFOs buy differently** — outcome buyers (accuracy, speed, cost, control); scorecard metrics (days to close, forecast accuracy, DSO, audit readiness).
2. **Modern CFO pressures** — steward→strategist, continuous close, AI forecasting, automated assurance, value intelligence.
3. **Three pillars** — Compress the Cycle · Multiply the Visibility · Defend the Margin (with use-case families: P2P/O2C, spend/contracts/treasury/BvA, rev rec + AI ROI attribution).
4. **Databricks advantage** — unified financial data, auditable by design (UC), AI-ready, works *with* ERP/EPM stack (not replace).
5. **CFO vocabulary** — DSO, DPO, EBIT, CCC, bps, run-rate, EBITDA bridge + “AI yes, with controls” framing.
6. **Stack cooperate lines** — ERP stays; Anaplan/Excel stay; regulated-function governance answer; ROI benchmarks; failed-DW recovery path.
7. **Discovery question bank** — Close, Forecasting, Revenue/Cash, Spend, Governance, Quick wins.
8. **Pipeline context** — finance use-case category counts (reference only; not put on slides).

## What we did with it

| Content | Treatment |
|---|---|
| Three pillars | **Appendix slide 16** (index 15) |
| CFO vocabulary + Daniel framing | **Appendix slide 17** (index 16) |
| Discovery banks | **Appendix slide 18** interactive (index 17); selected Qs also in main notes |
| ERP / EPM / regulated cooperate lines | **Appendix slide 19** (index 18); echoes main compete/coop slide 13 |
| ROI / DSO math | Notes only (illustrative benchmarks — not on-slide quotes) |
| Pipeline DBU table | **Not used** (internal pipeline stats; not enablement-critical for this hour) |
| Deep use-case KPI lists (80% touchless, etc.) | **Notes / skip** — too dense for sparse slides; available in source doc |

## Main-arc changes from this doc

**None required for pillars/vocab.** Trust, SOX exact language, HIPAA vs SOX, calendar, champion path, demo contract were already planned. Field Guide material filled **reference gaps** (pillars, vocab, discovery bank, stack cooperate) → appendix so the live ~45 min stays intact.

**Compete / coop tool vocabulary (slide 13 interactive)** expanded beyond the Field Guide’s Anaplan/BlackLine/OneStream mentions so HLS hears the stack that actually shows up:

| On-slide (8) | Notes-only |
|---|---|
| BlackLine, FloQast | Cadency / Trintech |
| Adaptive, Anaplan, Planful | Pigment |
| OneStream, Oracle EPM / FCCS | SAP Analytics Cloud / BPC (SAP-heavy accounts) |
| Oracle HFM (Hyperion Financial Management) | — clarify HFM ≠ FCCS/EPM Cloud |

Default posture unchanged: usually augment / feed governed truth; displace only when honest (HFM retirement path).

**Slide 13 redesigned as a 2×2 positioning matrix** (presenter feedback: the spectrum "read as meaningless"). Axes:
- X: **Leave their workflow alone** (left) ←→ **We become their source of truth** (right) — replaces the compete/cooperate axis.
- Y: **Our Databricks consumption** — low (bottom) → high (top).
- Quadrants are named as plays, derived from the JS array rather than hand-typed: **Best expansion play** (source of truth + high, “feed it first — biggest platform pull”), **Worth feeding** (source of truth + low, “same play, smaller platform pull”), **Win the data layer** (leave the workflow + high, “leave their workflow alone”), **Recognize it, don’t chase it** (leave the workflow + low, “no platform play here today”).

Placements: Anaplan / Adaptive / Planful / OneStream → Best expansion play; Oracle EPM/FCCS → Worth feeding; HFM → Win the data layer; BlackLine / FloQast → Recognize it, don’t chase it. Detail panel adds net-new education per tool: what it does, who owns it, how we help it, and where competing is honest.

## Other primary sources (unchanged)

- `slide-guide-ocfo-qbr.md` — session thesis, SOX verbatim, timing, roles
- QuidelOrtho SOX discussion deck / SOX positioning image — facsimile language on slide 6
- `customer-walkthrough-deck` skill templates — shell, rail, sync, interactives
