# Cancer Demographics: Impact of Demographics on Cancer Mortality
  
**Data Source**: [Kaggle - Cancer Regression Dataset](https://www.kaggle.com/datasets/varunraskar/cancer-regression)

## Project Overview

This project explores how demographic and socioeconomic factors affect cancer mortality across U.S. regions.

It consists of two main parts:
1. **EDA** – Exploratory Data Analysis
2. **REG** – Regression Modeling

---

## EDA Highlights

- Cleaned and merged datasets (`cancer_reg.csv` + household size)
- Handled missing values and outliers (e.g. extreme median age)
- Used correlation analysis and visualizations to identify key relationships
- Key correlations:
  - Higher death rate ↔ lower income, higher poverty, less education
  - Strong links with insurance type and employment status
- Created geospatial visualizations by U.S. states

---

## Regression Modeling

**Goal**: Predict `deathrate` using selected demographic features

### Methods Used:
- Linear, Ridge, Lasso, ElasticNet
- Polynomial Regression (degree 2)
- Feature selection: hypothesis-based, greedy, LASSO, SelectKBest

### Best Model:
- **Polynomial Regression with ElasticNet**
  - R² ≈ 0.56
  - Captures non-linear relationships and handles multicollinearity

---

## Conclusions

- Cancer mortality is influenced by income, education, employment, and insurance access
- ElasticNet with polynomial features achieved the best results
- Simpler linear models are easier to interpret but less accurate

---

## Tools

- Python (pandas, sklearn, seaborn, matplotlib, geopandas)
- Jupyter Notebook

