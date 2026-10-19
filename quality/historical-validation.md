# Model Validation — Historical FY2021–FY2025

The companion Excel workbook includes a **VALIDATION** worksheet. A zero difference indicates that the inputs and arithmetic agree with the disclosed totals within reported USD-million units; it does **not** certify that every input is free from classification or interpretive issues.

| Check | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Sales less cost of sales = gross profit | 0 | 0 | 0 | 0 | 0 |
| Gross profit less SG&A and operating D&A = operating income | 0 | 0 | 0 | 0 | 0 |
| Operating income less net interest/other = pretax | 0 | 0 | 0 | 0 | 0 |
| Pretax less income tax = net income | 0 | 0 | 0 | 0 | 0 |
| Assets less liabilities and equity | 0 | 0 | 0 | 0 | 0 |
| Current-asset subaccounts sum to current assets | 0 | 0 | 0 | 0 | 0 |
| OCF + ICF + financing CF = cash change before FX | 0 | 0 | 0 | 0 | 0 |
| Opening cash + cash change before FX + FX = ending cash | 0 | 0 | 0 | 0 | 0 |
| CF ending cash less balance-sheet cash | 0 | 0 | 0 | 0 | 0 |

### Reproduction
- CSV: `data/historical-financials.csv`, rows named as reported statement line items.
- Fiscal year columns: FY2021–FY2025; values are USD millions except per-share amounts and diluted average-share counts.
- **FY2020 opening values used for FY2021 averages:** inventory $16,627m, assets $70,581m, sourced from the FY2021 filing.
- Formulas: `operating margin = operating income / sales`; `simple FCF = OCF + signed capital expenditures`; `net working capital = current assets − current liabilities`.
- All percentages shown in reports are calculated and rounded, not separate source data.

**Review note:** A subsequent financial-model PR should test acquisition-normalized growth, complete the source trace to filing pages, and attach the workbook as a repository asset. This report does not claim a complete DCF valuation.
