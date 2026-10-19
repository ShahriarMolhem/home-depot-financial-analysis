# Primary Data Source Register

**Company:** The Home Depot, Inc. (NYSE: HD; SEC CIK 0000354950)  
**As-of research date:** October 18, 2026  
**Historical annual study:** FY2021 through FY2025

## Verified filing entry points
| Fiscal label | Fiscal year ended | Primary Form 10-K | Source type |
| --- | --- | --- | --- |
| FY2025 | February 1, 2026 | [SEC 10-K FY2025](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/hd-20260201.htm) | SEC filing |
| FY2024 | February 2, 2025 | [SEC 10-K FY2024](https://www.sec.gov/Archives/edgar/data/354950/000035495025000085/hd-20250202.htm) | SEC filing |
| FY2023 | January 28, 2024 | [SEC 10-K FY2023](https://www.sec.gov/Archives/edgar/data/354950/000035495024000062/hd-20240128.htm) | SEC filing |
| FY2022 | January 29, 2023 | [SEC 10-K FY2022](https://www.sec.gov/Archives/edgar/data/354950/000035495023000059/hd-20230129.htm) | SEC filing |
| FY2021 | January 30, 2022 | [SEC 10-K FY2021](https://www.sec.gov/Archives/edgar/data/354950/000035495022000070/hd-20220130.htm) | SEC filing |

Supporting official references:
- [Home Depot annual report archive](https://ir.homedepot.com/financial-reports/annual-reports/recent)
- [Home Depot investor documents](https://ir.homedepot.com/investor-resources/investor-documents)
- [Fiscal 2025 fourth-quarter and full-year earnings release (February 24, 2026)](https://ir.homedepot.com/~/media/Files/H/HomeDepot-IR/press-release/q4-2025-earnings-release.pdf)
- [FY2025 SEC filing index, filed March 18, 2026](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/0001628280-26-019436-index.html)

## Extraction and documentation protocol
For **every material reported number**, capture:
1. Fiscal year, statement and original account label;
2. Form 10-K URL and exact page, financial-statement heading, note, or table;
3. Originally reported unit (e.g., millions), original sign and displayed rounding;
4. Mapped standardized line item, normalization rationale, and any restatement/filing-version caveat;
5. Cross-check against overlapping years in another report before committing the final dataset.

## Expected source categories
| Model area | Expected location within SEC annual report |
| --- | --- |
| Sales, cost of sales, operating income, taxes, net income | Consolidated Statements of Earnings |
| Inventory, receivables, cash, payables, debt, equity | Consolidated Balance Sheets |
| Cash from operations, capex, buybacks, dividends | Consolidated Statements of Cash Flows |
| Comparable sales, product mix, margin explanations | Management Discussion & Analysis |
| Acquisitions, debt terms, commitments, accounting policies | Notes to Consolidated Financial Statements |

## Data governance
- Do not invent or silently interpolate missing historical data.
- If a statement field is unavailable or definitions change, mark `N/A` and explain.
- Treat forecasts and interest-rate/market assumptions as **analyst assumptions**, never as historical reported facts.
- Do not copy entire SEC reports into this repository; cite and link source documents, extract only the small tables/figures needed for analysis.
- Equity-price or treasury-rate data (if included) require a separately dated, attributable source and retrieval date.

## Dataset status
**Not yet extracted.** This register identifies official sources, not completed financial model inputs. Historical values and calculated results will be committed in the model-development PR after independent checks.
