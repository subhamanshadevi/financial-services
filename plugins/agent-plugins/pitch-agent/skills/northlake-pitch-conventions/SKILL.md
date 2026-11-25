---
name: northlake-pitch-conventions
description: Northlake Capital Partners house rules for pitchbooks — peer and precedent selection, metric definitions, calendarisation, valuation ranges, formatting, footnotes and disclaimers. Use for every pitch, comps, precedents, DCF, LBO or football-field task for Northlake, before any other pitch skill runs.
---

# Northlake pitch conventions

Read `references/06_Northlake_Pitch_Conventions.md` and `references/07_Valuation_Methodology_Standards.md` in full before any work. Where they conflict with another skill's defaults, these rules win.

## Peer selection
- Six to eight trading peers in the same end markets (aerospace, medical, industrial precision components).
- Revenue $150M–$3B; LTM EBITDA margin within 8 percentage points of the target.
- Exclude conglomerates and companies with under 50% of revenue from precision components.
- Write `04_Peer_Selection_Rationale.md`: every candidate, included or excluded, with the rule applied.
- STOP after the peer set and precedents are screened (Gate G1). Present the table and the memo; wait for the VP's approval or edits.

## Precedents
- Control deals in the last five years; exclude distressed sales and minority stakes; 5–10 deals.

## Metrics
- EV = diluted market cap + net debt + minority interest + preferred.
- Adjusted EBITDA as reported; never mix LTM and NTM in one column.
- Target NTM EBITDA = 25% × current-year estimate + 75% × next-year estimate (LTM ending September).

## Valuation ranges
- Trading comps: 25th–75th percentile EV / NTM EBITDA (PERCENTILE.INC) × target NTM EBITDA.
- Precedents: 25th–75th percentile EV / LTM EBITDA × target LTM EBITDA.
- DCF: WACC 9.5% ± 1.0 pt at 3.0% terminal growth; sensitivity grid WACC 8.5–10.5% × growth 2.5–3.5%.
- LBO: 5.0x entry leverage, 8.0% interest, full sweep, 4-year hold, 10.0x exit; implied EV at 25% and 20% IRR.
- Illustrative range: overlap of comps and precedents, rounded to the nearest $10M. Label it "illustrative".
- STOP after the workbook is built (Gate G2).

## Workbook rules
- Tabs: Cover, Inputs, Comps, Precedents, DCF, LBO, Football Field, Checks, Sources.
- Blue = inputs, black = formulas, green = cross-sheet links. No hard-codes in calculation cells.
- Every input cell has a source in the Sources tab (file, sheet, cell or connector, retrieval date).
- Name the ranges the deck uses (for example `Comps_Median_NTM`, `FF_Range_Low`).

## Deck rules
- Use the `northlake-template` skill layouts. Section order per conventions §1.
- $M with one decimal in tables, none in headlines; multiples to one decimal with "x".
- Every chart and table footnoted: "Source: …" then "Note: …".
- Headlines are full-sentence messages, no trailing full stop, no superlatives without data.
- Final slide: disclaimer from `10_Compliance_Disclaimers.txt`, verbatim.
- Any figure without a source: mark `[UNSOURCED]`; a released deck must contain none.
- Run `ib-check-deck` and fix every tie-out finding before Gate G3.

## Never
- Never send email or messages; draft the cover note as text for the banker.
- Never use data the requesting banker is not entitled to see.
- Never estimate a missing multiple or figure.
