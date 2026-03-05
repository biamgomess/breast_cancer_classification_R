# Breast Cancer Wisconsin (Diagnostic) — Data Analysis & Decision Tree (R)

This repository contains a **reproducible data analysis** on the *Breast Cancer Wisconsin (Diagnostic)* dataset, focusing on:
- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- A baseline **Decision Tree** classifier
- Model evaluation (confusion matrix, accuracy, sensitivity/specificity, ROC-AUC)

> Goal: show end-to-end data analysis skills (cleaning → exploration → modeling → evaluation) with clear visuals and documented reasoning.

## Project structure
- `data.csv` — dataset (569 rows, 33 columns; includes an empty `Unnamed: 32` column that is removed in the pipeline)
- `report.qmd` — main Quarto report (R) with EDA + model
- `README.md` — project overview
- `styles.css` — typography (Times) for the HTML report

## How to run locally 
You can reproduce everything with R (≥ 4.2).

Suggested packages:
- `tidyverse`, `janitor`
- `caret`
- `rpart`, `rpart.plot`
- `pROC`, `yardstick`, `rsample`

## Notes
- The dataset uses `diagnosis` with values:
  - `M` = malignant
  - `B` = benign
- This project is intentionally “baseline-first”: the tree model is a starting point. Next steps could include:
  - Logistic regression, Random Forest / XGBoost
  - Cross-validation and tuning
  - Feature engineering and calibration
