# Logistic Regression — Employee Turnover Prediction

## Overview

This project builds a Logistic Regression model to predict employee turnover — whether an employee is likely to leave the company — based on workplace and demographic factors. The goal is to help identify at-risk employees early, so retention efforts can be targeted rather than applied broadly.

## Dataset

**Features used:**
- Age
- Salary
- Experience
- Job Satisfaction
- Performance Rating

**Target variable:** whether the employee left the company (binary classification).

> Dataset and problem statement were provided as part of the Apna College AI/ML course and are not included in this repository, as that material belongs to the course.

## Methodology

1. **Data preprocessing** — cleaning the dataset and preparing features for modeling
2. **Train-test split** — separating data to evaluate the model on unseen samples
3. **Model training** — Logistic Regression as the baseline classifier
4. **Regularization comparison** — trained with both L1 (Lasso) and L2 (Ridge) regularization to compare their effect on performance
5. **Model evaluation** — assessed using accuracy and a classification report

## Results

| Model Variant | Accuracy |
|---|---|
| Baseline Logistic Regression | ~85.9% |
| L1 (Lasso) Regularization | ~87.0% |

L1 regularization slightly outperformed the baseline, likely due to its feature-selection effect — shrinking less useful feature coefficients toward zero and reducing overfitting.

**Planned improvement:** since employee turnover datasets are often imbalanced (far more employees stay than leave), accuracy alone can be a misleading metric — a model could score well simply by predicting "stays" most of the time. Future iterations should report precision, recall, and F1 score specifically for the "left" class to get a more reliable measure of how well the model identifies actual turnover cases.

## Key Learnings

- How Logistic Regression works internally, including the role of the sigmoid function in producing probability outputs
- The difference between L1 (Lasso) and L2 (Ridge) regularization, and their respective effects on model coefficients and overfitting
- The importance of the regularization strength parameter (`C`) in controlling model complexity
- How to interpret a classification report beyond just accuracy

## Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Matplotlib`
