# DCF Model Specification — Reproduction Guide

**Scope:** FCFF DCF valuation based on Home Depot FY2025 public filings, with author-generated forecasts.  
**Units:** USD millions; shares in millions; prices in USD/share.

## Data provenance
- [FY2025 reported figures](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/hd-20260201.htm), consolidated balance sheets, consolidated earnings and cash flows.
- Historical CSV: [FY2021–FY2025](../data/historical-financials.csv).
- Methodology overview: [methodology](../reports/methodology.md).

## Actual inputs at FY2025 end

```text
sales = 164683
ebit = 20890
da_from_cash_flow_statement = 4121
cash_capex = 3679
operating_nwc = 11427
short_term_borrowings = 4464
current_lt_debt = 4967
noncurrent_lt_debt = 46341
cash = 1389
year_end_shares_m = 996

net_financial_debt = 4464 + 4967 + 46341 - 1389 = 54383
```

## Operating NWC treatment

The baseline is **$11,427m**, obtained from FY2025 operating current assets (receivables, inventory, other current assets) minus operating current liabilities (accounts payable, accrued salaries/expenses, sales taxes payable, deferred revenue, income taxes payable, other accrued expenses), **excluding cash and financial debt**. Amounts are reported in the 10-K. This simplified NWC treatment should not be confused with `total current assets - total current liabilities`.

The forecast assumptions use **7% of sales** in projected years; the initial `ΔNWC` is the forecast FY2026 NWC minus the actual FY2025 NWC baseline.

## Base scenario assumptions

- Sales growth: `[0.03, 0.032, 0.032, 0.03, 0.028]`
- Operating margins: `[0.129, 0.13, 0.132, 0.133, 0.134]`
- Cash tax rate: `0.24`
- Cash-flow statement D&A / sales: `0.025`
- Capex / sales: `0.023`
- Operating NWC / sales: `0.07`
- WACC: `0.08`
- Perpetual growth: `0.025`
- Shares: `996` (FY2025 **year-end** shares, not average diluted shares)

## DCF formulas
```text
Sales_t = Sales_{t-1} * (1 + Growth_t)
EBIT_t = Sales_t * Margin_t
NOPAT_t = EBIT_t * (1 - Tax_t)
D&A_t = Sales_t * D&A_Ratio_t
Capex_t = Sales_t * Capex_Ratio_t
NWC_t = Sales_t * NWC_Ratio_t
FCFF_t = NOPAT_t + D&A_t - Capex_t - (NWC_t - NWC_{t-1})

PV_forecast = Σ FCFF_t/(1 + WACC)^t
Terminal_value = FCFF_5*(1+g)/(WACC-g)
PV_terminal = Terminal_value/(1+WACC)^5
EV = PV_forecast + PV_terminal
Equity_value = EV - Net_debt
Per_share = Equity_value / 996
```

## Base-case recomputation targets

| Output | Model result |
| --- | ---: |
| Forecast period PV ($m) | 71,552.38 |
| Discounted terminal ($m) | 247,305.96 |
| Enterprise value ($m) | 318,858.34 |
| Net financial debt ($m) | 54,383 |
| Equity value ($m) | 264,475.34 |
| Shares outstanding (millions) | 996 |
| Per-share value ($) | 265.5375 |

**Note:** The historical model's FY2025 cash-flow D&A includes depreciation plus amortization and was linked in the workbook, rather than using the separate income-statement expense subtotal.

## Sensitivity method
Hold the projected FCFF stream fixed; separately vary WACC over **6.50%–9.50%** and perpetual terminal growth over **1.5%–3.5%**. Recalculate the five-year FCFF present values at **each** WACC, the terminal value at **each** WACC and g, and the equity bridge using the same reported FY2025 net financial debt and year-end share count.

## Excel workbook
The companion workbook prepared for this PR includes:
- `START HERE`
- `SOURCE DATA`
- `RATIO ANALYSIS`
- `VALIDATION`
- `SOURCE TRACE`
- `CHARTS`
- `DCF ASSUMPTIONS`
- `DCF MODEL`
- `SENSITIVITY`
- `DCF CHECKS`

**Attachment pending:** The workbook has been created and locally checked, but has not yet been attached as a binary GitHub repository file. This Markdown document is a transparent reconstruction specification, **not a replacement for the Excel file**.

## Modeling risk
The current model is an educational, simplified DCF. It does not separately model future M&A, leases, market-based WACC components, or share issuance/repurchases. Its purpose is to demonstrate a coherent and explicit analytical process, **not to claim certified intrinsic value**.
