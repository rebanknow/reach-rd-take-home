# Data dictionary

## P&L CSVs

UTF-8, comma-separated, with a header row. Numeric values have no currency symbols or thousands separators.

| Column | Meaning |
| --- | --- |
| `account` | Income, expense, calculated subtotal or employee metric |
| `unit` | `GBP`, `USD` or `people` |
| `q1`–`q4` | Amount incurred during the quarter, or the specified quarter headcount metric |
| `full_year_or_year_end` | Sum of quarters for money; average of quarterly averages for average employees; Q4 closing count for year-end employees |
| `basis` | Distinguishes synthetic inputs, calculated rows and headcount aggregation |

All financial and headcount inputs are synthetic. Revenue and expense inputs are positive. Losses are negative. Zero means zero, not unknown. Currency units are whole GBP or USD, not thousands. Average employee counts can be fractional.

## Calculated rows

- Total revenue = subscription revenue + implementation revenue.
- Total cost of sales = production cloud hosting + customer delivery services.
- Gross profit = total revenue − total cost of sales.
- Total employee costs = salaries and bonuses + employer payroll taxes/NIC + employer benefits/pensions + severance/redundancy.
- Total operating expenses = total employee costs + external data services + platform cloud and compute + software subscriptions + recruitment and people services + marketing and events + legal and accounting + workspace and utilities + travel and subsistence + insurance and administration + depreciation.
- Operating profit/(loss) = gross profit − total operating expenses.
- Profit/(loss) before tax = operating profit/(loss) + grant income + interest income − interest expense.
- Net profit/(loss) = profit/(loss) before tax − corporation tax expense/(credit).

Subtotal rows coexist with their component rows. Do not sum every CSV row: that would double-count expenses and mix headcounts with money. No R&D credit or deferred tax asset has been booked. Accounting profit/loss is not itself taxable profit/loss.

## JSON files

`scenario.json` records explicit exercise assumptions. Fee fractions are decimals (0.15 = 15%). `delivery_cost: null` means not supplied, not zero. The FX rate is GBP per USD and is an invented management-comparison assumption.

`public-team.json` records source URLs and self-reported public observations as of 9 October 2026. Public role, location and timing fields are textual evidence; they do not assign a salary, employing entity or qualifying R&D percentage. The number of public profiles is not the scenario payroll headcount.
