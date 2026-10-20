# Home Depot | Financial Performance & Valuation

**Shahriar Molhem** · BBA Finance, University of Georgia — Terry College of Business  
**Skills practiced:** Financial statement analysis, Excel modeling, discounted cash flow (DCF), sensitivity analysis

## Why this project?

I wanted to understand why a company could grow its sales without growing its operating profit. I used Home Depot's FY2021–FY2025 SEC filings to explore the difference, then built a simple valuation model to see how much the answer changes when the assumptions change.

## Key findings

- **Sales grew while operating profit declined.** Revenue went from **$151.2 billion** in FY2021 to **$164.7 billion** in FY2025 (+8.9%); operating income went from **$23.0 billion** to **$20.9 billion** (−9.3%).
- **Margins tightened.** Operating margin fell from **15.2%** to **12.7%** over the same period.
- **Cash flow offered another perspective.** FY2025 operating cash flow was **$16.3 billion**. After **$3.7 billion** of capital expenditures, simplified free cash flow was **$12.6 billion**.
- **The valuation depends heavily on assumptions.** My illustrative five-year FCFF model yields **$265.54 per share** using **8.0% WACC** and **2.5% perpetual growth**; **77.6%** of estimated enterprise value comes from the terminal value.

The DCF is a *hypothetical model outcome as of FY2025 year-end*, **not** a current price target. FY2024 also contained 53 weeks, and acquisitions affect comparisons.

## Project files

| Resource | What you'll find |
| --- | --- |
| [Executive summary](reports/executive-summary.md) | Main findings in plain English |
| [Historical financial performance](reports/financial-performance.md) | Five-year sales, earnings, and cash flow |
| [DCF analysis and sensitivity](reports/valuation-and-scenarios.md) | Forecast assumptions, value bridge, and uncertainty |
| [Excel workbook](models/home_depot_financial_model_with_dcf.xlsx) | Historical ratios, DCF formulas, checks, and scenario tables |
| [Historical data](data/historical-financials.csv) · [SEC sources](data/source-register.md) | Reported inputs and their original filings |
| [Presentation](presentations/home_depot_financial_analysis_presentation.pptx) | Ten-slide overview |
| [Slide-by-slide speaking script](presentations/slide-by-slide-speaking-script.md) | English practice transcript for the deck |
| [Methodology](reports/methodology.md) · [Review notes](quality/release-readiness.md) | Assumptions, controls, and remaining limitations |

## How I worked through it

I started with the reported financial statements, calculated trends and cash flow measures, and used forecast assumptions to model unlevered free cash flow. I then tested how changing WACC and terminal growth affects the implied equity value. The [valuation specification](models/valuation-model-specification.md) shows the underlying logic.

**Primary source:** [Home Depot FY2025 Form 10-K](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/hd-20260201.htm).

*This is an undergraduate project based on public filings, with AI-assisted drafting and calculation support. It is not an audit, professional appraisal, or investment recommendation. The assumptions and source values require the author's understanding and review.*
