# Home Depot: Illustrative FCFF Discounted Cash Flow Valuation

**Author:** Shahriar Molhem | Undergraduate BBA Finance | University of Georgia  
**Valuation reference date:** FY2025 year-end, February 1, 2026  
**Scope:** Educational valuation exercise, **not** a live stock-price target or investment recommendation.

## Executive summary

Using reported FY2025 results as a starting point and **independent student assumptions** for FY2026–FY2030, a five-year, unlevered free-cash-flow-to-the-firm (FCFF) model produces an **illustrative enterprise value of $318.9 billion**. After subtracting modeled net financial debt of **$54.4 billion**, the implied equity value is **$264.5 billion**. Dividing by **996 million year-end shares** yields **$265.54 per share** under the *base-case assumptions*, **not** an observed market value.

These values are illustrative outputs of a simplified model, not predictions. **77.6%** of modeled enterprise value derives from the discounted terminal value; this makes the result particularly sensitive to WACC and perpetual growth.

## Reported starting point (actual FY2025, USD millions)

| Reported metric | FY2025 | Source |
| --- | ---: | --- |
| Sales | 164,683 | [FY2025 SEC Form 10-K, consolidated earnings](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/hd-20260201.htm) |
| Operating income | 20,890 | Same |
| Depreciation and amortization (cash flow statement) | 4,121 | Same, cash flows |
| Capital expenditures, absolute outflow | 3,679 | Same, cash flows |
| Cash and equivalents | 1,389 | Same, balance sheet |
| Short-term debt | 4,464 | Same, balance sheet |
| Current maturities of long-term debt | 4,967 | Same, balance sheet |
| Long-term debt, excluding current maturities | 46,341 | Same, balance sheet |
| Year-end common shares, millions | 996 | Same, balance sheet |

**Operating working capital baseline:** $11,427 million, defined as (receivables + inventory + other current assets) less (accounts payable + accrued salaries/expenses + sales taxes payable + deferred revenue + income taxes payable + other accrued expenses), excluding cash, debt and lease liabilities. Derived from FY2025 balance sheet line items. This is a **simplified model definition** and must not be confused with the current ratio's net working capital.

## Student assumptions (not issuer guidance)

| Input | FY2026 | FY2027 | FY2028 | FY2029 | FY2030 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Revenue growth | 3.0% | 3.2% | 3.2% | 3.0% | 2.8% |
| Operating profit margin | 12.9% | 13.0% | 13.2% | 13.3% | 13.4% |
| Modeled cash tax rate | 24.0% | 24.0% | 24.0% | 24.0% | 24.0% |
| Cash-flow D&A / sales | 2.5% | 2.5% | 2.5% | 2.5% | 2.5% |
| Capital expenditures / sales | 2.3% | 2.3% | 2.3% | 2.3% | 2.3% |
| Operating working capital / sales | 7.0% | 7.0% | 7.0% | 7.0% | 7.0% |

**Base-case discount rate (WACC): 8.0%**; **terminal perpetual FCFF growth: 2.5%.** These are chosen for an illustrative academic exercise; they are **not independently derived market-cost-of-capital estimates**. A more advanced valuation should estimate WACC from observable capital-market inputs and consider alternate terminal-value approaches.

## Calculation method

For each future year:

```text
Sales_t = Sales_(t-1) × (1 + growth_t)
EBIT_t = Sales_t × Operating_margin_t
NOPAT_t = EBIT_t × (1 − tax_rate_t)
D&A_t = Sales_t × D&A_as_%_of_sales
Capex_t = Sales_t × Capex_as_%_of_sales
Operating_NWC_t = Sales_t × NWC_as_%_of_sales
ΔNWC_t = Operating_NWC_t − Operating_NWC_(t-1)
FCFF_t = NOPAT_t + D&A_t − Capex_t − ΔNWC_t

Enterprise Value =
    Σ_{t=1..5}[FCFF_t/(1+WACC)^t]
    + [FCFF_5 × (1+g) / (WACC−g)] /(1+WACC)^5

Equity Value = Enterprise Value − Net Financial Debt
Per-share Value = Equity Value / FY2025 year-end shares
```

The base model is **not** adjusted for all operating lease liabilities and other potential nonoperating assets/liabilities, nor for future acquisitions or detailed debt changes. It treats FCFF as free cash flow **before** financing and uses year-end reported shares rather than forecast dilution.

