# The Home Depot | Financial Performance & Valuation

**Independent undergraduate finance portfolio project**  
**Shahriar Molhem** | BBA Finance | University of Georgia, Terry College of Business

> **Status: Financial analysis and project files completed; private final owner review and public-release approval pending.** This is an undergraduate case study, not a CPA/audit opinion, professional appraisal, issuer report or investment recommendation.

## The headline

Between fiscal 2021 and fiscal 2025, Home Depot's reported net sales increased **8.9%**, while reported operating earnings fell **9.3%**. Operating margin decreased from **15.2% to 12.7%**. A simplified FY2025-date FCFF DCF exercise produces **$265.54/share** under assumptions of 8.0% WACC and 2.5% perpetual growth. The valuation is **not** a current market-price target and changes considerably when assumptions change.

## Start here

| Resource | What it offers |
| --- | --- |
| [Executive summary](reports/executive-summary.md) | Recruiter-friendly overview of the main findings |
| [Historical financial performance](reports/financial-performance.md) | Five-year reported sales, earnings and cash flow analysis |
| [DCF valuation and scenarios](reports/valuation-and-scenarios.md) | Forecast assumptions, per-share valuation and WACC/g grid |
| [Historical source CSV](data/historical-financials.csv) | SEC-reported fiscal-year financial statement figures |
| [Model specification](models/valuation-model-specification.md) | Reproducible DCF methods and formulas |
| [Data source register](data/source-register.md) | Official SEC filings and extraction rules |
| [Presentation outline](presentations/presentation-outline.md) | Ten-slide speaker deck structure |
| [Interview brief](reports/interview-brief.md) | Talking points and limitations for recruiters |
| [Validation checklist](quality/release-readiness.md) | Completed formula checks and publication blockers |

## Deliverables and availability

| Deliverable | Status |
| --- | --- |
| Source-linked research reports (Markdown) | Available in repository |
| Fiscal 2021–2025 input data (CSV) | Available in repository |
| Historical and DCF calculation methodology | Available in repository |
| [Excel model (10 worksheets)](models/home_depot_financial_model_with_dcf.xlsx) | **Uploaded to repository; ZIP integrity and file identity verified** |
| [PowerPoint presentation (10 slides + speaker notes)](presentations/home_depot_financial_analysis_presentation.pptx) | **Uploaded to repository; ZIP integrity and file identity verified** |

**Publication gate:** Both binary files have been uploaded and file-integrity checked. Keep this repository Private until its owner has reviewed the materials and explicitly approves public release. No independent CPA/audit or professional valuation certification is implied.

## Project workflow

- **PR #1:** Research scope, methodology and SEC source register.
- **PR #2:** Extracted five-year financial statements, historical analysis and reconciliation.
- **PR #3:** Educational FCFF model specification, base-case valuation and sensitivity analysis.
- **PR #4:** Executive summary, interview brief, presentation documentation and final publication checks.

## Technical approach

- Primary data: public Form 10-K reporting for FY2021–FY2025.
- Historic metrics: growth, profitability, selected balance-sheet efficiency and operating cash flow.
- Illustrative DCF: after-tax EBIT + noncash D&A − capex − modeled increase in operating working capital.
- Forecast inputs: author-selected assumptions, clearly separated from reported facts.
- Validation: reconciliation tests, source trace register and scenario consistency controls.
- Communication: executive narrative and 10-slide speaker deck appropriate to a BBA finance student.

## Critical limitations

- FY2024 had 53 weeks, unlike adjacent 52-week years.
- Acquisitions (SRS in FY2024 and GMS in FY2025) limit simple year-over-year organic comparisons.
- WACC of 8% and g of 2.5% are illustrative, not derived current-market estimates.
- The model uses a simplified enterprise-to-equity bridge; leases and certain other potential adjustments are not exhaustively treated.
- About 77.6% of the calculated enterprise value is discounted terminal value.

**Source:** [Home Depot FY2025 SEC Form 10-K](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/hd-20260201.htm) · [Home Depot Investor Relations](https://ir.homedepot.com/financial-reports/annual-reports/recent)

**Disclosure:** Independent student analysis, with AI-assisted drafting and calculation support; not a third-party-verified professional valuation. Historical results should be differentiated from model assumptions and interpreted with disclosures.
