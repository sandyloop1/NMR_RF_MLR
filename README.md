# Neonatal Mortality Rate Analysis in India
### Predictive Modelling using Random Forest and Multiple Linear Regression (NFHS-5)

---

## Overview

This project analyses **neonatal mortality rates (NMR) across Indian states and districts** using data from the National Family Health Survey (NFHS-5, 2019–21) — India's largest nationally representative household health survey covering 636,699 households.

Two predictive modelling approaches are compared:
- **Random Forest (RF)** — a machine learning ensemble method for identifying non-linear predictors of neonatal mortality
- **Multiple Linear Regression (MLR)** — for interpretable, linear association analysis

The goal is to identify the most significant socioeconomic, maternal, and health system predictors of neonatal mortality to inform public health policy and intervention targeting.

---

## Key Questions

- Which maternal, nutritional, and health system factors best predict neonatal mortality at the state/district level?
- How does a machine learning approach (Random Forest) compare to classical regression (MLR) in predictive accuracy?
- Which variables contribute most to explaining variation in NMR across India?

---

## Dataset

- **Source:** NFHS-5 Factsheets (2019–21), Ministry of Health & Family Welfare, Government of India
- **Coverage:** All Indian states and UTs
- **Key variables include:** institutional delivery rates, antenatal care coverage, skilled birth attendance, maternal anaemia, child stunting, open defecation, female literacy, household wealth index

---

## Methods

### Exploratory Data Analysis
- Correlation matrix and heatmaps
- Distribution analysis of NMR across states
- Feature selection based on collinearity checks

### Random Forest
- Hyperparameter tuning via cross-validation
- Variable importance plot (top 10 predictors)
- Out-of-bag error estimation

### Multiple Linear Regression
- Stepwise variable selection
- Residual diagnostics
- Model comparison (R², RMSE)

---

## Key Finding

The Random Forest model identified **institutional delivery rate, skilled birth attendance, and maternal anaemia** as the top three predictors of neonatal mortality — consistent with global evidence but with state-level granularity relevant to Indian health planning.

---

## Files

| File | Description |
|------|-------------|
| `Exploratory Data_Analysis_14th_JULY_2025.Rmd` | Full R Markdown source code |
| `Exploratory Data analysis_Knitted_RF_MLR(FINAL).html` | Rendered HTML report with outputs |
| `NFHS_5_Factsheets_Data.csv` | Cleaned dataset used for analysis |
| `RF_Top 10_variable_importance.png` | Variable importance plot from Random Forest |

---

## Tools & Libraries

- **Language:** R (RStudio)
- **Key packages:** randomForest, caret, ggplot2, dplyr, corrplot, knitr

---

## Author

**Dr. Sandeep Praharsha Thullimalli**
MBBS | MSc Global Health (University of Glasgow)
Health Coordinator, LASI Wave-2 — IIPS, Mumbai
Principal Investigator, SORT IT Childhood TB Operational Research (WHO/MSF/The Union)

LinkedIn: linkedin.com/in/sandeep-praharsha-thullimalli-aa4528b6
