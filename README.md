# Retail Sales Performance Dashboard

A Power BI dashboard project intended to help retail stakeholders bring sales, product, regional, store, customer, and returns reporting into one analytical view. The portfolio brief identifies four report pages and several approximate displayed metrics, but the source `.pbix`, screenshots, dataset, and calculation definitions were not present in the inspected workspace. This README records the available information without presenting unverified implementation details as fact.

> **Portfolio status:** Documentation is prepared from the project brief. Dashboard screenshots and the report file are not currently included, so the report itself cannot yet be independently reviewed from this repository.

## Table of contents

- [Executive summary](#executive-summary)
- [Business problem](#business-problem)
- [Business objectives](#business-objectives)
- [Project scope](#project-scope)
- [Tools and technologies](#tools-and-technologies)
- [Dataset](#dataset)
- [Preparation and modeling](#data-preparation-and-modeling)
- [KPI definitions](#kpi-definitions)
- [Dashboard pages](#dashboard-architecture-and-pages)
- [Available observations](#available-observations)
- [Business questions](#business-questions)
- [Recommendations](#recommendations)
- [Limitations and assumptions](#limitations-and-assumptions)
- [Viewing the report](#how-to-view-the-power-bi-report)
- [Repository structure](#repository-structure)
- [Skills demonstrated](#skills-demonstrated)
- [Future improvements](#future-improvements)
- [Conclusion](#project-conclusion)
- [Portfolio summary](#portfolio-summary)

## Executive summary

The reported dashboard is organized around executive sales performance, products, regional and store results, and customer and returns analysis. The project brief reports approximately **1.47M total revenue**, **5,710 units sold**, **633 returns**, **180.52K discounts**, a **0.11 return rate**, **29.37K average revenue per store**, and **2.83K average customer spend**. These are values as supplied from the dashboard display; they have not been recalculated against source data.

The report is designed to support monitoring and comparison. No business impact—such as revenue growth, lower returns, cost savings, or improved profitability—has been established by the materials currently available.

## Business problem

Retail performance information can be difficult to interpret when sales, product, geography, store, customer, discount, and return reporting is spread across separate views or dimensions. Stakeholders may lack a consistent way to move from an overall result to the products, locations, or customer groups associated with it.

This dashboard is intended to consolidate those perspectives into a set of report pages and interactive filters. Its purpose is decision support: it can help users explore reported performance, but the available evidence does not establish that it changed business outcomes.

## Business objectives

- Monitor reported revenue and units sold.
- Compare revenue across months.
- Examine product and category contribution.
- Compare performance across regions, cities, and stores.
- Explore customer spending and purchase frequency.
- Review returns and discount metrics together with sales measures.
- Filter results by year, region, product category, store format, and customer attributes where those fields are available in the report.

## Project scope

The described scope is a four-page Power BI report covering executive, product, regional/store, and customer/returns perspectives. The intended analysis spans time, product, geography, store, customer, sales, discounts, and returns.

This repository does not currently contain the report or evidence needed to confirm the data model, visual interactions, filter behavior, ETL process, or calculations. No SQL integration, automated refresh, real-time processing, or deployment is claimed.

## Tools and technologies

| Tool | Evidence and status |
|---|---|
| Microsoft Power BI | Identified as the dashboard platform in the project brief; the `.pbix` file was not found for verification. |
| Git / GitHub | Used to version and publish this documentation repository. |
| SQL, Python, Excel | No project source files establishing their use were found; they are not claimed as implementation tools. |

## Dataset

No dataset attributable to this dashboard was found in the inspected project folders. Accordingly, its source, licensing/provenance, row count, date coverage, schema, grain, and personal or confidential data status cannot be documented or validated here.

The separate Retail Demand Forecasting project in the workspace contains sales-related files, but it is a distinct project and is not represented as this dashboard's data source. No data has been copied from it.

## Data preparation and modeling

The source data, Power Query steps, model relationships, and transformation logic were unavailable. Data cleaning, deduplication, date handling, dimensional modeling, and refresh processes therefore cannot be described as completed or verified. These details should be added from the actual report and source files when available.

## KPI definitions

The following values were supplied as approximate dashboard display values. Their names are retained, but their formulas, units, aggregation rules, and filter behavior cannot be confirmed without the report model and data.

| Displayed metric | Approximate value supplied | Calculation status |
|---|---:|---|
| Total revenue | 1.47M | Definition and currency not verified. |
| Total units sold | 5,710 | Unit and treatment of cancellations/returns not verified. |
| Total returns | 633 | Counting basis (transactions, items, or another unit) not verified. |
| Total discounts | 180.52K | Currency, aggregation, and whether gross or net are not verified. |
| Return rate | 0.11 | Display format and denominator are unclear; do not interpret as 11% until verified. |
| Average revenue per store | 29.37K | Store population, period, and averaging method are unverified. |
| Average customer spend | 2.83K | Customer population, period, and averaging method are unverified. |

These figures should not be compared or combined as if they shared a verified currency, time period, or denominator.

## Dashboard architecture and pages

The page names below come from the project brief. Screenshots and the Power BI report were not available, so these are scope descriptions rather than visual inspections.

1. **Sales Performance | Executive Overview** — intended as the high-level sales monitoring page. The supplied brief associates the overall revenue, units, returns, discounts, return rate, store average, and customer average metrics with the dashboard; exact placement by page is unverified.
2. **Product Performance** — intended to support comparison of products and categories, including identification of higher-revenue contributors. Specific rankings and chart encodings are unavailable.
3. **Regional & Store Performance** — intended to compare results across regional, city, and store dimensions. Specific geographies, store formats, and visual details are unavailable.
4. **Customer & Returns Analytics** — intended to explore customer spending/frequency and returns. Segment definitions and the income-bracket consistency noted for review cannot be checked without the report.

### Screenshots

The four source screenshots were not found in the accessible workspace, so there are no image files to embed yet. Add the verified images under `screenshots/` and link them here when available. No substitute or illustrative screenshots have been created.

## Available observations

Only the approximate headline values above are available, without a dataset, time series, comparison baseline, or screenshot evidence. They are not sufficient to establish trends, outliers, product rankings, regional differences, customer behavior, or operational causes.

The project brief flags several validation questions for review in the actual report:

- Whether monthly revenue is sorted chronologically rather than alphabetically.
- Whether return rate is formatted consistently and uses an appropriate, documented denominator.
- How average customer spend and average revenue per store are defined.
- Whether income bracket categories are consistent.
- Whether chart titles and labels specify clear units and periods.
- Whether revenue, discounts, units, and returns are presented with distinct definitions and compatible units.

These are checks to perform, not confirmed defects.

## Business questions answered

Based on the stated page and filter scope, the report is intended to help users investigate:

- What revenue and unit volume are being reported?
- How does reported revenue vary by month?
- Which products or categories appear to contribute more revenue?
- How do reported results compare by region, city, and store?
- How do spending and purchase frequency vary across customers or supported customer attributes?
- What return and discount values are reported, and how do they vary under available filters?
- How do these views change when filtering by year, region, category, store format, or customer attributes supported by the model?

The report's ability to answer these questions should be confirmed against the `.pbix` file and its underlying data.

## Recommendations

These are suggested next steps for retail management, not measured findings:

- Validate KPI definitions and display formats with finance and operations owners before using them in decisions.
- Review high-revenue products and categories alongside units, discounting, and returns to understand the full commercial picture.
- Compare regional and store performance using consistent time periods and store populations.
- Segment customer spend and purchase frequency only where definitions, sample sizes, and privacy safeguards are clear.
- Investigate return patterns with product, channel, and reason data if those fields are available.
- Test chart sorting, titles, units, and filter interactions with report users.

## Limitations and assumptions

- The `.pbix`, four screenshots, dataset, SQL, DAX, and transformation documentation were not found in the accessible locations searched.
- Page names, filter dimensions, and approximate KPI values are sourced from the project brief, not independently inspected report artifacts.
- KPI formulas, currency, date range, data grain, and refresh state are unknown.
- The supplied values are approximate display values and are not independently recalculated.
- No causal or financial business impact has been measured.
- Proposed recommendations are exploratory and require validation against actual data and business context.

## How to view the Power BI report

The report file is not included because it was not found. To make this project reviewable, add the original `.pbix` after confirming it is safe to share and within repository size constraints. A reviewer with Power BI Desktop can then open the file locally. If the file is too large for standard Git hosting, use Git LFS or a GitHub Release and link it here; do not describe the report as uploaded until that has been done.

## Repository structure

```text
retail-sales-performance-dashboard/
└── README.md
```

Only the README is included at present because no verified dashboard assets or source documentation were available. Directories for screenshots, data, report, or documentation will be added when real project files are supplied.

## Skills demonstrated

This documented project scope is relevant to:

- Business problem framing and stakeholder-oriented reporting.
- KPI interpretation and validation planning.
- Retail sales, product, regional/store, customer, discount, and returns analysis.
- Dashboard communication and analytical documentation.
- Evidence-based recommendations and transparent limitation reporting.

Specific implementation skills such as DAX development, data modeling, SQL analysis, or Power Query transformation should only be listed after the report or source files verify them.

## Future improvements

1. Add the original `.pbix` and four page screenshots.
2. Document dataset provenance, schema, grain, date coverage, and sharing/privacy review.
3. Capture Power Query transformations, model relationships, and verified DAX definitions.
4. Define each KPI, including its units, denominator, period, and treatment of returns/discounts.
5. Validate month sorting, income brackets, visual labels, and filter behavior.
6. Recalculate displayed metrics from source data and document reconciliation checks.
7. Add evidence-based findings with clear time frames and comparison baselines.

## Project conclusion

The stated dashboard scope addresses a practical retail reporting need by bringing several performance dimensions into one intended Power BI experience. The currently available project evidence supports documenting that scope and the approximate values supplied in the brief, but not validating the calculations, visuals, dataset, or business impact. Adding the original report and source materials is necessary for a recruiter to review the analytical implementation and for the findings to be independently reproduced.

## Portfolio summary

**Resume / LinkedIn summary:** Framed a retail performance reporting problem and documented a four-page Power BI dashboard concept spanning executive sales, products, regions/stores, customers, and returns. Recorded supplied headline metrics with explicit validation caveats and outlined KPI, data quality, and reporting checks; implementation details and business impact remain subject to verification against the original report and source data.
