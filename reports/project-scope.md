# Project Scope and Research Design

**Author:** Shahriar Molhem · University of Georgia · Undergraduate Finance Portfolio  
**Phase:** PR 1 — Foundation · **Created:** October 18, 2026

## Objective
Examine how Home Depot's financial performance developed during fiscal years 2021 through 2025, distinguish operating changes from accounting and capital-allocation effects, and estimate illustrative equity value using documented assumptions.

## Core questions
1. How quickly did reported revenue change, and did margins expand or contract?
2. What happened to inventory, receivables and payables relative to sales and cost of sales?
3. How effectively did operating profit convert into operating cash flow and free cash flow?
4. What changed in financial leverage and shareholder equity, and how might repurchases distort return-on-equity comparisons?
5. How sensitive is an illustrative DCF estimate to operating assumptions, the discount rate, and terminal growth?

## Analytical boundaries
- **Historical period:** FY2021–FY2025. Home Depot fiscal-year labels are used, not calendar-year labels.
- **Source hierarchy:** SEC annual reports/Form 10-K first; issuer earnings releases and IR documents for supplementary context.
- **Currency:** USD millions unless otherwise indicated; keep raw figures unrounded in the model.
- **Reporting basis:** U.S. GAAP. Reconcile or explain any non-GAAP measure separately.
- **Forecasting:** Educational, assumption-driven scenarios. No access to management's internal forecast or budgets.
- **Not in scope:** Audit assurance, certified valuation, stock recommendation, unexplained peer price targets, or claims based on unpublished records.

## Historical model tabs (planned)
1. **Sources & Notes:** filing year, URL, statement, section/page, units, labels, extraction notes.
2. **Raw Reported Data:** exactly as reported, with no hardcoded derived ratios.
3. **Normalized Historical:** consistent signs and units, reconciliation notes.
4. **Ratio Analysis:** formulas only for derived metrics.
5. **Cash Flow & Capital Allocation:** OCF, capex, FCF, dividends, repurchases, debt context.
6. **Forecast & DCF:** visibly separated historical facts and analyst assumptions.
7. **Sensitivity & Checks:** scenario table and validation flags.
8. **Charts:** interpretable, labeled trends tied to modeled values.

## Planned output reports
- `reports/financial-performance.md`: evidence-based analysis of trends.
- `reports/valuation-and-scenarios.md`: assumptions, estimates, sensitivity and limitations.
- `reports/executive-summary.md`: hiring-manager-friendly concise insights.
- `presentations/home-depot-financial-analysis.pptx`: slide deck with speaker-friendly structure.

## Explicit comparability questions
- **Fiscal 2024 contains 53 weeks**, while the adjacent fiscal-year comparisons may have 52 weeks; raw sales growth must be contextualized and, where possible, complemented with reported comparable sales.
- Changes in acquisition scope (including **SRS Distribution**) may affect growth and balance-sheet comparisons; document relevant dates and disclosures from the filings before attributing effects.
- ROE can become misleading when accumulated buybacks affect book equity. Do not interpret extreme ROE without discussing the denominator.
- Use consistent acquisition and debt treatment in enterprise-value and DCF calculations, and do not label a simplified valuation as definitive.

## Completion criteria
The project is publishable only when (1) every key reported figure has a source trail, (2) all statements and derived calculations pass automated/manual checks, (3) judgmental assumptions are visible and defendable, (4) every public-facing conclusion matches the workbook, and (5) the owner has reviewed the materials sufficiently to discuss them in an internship interview.
