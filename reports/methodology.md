# Proposed Analysis Methodology

**Status:** Design only; no financial results or valuation have been calculated.

## 1. Historical performance
Calculate each metric using source-traced reported line items.

| Metric | Definition | Interpretation / guardrail |
| --- | --- | --- |
| Revenue growth | `Sales_t / Sales_(t-1) - 1` | Compare 53-week FY2024 separately and review same-store sales |
| Gross margin | `(Sales - Cost of Sales) / Sales` | Product mix and cost pressures, not evidence of causation by itself |
| Operating margin | `Operating Income / Sales` | Note significant acquisition-related effects |
| Net margin | `Net Income / Sales` | Interest, tax, and other below-operating effects |
| Current ratio | `Current Assets / Current Liabilities` | Interpret with seasonal retail working capital |
| Inventory turnover | `Cost of Sales / Average Inventory` | Use beginning/ending balance; period consistency |
| Operating cash conversion | `Operating Cash Flow / Net Income` | May be unstable in one year; interpret trends |
| Free cash flow (simple) | `Operating Cash Flow - Capital Expenditures` | Explicitly a simplified FCF definition |
| Debt to equity | `Total Interest-Bearing Debt / Book Equity` | Caution if equity is unusually low |
| ROA | `Net Income / Average Total Assets` | Average balances and acquisition effects |
| ROIC (educational) | `NOPAT / Average Invested Capital` | State exact invested-capital definition; may differ from issuer's adjusted ROIC |

> Measures with average denominators may require opening FY2020 balances for FY2021. Acquire source values or mark unavailable; never invent opening balances.

## 2. Disclosures and comparability
- Distinguish **as reported** growth from organic/comparable-sales changes where appropriate.
- FY2024 had **53 weeks**, so its reported revenue is not directly comparable on a 52-week basis without a clear adjustment.
- Read acquisition and capital allocation notes before attributing year-to-year balance-sheet changes.
- Clearly distinguish GAAP metrics from issuer-provided adjusted or non-GAAP measures.
- Avoid treating accounting correlation as operational cause without management discussion or additional evidence.

## 3. Valuation exercise (future stage)
Use a basic **FCFF discounted cash flow** model with explicit, documented assumptions:
- `EBIT * (1 - Tax Rate) = NOPAT`
- `FCFF = NOPAT + D&A - Capex - Change in Operating NWC`
- `Enterprise Value = PV(Projection-period FCFF) + PV(Terminal Value)`
- `Equity Value = Enterprise Value - Net Debt +/- Other Nonoperating Adjustments`
- `Value Per Share = Equity Value / Diluted Shares (consistent timing/basis)`

Use a justified discount rate and terminal assumptions; present scenario sensitivities for WACC and terminal growth. Check that terminal growth is less than WACC in perpetuity-based terminal value. Report a range rather than implying false precision. No market price comparison until a dated source is documented.

## 4. Numeric QA
- Check `Assets = Liabilities + Equity` within filing-rounding tolerance.
- Check `Operating Cash Flow + Investing Cash Flow + Financing Cash Flow + FX adjustments = Change in Cash` according to statement presentation.
- Confirm that derived gross profit/operating income aligns with disclosed totals and presentation.
- Confirm historical Excel formulas reference model cells instead of typed output values.
- Confirm DCF terminal value and present value formulas are internally consistent.
- Ensure markdown reports, tables, charts and slides pull from the verified model, not independently typed approximations.

## 5. Communication standard
Write at a **BBA Finance student** level: evidence, calculation, interpretation, limits. The output is research for internship portfolio review, not an audit opinion, a certified appraisal, or personal investment advice.