## Forecast results (USD millions)

| | FY2026 | FY2027 | FY2028 | FY2029 | FY2030 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Sales | 169,623 | 175,051 | 180,653 | 186,073 | 191,283 |
| EBIT | 21,881 | 22,757 | 23,846 | 24,748 | 25,632 |
| NOPAT | 16,630 | 17,295 | 18,123 | 18,808 | 19,480 |
| FCFF | 16,522 | 17,265 | 18,092 | 18,801 | 19,498 |
| Discounted FCFF | 15,299 | 14,802 | 14,362 | 13,819 | 13,270 |

All projections above are formula-generated from the assumptions—not reported future company performance.

## Valuation bridge

| Component | Value (USD millions) |
| --- | ---: |
| Present value of forecast FCFF (5 years) | 71,552 |
| Terminal value (undiscounted at FY2030) | 363,374 |
| Present value of terminal value | 247,306 |
| **Enterprise value** | **318,858** |
| Less: financial debt (short-term + current long-term + noncurrent long-term) | (55,772) |
| Add: cash | 1,389 |
| **Equity value** | **264,475** |
| FY2025 year-end shares (millions) | 996 |
| **Illustrative equity value per share** | **$265.54** |

The terminal value comprises **77.6%** of enterprise value. A forecast model with such a large terminal component should never be presented as providing a precise intrinsic value.

## Sensitivity: value per share in USD

| WACC ↓ / perpetual growth → | 1.5% | 2.0% | 2.5% | 3.0% | 3.5% |
| --- | ---: | ---: | ---: | ---: | ---: |
| 6.50% | 310.31 | 344.13 | 386.40 | 440.75 | 513.21 |
| 7.25% | 262.25 | 286.76 | 316.42 | 353.07 | 399.49 |
| **8.00%** | **225.29** | **243.74** | **265.54** | **291.70** | **323.68** |
| 8.75% | 195.98 | 210.28 | 226.87 | 246.34 | 269.53 |
| 9.50% | 172.18 | 183.53 | 196.50 | 211.46 | 228.92 |

The base-case value is highlighted in bold at 8.0% WACC / 2.5% perpetual growth. **A sensitivity grid is not a statistically derived confidence interval** and should not be interpreted as an expected market-price range.

## Main findings and limitations

1. Home Depot's FY2025 historical operating margin was ~12.7%, below FY2021's ~15.2%; the model's 2026–2030 margin path **assumes a gradual recovery**, rather than proving it will happen.
2. Revenue forecasting does not isolate organic expansion from historical acquisitions. The 53-week FY2024 and acquisitions of SRS Distribution (2024) and GMS (2025) complicate year-over-year comparisons.
3. The base model uses a flat 7% operating working-capital intensity, not a detailed operating-ledger forecast. Inventory, payables, and timing shifts may cause larger actual swings.
4. The 8.0% WACC and 2.5% terminal growth are teaching assumptions, not sourced investment-bank cost-of-capital estimates.
5. FY2025 financial statements are used as the reference base, deliberately excluding later quarter-end changes; this is a **historical-date exercise**, not a real-time stock recommendation.
6. The enterprise-to-equity bridge excludes some lease-related and other adjustments; another properly specified model could give a materially different result.
7. No independent external review, audit assurance, or certification of valuation is implied.

## Reproducibility and quality controls

The workbook `home_depot_financial_model_with_dcf.xlsx` was prepared as the Excel companion deliverable for this PR. Until uploaded to this repository, the **download is available from the project-development conversation**, rather than as an in-repository asset. A formula-readable scenario and valuation summary appear in [valuation-model-specification.md](../models/valuation-model-specification.md).

Calculated crosschecks returned **zero differences** for the base-case value versus the sensitivity grid center, FY2025 EBIT margin reconciliation, cash-flow D&A, capital expenditures, net debt bridge, and source-trace years. Arithmetic controls validate internal consistency, not the economic accuracy of forecasts.

## Source documents

- [The Home Depot FY2025 Form 10-K filed March 18, 2026](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/hd-20260201.htm)
- [Home Depot official SEC FY2025 filing index](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/0001628280-26-019436-index.html)
- [Home Depot Annual Reports — Investor Relations](https://ir.homedepot.com/financial-reports/annual-reports/recent)

**Next:** Before public release, owner interview-readiness review and a concise presentation suitable for an internship portfolio.
