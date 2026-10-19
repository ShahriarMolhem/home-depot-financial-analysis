# Validation Checklist and Release Gates

**Status: foundation created — no model completed**

## Source integrity
- [ ] Each FY2021–FY2025 income-statement input mapped to a filing table/page
- [ ] Balance-sheet and cash-flow historical inputs mapped similarly
- [ ] Fiscal 2024 extra-week comparability disclosed where relevant
- [ ] Significant acquisitions and accounting-policy changes identified
- [ ] Numeric scales (actual dollars vs USD millions) checked consistently
- [ ] Data changes documented; no fabricated source values

## Excel calculation checks
- [ ] Balance sheet identity reconciles for every applicable year
- [ ] Income statement arithmetic reconciles to reported net earnings
- [ ] Cash flow checks reconcile under the filing's presentation
- [ ] Average-balance metrics use appropriate opening/closing balances
- [ ] No hidden hardcoded valuation output replaces a formula
- [ ] Historical data visually distinguished from forecast inputs
- [ ] Ratio labels and chart units match formulas
- [ ] Scenario/sensitivity outputs respond correctly to assumption changes

## Reporting and presentation checks
- [ ] Findings distinguish fact, calculation, assumption and interpretation
- [ ] Key conclusions can be reproduced from the workbook
- [ ] Tables/figures have units, periods and source notes
- [ ] No audit, CPA, or independent expert certification implied
- [ ] No claims of confidential company data
- [ ] README, markdown reports and PowerPoint agree on results
- [ ] Presentation discusses at least three important limitations
- [ ] Portfolio owner reviews the material and prepares a concise interview explanation

## Planned GitHub review stages
1. **PR1 / Foundation:** scope, methodology, sources and this QA plan.
2. **PR2 / Historical model:** extract dataset, model and actual ratios.
3. **PR3 / Financial interpretation & valuation:** document the findings and scenarios; resolve issues.
4. **PR4 / Presentation & release:** publish hiring-ready visuals, presentation, and summary.

**Release gate:** Keep this repository private until the full model and reports are validated and the owner approves publishing.
