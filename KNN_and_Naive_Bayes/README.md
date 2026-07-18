# KNN, Naive Bayes & Logistic Regression — Iris Flower Classification

## Overview
Implements and compares three classifiers — KNN, Gaussian Naive Bayes, and Logistic Regression — on the Iris dataset, to see how each performs on the same classification task.

## Dataset
**Iris Flower Dataset** — Sepal/Petal length & width as features, flower species as target (3 classes).

## Steps
1. Data preprocessing + label encoding
2. Train-test split
3. Trained Logistic Regression, KNN, and Gaussian Naive Bayes
4. Evaluated via accuracy, confusion matrix, and classification report

## Results
| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| Logistic Regression | 1.00 | 1.00 | 1.00 | 1.00 |
| KNN | 1.00 | 1.00 | 1.00 | 1.00 |
| Gaussian Naive Bayes | 1.00 | 1.00 | 1.00 | 1.00 |

> All three hit perfect scores — expected, since Iris is small and near-perfectly separable, not evidence these models are flawless in general.

## Key Learnings
- End-to-end classification workflow (preprocess → encode → split → train → evaluate)
- How KNN, Naive Bayes, and Logistic Regression differ in approach
- Reading a confusion matrix and classification report
- Why a dataset's separability affects how meaningful accuracy actually is

## Tech Stack
`Python` · `Pandas` · `Scikit-learn` · `Jupyter Notebook`

