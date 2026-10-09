# Reach Industries — R&D upsell trial data

Draft v1 · Prepared 9 October 2026

This repository contains source material for assessing a UK R&D upsell. It is not a completed claim or a prescribed workflow. The final assessment brief will be supplied separately.

## Files

| File | Contents |
| --- | --- |
| `data/uk-pnl.csv` | Synthetic UK standalone accounts in GBP, plus aggregate employee counts |
| `data/us-pnl.csv` | Synthetic US standalone accounts in USD, plus aggregate employee counts |
| `data/scenario.json` | Accounting period, entities, currencies, scenario status and commercial assumptions |
| `data/public-team.json` | Publicly reported names, roles, locations, timing and source links |
| `context/accounting-notes.md` | Basis of preparation, cost descriptions and available supporting material |
| `context/business-notes.md` | Synthetic operational context and decision sought |
| `context/sources.md` | Public research sources and provenance |
| `DATA-DICTIONARY.md` | CSV fields, sign conventions and total calculations |

## Financial confidentiality and synthetic data

Reach's actual financial information is strictly prohibited from being shared in this exercise. Every financial figure here is invented. All scenario headcounts, accounting dates, contractual facts and operational vignettes are fictional. No actual or synthetic individual salaries are supplied; payroll exists only as entity-level aggregates.

Reach's identity, product and public team references are real. Public profiles are self-reported evidence, not verified payroll records. Scenario facts take precedence for this exercise. In particular, the two unnamed US research hires in the business notes are fictional additions, not claims about real people.

## Working with the data

Use any tools or resources you find useful. You may contact Caribou with questions or request time with Jesse. Please do not contact Reach or its employees.

The accounting period is 1 October 2025–30 September 2026. The accounts are standalone entity statements, not a consolidated group P&L. Salary figures are costs incurred in each quarter, not annual salary rates. No role-level or person-level payroll allocation is included.

The CSVs contain evaluated numeric values, not spreadsheet formulas. Derived totals were recalculated and checked before export; see the data dictionary for their definitions. When changing input figures, recompute the totals. No Excel file or spreadsheet application is required.
