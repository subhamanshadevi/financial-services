## Northlake firm overrides (appended to pitch-agent.md by TCS)

### Skills to load first
`northlake-pitch-conventions`, then `northlake-template`. Their rules win over other skill defaults.

### Gates
- **G1 — peer set.** After screening peers and precedents, stop. Present the peer table, the precedent table and `04_Peer_Selection_Rationale.md`. Wait for the VP's approval or edits. Log the decision and approver.
- **G2 — valuation.** After the workbook is built and its checks pass, stop. Wait for VP then MD approval.
- **G3 — release.** After deck QC, stop. Only the MD releases the deck.

### Additional steps
- After the football field: run `/buyer-list` against `09_Buyer_Universe_Seed_List.xlsx` and `08_Northlake_Credentials.xlsx`; write `05_Buyer_Universe_Longlist.xlsx` ranked High / Medium / Low with the reason for each.
- After G3: draft a cover note (plain text, for the MD to paste into Outlook). Do not send it.
- Throughout: append every sourced figure, gate decision and approver to `07_Source_Register_and_Run_Log.json`.

### Demo data rule (sprint only)
Licensed connectors are disabled. Files `03_Peer_Universe_Market_Data.xlsx` and `04_Precedent_Transactions.xlsx` are the authoritative market data. Cite file, sheet and row for every figure, and use each file's as-of date as the retrieval date. All companies are fictional; do not look them up on the web.

### Output names
01_Project_Keystone_Valuation_Model.xlsx · 02_Project_Keystone_Pitchbook.pptx · 03_Deck_QC_Report.md · 04_Peer_Selection_Rationale.md · 05_Buyer_Universe_Longlist.xlsx · 06_Cover_Note_Draft.eml · 07_Source_Register_and_Run_Log.json · 08_Approvals_Record.md
