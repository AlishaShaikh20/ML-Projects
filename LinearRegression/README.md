# Linear Regression — Insurance Cost Prediction

## Overview
Predicts medical insurance charges using Linear Regression, based on demographic and health-related features.

## Dataset
[Medical Insurance Cost Dataset](https://www.kaggle.com/datasets/mosapabdelghany/medical-insurance-cost-dataset) — includes age, sex, BMI, number of children, smoking status, and region. Target variable: `charges` (medical insurance cost).

## Steps
- Data preprocessing (encoding categorical features)
- Train-test split
- Model training using Linear Regression
- Model evaluation using MSE and R² score

## Results
- **R² Score:** 0.78
- **MSE:** 33,596,916
- **RMSE:** ~5,800

## Key Learnings
- One-hot encoding vs. label encoding, and when to use each
- Understanding model performance metrics (MSE, RMSE, R²) and what they actually represent
- Effect of feature scaling and target scale on interpretation

## Notes / Limitations
R² of 0.78 leaves some variance unexplained — likely due to `charges` having a long right tail (a small number of high-cost outliers, often smokers with additional health complications). A log-transform on the target or a non-linear model could likely improve on this baseline.
