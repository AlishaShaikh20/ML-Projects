# Machine Learning Fundamentals

Hands-on implementations from my AI/ML coursework — one folder per algorithm, each with a working notebook and a real dataset/problem to solve, not just toy examples.

> My main, fully deployed end-to-end projects (Cold Outreach Agent, Technical Onboarding Assistant, and others) live in separate repositories — this repo is specifically my algorithm-by-algorithm learning record.

---

## Progress

| Algorithm | Project | Status |
|---|---|---|
| Linear Regression | House Price Prediction | ✅ |
| Logistic Regression | Employee Turnover | ✅ |
| K-Nearest Neighbors | Iris Flower Classification | ✅ |
| **Supervised algorithms comparison** | **Credit Score & Loan Approval System** | ✅ |
| Decision Trees | ShopSmart — Visitor Purchase Prediction | ✅ |
| SVM | — | 🔜 |
| Gradient Boosting / AdaBoost / Ensembles | NovaGen Lab | 🔜 |
| Unsupervised Learning (Clustering, DBSCAN) | Smart Clustering System | 🔜 |
| Deep Learning (ANN, CNN, RNN) | — | 🔜 |
| Transformers, RAG, GenAI | — | 🔜 |

*Updated as each folder is finished and pushed — this table is the source of truth for what's actually done, not a course syllabus.*

---

## 1. Linear Regression — House Price Prediction
Predicts house prices from features like size, location, and number of rooms using linear regression.

## 2. Logistic Regression — Employee Turnover
Classifies whether an employee is likely to leave the company, based on workplace and demographic factors.

## 3. K-Nearest Neighbors — Iris Flower Classification
Classifies flower species from petal/sepal measurements — the classic KNN benchmark dataset.

## 4. Credit Score & Loan Approval System
Ran the full set of supervised algorithms (logistic regression, decision trees, SVM, KNN, etc.) on the same loan-approval dataset to directly compare performance. **Logistic regression gave the best results.**

## 5. Decision Trees — ShopSmart (Visitor Purchase Prediction)
Predicts whether an e-commerce visitor session will result in a purchase, using browsing behavior across 12,330 sessions. Evaluated using F1 score (not accuracy) due to class imbalance — see the project's own README for the full reasoning.

---

## Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Matplotlib`

---

## Notes

This repo will keep growing as I work through the rest of the course (SVM, ensemble methods, unsupervised learning, deep learning, and RAG/GenAI). Each new folder gets pushed once it's actually done and understood, not just started.
