# Source provenance

Collected 9 October 2026. Each source file identifies its origin; [manifest.json](sources/manifest.json) records retrieval methods and transformations.

| Material | Origin | Treatment |
| --- | --- | --- |
| Two complete call transcripts | Grain, meetings `e149b72b-1426-4a12-9f0d-f8937a53e16c` and `52e8f957-9051-4221-ab97-c152f8cf3d18` | Financial figures withheld; speaker labels, timestamps and remaining wording retained |
| Company, deal, two contacts, referral contact, workspace links and two tasks | Attio MCP | Native returned text inside JSON; financial values withheld and public enrichment fields omitted as recorded in each file |
| Reach handover | Notion page `3f24d7a6-0990-81e4-9760-e826cc26ed33`, linked from Attio | Page body retained with financial amounts withheld |
| Jesse’s video | User-supplied YouTube URL; transcript retrieved via Firecrawl | Machine transcript retained, including transcription errors |
| P&Ls and scenario assumptions | Created for this exercise | Synthetic; no actual client financial values |

## Reading the sources

The September call starts with Silas, who leaves at approximately 01:23. Kathryn provides the substantive client context. The October call is between Kathryn and Juan. No separate substantive founder interview was found in the company-filtered Grain results.

CRM and handover text is existing internal interpretation, not a new answer key. The sources can disagree, contain transcription errors, or reflect different dates. In particular, the Attio workspace links include a record labelled TEST; it is not evidence of actual staffing. Source links and record IDs identify provenance, not a guarantee of accuracy.

Source monetary amounts, client allocation percentages and relevant financial fields are replaced with explicit withholding markers. They were not replaced silently with P&L totals: ARR, historical refunds and annual revenue are different measures. The synthetic P&Ls govern exercise calculations. Original private recording/page links that would bypass these redactions are not included. Jesse’s briefing is provided; public company/team research is left to the candidate.

## Coverage and gaps

- Grain company-filtered listing returned two meetings and no next cursor. Both full transcripts are included.
- Attio returned one matching company and one linked deal, two company contacts, a referral contact, two workspace records and two deal tasks. These directly related records are included.
- Searches found no notes attached to the company, deal, founder or finance contact; no company/deal comments; no company tasks; and no company-linked Attio call recordings.
- Domain-filtered email search returned no results and no next page. A second semantic search including other workspace members also returned no results. This is a limit of accessible results, not proof that emails do not exist.
- The linked Notion handover was retrieved in full. No underlying payroll exports, supplier contracts, historical claim spreadsheets, technical tickets, experiment logs or accounting-system attachments were retrieved. Mentions of those materials do not mean they are included.

The exact accounting dates, amounts and headcount averages are exercise assumptions. Historical estimates in the calls are not audited headcount reconciliations. CRM summaries are secondary evidence; the transcripts retain what was actually recorded.

The scenario adds two fictional US research hires to the historical team. Their dates and employing entity are specified in `data/scenario.json`; their costs are included only in the aggregate US accounts. This explicit exercise variation takes precedence over source statements about US staffing.
