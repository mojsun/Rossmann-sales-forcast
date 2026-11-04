# Rossmann Store Sales Forecasting & Retail Analytics

**Academic team project | Master of Management Analytics, Smith School of Business, Queen's University | 2026**

## Project overview

This project examines how a retail chain can use historical sales, store characteristics, calendar information, and promotion schedules to forecast daily store sales. The goal is to support better **inventory, staffing, and promotion planning** through interpretable analytics and an executive-facing dashboard.

## Business problem

Rossmann needs reliable forecasts for individual stores and trading days. A single chain-wide forecast can overlook differences between stores and the varying impact of promotions across weekdays and store formats.

**Key questions:**
- How accurately can we forecast daily sales using information available before the sales day?
- Which factors explain differences in store performance?
- When and where do promotions have the greatest modeled impact?
- How can forecast results inform practical retail decisions?

## Data and methods

- **Scope:** 100 stores and 42,400 store-day observations spanning January 2014 to February 2015.
- **Model:** Ordinary least squares (OLS) regression on log daily sales, incorporating store fixed effects, calendar and holiday controls, promotion variables, and interaction terms.
- **Validation:** Chronological holdout using January–February 2015 as unseen test data.
- **Analysis:** Data preparation, feature engineering, regression modeling, model validation, and interpretation of promotion effects.

## Key results

| Measure | Result |
|---|---:|
| Training R² | 0.8323 |
| Test R² | **0.8293** |
| Test RMSE (log sales) | 0.1851 |
| Test MAE (log sales) | 0.1331 |
| Coverage of 95% prediction intervals | 95.30% |

**Business insights:**
- Adding store-specific baselines improved test R² from approximately **0.28 to 0.81**, demonstrating the importance of differences between stores.
- The modeled uplift from a single-day promotion varied substantially by weekday: approximately **78.7% on Monday** versus **37.4% on Friday** under comparable conditions.
- The results support **store-specific forecasting** and more targeted promotion, inventory, and staffing plans rather than relying on one network-wide assumption.

These are **model-based findings from an academic case study**, not outcomes measured after real-world deployment.

## Project materials

The repository is organized into the following folders:

```text
Rossmann-sales-forcast/
├── Dashboard/   # Executive dashboard files and PDF export
├── Images/      # Screenshots and visualizations
├── Notebooks/   # Jupyter notebook(s) for analysis
├── Reports/     # Project documentation and reports
└── README.md    # Project overview
```

Browse the folders above for the analysis, dashboard, and supporting documentation. The HTML dashboard may be opened locally in a browser; a PDF export provides a static view.

## Skills demonstrated

**Python · Data Cleaning · Exploratory Data Analysis · OLS Regression · Statistical Modeling · Forecasting · Model Validation · Retail Analytics · Data Visualization · Business Communication**

## Project context and acknowledgment

Completed as a **team project** during the Master of Management Analytics program at Queen's University. The analysis and results reflect collaborative academic work. Individual contributions should not be inferred from this summary.

*The analysis uses historical case-study data and is intended to demonstrate analytical and business problem-solving skills.*
