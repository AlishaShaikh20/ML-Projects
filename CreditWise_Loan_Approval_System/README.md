# CreditWise Loan Approval System

## Overview
Predicts whether a loan application should be approved or rejected based on applicant financial and personal information — aimed at reducing manual verification time and improving consistency in loan decisions.

## Problem Statement
Traditional loan approval relies on manual verification of income, employment, and credit history — slow, inconsistent, and prone to bias. This project builds a predictive model to automate that decision using ML.

## Features Used
Applicant/Coapplicant Income, Employment Status, Age, Marital Status, Dependents, Credit Score, Existing Loans, DTI Ratio, Savings, Collateral Value, Loan Amount, Loan Term, Loan Purpose, Property Area, Education Level, Gender, Employer Category

## Models Compared
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Naive Bayes

## Results
| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| Logistic Regression | 0.870 | 0.778 | 0.803 | 0.790 |
| Naive Bayes | 0.865 | 0.804 | 0.738 | 0.769 |
| KNN | 0.765 | 0.630 | 0.557 | 0.591 |

**Logistic Regression performed best overall**, with the highest accuracy and F1 score. KNN lagged noticeably behind both, likely due to sensitivity to feature scaling and the higher-dimensional feature set (18 features) — distance-based methods like KNN tend to degrade more in higher dimensions compared to linear or probabilistic models.

## Techniques Used
Data cleaning, label encoding, feature engineering, feature scaling, train-test split, correlation heatmap, model evaluation

## Tech Stack
`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Scikit-learn`

## Future Improvements
- Flask web app for real-time predictions
- Model deployment
- Database integration
