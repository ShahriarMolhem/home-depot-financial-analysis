# Historical Financial Performance — The Home Depot, FY2021–FY2025

**Independent BBA Finance student analysis** · Shahriar Molhem, University of Georgia  
**Historical period:** FY2021–FY2025 · **Units:** USD millions except per-share data.  
**Status:** Historical analysis only. A forward-looking DCF is **not** yet complete; this is not an investment recommendation.

## Executive observations

Home Depot reported **$164.683 billion** of FY2025 net sales versus **$151.157 billion** in FY2021, an **8.9% cumulative increase**. Operating income moved in the opposite direction, declining from **$23.040 billion** to **$20.890 billion** (**9.3% below** FY2021). Operating margin consequently declined from **15.2%** to **12.7%**. Those reported changes establish a margin compression pattern; they do not establish a single causal explanation.

Operating cash flow in FY2025 was **$16.325 billion**, versus **$19.810 billion** in FY2024, a **17.6% decrease**. Simplified free cash flow (operating cash flow less capital expenditures) was **$12.646 billion** in FY2025 versus **$16.325 billion** a year earlier. This measure differs from unlevered FCFF used in valuation.

## Historical performance dashboard

| USD millions except ratios | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Net sales | 151,157 | 157,403 | 152,669 | 159,514 | 164,683 |
| Gross profit | 50,832 | 52,778 | 50,960 | 53,308 | 54,865 |
| Operating income | 23,040 | 24,039 | 21,689 | 21,526 | 20,890 |
| Net income | 16,433 | 17,105 | 15,143 | 14,806 | 14,156 |
| Operating margin | 15.2% | 15.3% | 14.2% | 13.5% | 12.7% |
| Net margin | 10.9% | 10.9% | 9.9% | 9.3% | 8.6% |
| Operating cash flow | 16,571 | 14,615 | 21,172 | 19,810 | 16,325 |
| Capex (cash outflow, absolute) | 2,566 | 3,119 | 3,226 | 3,485 | 3,679 |
| Simplified FCF | 14,005 | 11,496 | 17,946 | 16,325 | 12,646 |
| Inventory | 22,068 | 24,886 | 20,976 | 23,451 | 25,817 |
| Cash | 2,343 | 2,757 | 3,760 | 1,659 | 1,389 |

## Reading the results

**Revenue versus operating profit.** Revenue was higher at the end of the series, but profitability did not track that increase. SG&A represented about **16.8% of sales in FY2021** and **18.6% in FY2025**; this proportional shift is consistent with operating-margin pressure. Because the company has changed its business mix and acquisition footprint, it would be inaccurate to attribute the difference to one operating driver without evaluating management's disclosures and the effects of acquisitions.

**Cash generation.** Capital expenditures increased from **$2.566 billion (FY2021)** to **$3.679 billion (FY2025)**. FY2025 operating cash flow was 17.6% below FY2024; the simplified FCF measure therefore fell 22.5%. Cash flow can vary with inventory, supplier payment timing, taxation, and other balance-sheet movements, so one year should not be extrapolated as a permanent trend.

**Balance-sheet context.** Assets rose from **$71.876 billion** in FY2021 to **$105.095 billion** in FY2025. Shareholder equity was **negative in FY2021**; a simple ROE comparison would produce an economically misleading figure for that year. The future ratio analysis should consider inventory efficiency and leverage alongside disclosed acquisitions rather than labeling every increase in assets organic expansion.

## Comparability and accounting caveats

1. FY2024 included **53 weeks**, whereas adjacent fiscal years generally included 52; the 2024 reported-sales base has an extra week.
2. The **SRS Distribution acquisition** in FY2024 and **GMS acquisition** in FY2025 affect consolidated reporting and make unadjusted multi-year growth an imperfect proxy for organic growth.
3. The simplified FCF calculation (`OCF - capex`) is **not** equivalent to FCFF in a DCF analysis.
4. Actual ratio formulas and source values are available in `data/historical-financials.csv`; in the companion Excel model ratios are calculated from linked cells.
5. This report reflects a **student's independent analysis** of published filings, not audit assurance or a certified valuation.

## Data validation performed

The workbook's **VALIDATION** sheet checks, year by year, gross profit; operating profit; pretax earnings; net earnings; assets = liabilities + equity; sum of disclosed current asset categories; operating + investing + financing cash flows; beginning-to-ending cash movements including FX; and ending cash against balance-sheet cash. All recorded differences in the initial pass equal **zero** for FY2021–FY2025.

## Primary sources

- [FY2025 Form 10-K, Consolidated Statements of Earnings, Balance Sheets and Cash Flows](https://www.sec.gov/Archives/edgar/data/354950/000162828026019436/hd-20260201.htm)
- [FY2023 Form 10-K, FY2021–FY2023 historical earnings and cash flows](https://www.sec.gov/Archives/edgar/data/354950/000035495024000062/hd-20240128.htm)
- [FY2022 Form 10-K, early balance sheets](https://www.sec.gov/Archives/edgar/data/354950/000035495023000059/hd-20230129.htm)

**Next:** Source-trace review, acquisition and same-store-sales discussion, then a separately identified assumption-driven valuation exercise in PR3.
