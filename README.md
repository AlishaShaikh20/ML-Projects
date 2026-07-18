# Machine Learning Fundamentals

Hands-on implementations from my AI/ML coursework (Apna College) — one folder per project, each with a working notebook, real results, and a short writeup.

> My main, fully deployed end-to-end projects (Cold Outreach Agent, Technical Onboarding Assistant, and others) live in separate repositories — this repo is specifically my algorithm-by-algorithm learning record.

## Progress

| Project | Algorithm(s) | Status |
|---|---|---|
| Insurance Cost Prediction | Linear Regression | ✅ |
| Employee Turnover Prediction | Logistic Regression | ✅ |
| Iris Flower Classification | KNN, Naive Bayes, Logistic Regression | ✅ |
| CreditWise Loan Approval | Logistic Regression, KNN, Naive Bayes (compared) | ✅ |
| ShopSmart Purchase Prediction | Decision Tree | ✅ |
| SVM | — | 🔜 |
| Ensemble Methods (Boosting, Voting/Stacking) | NovaGen Lab | 🔜 |
| Unsupervised Learning | Clustering, DBSCAN | 🔜 |
| Deep Learning | ANN, CNN, RNN | 🔜 |
| Transformers, RAG, GenAI | — | 🔜 |

*Updated as each project is finished and pushed.*

## Projects

**[Insurance Cost Prediction](./linear-regression)** — Linear Regression predicting medical insurance charges. R² 0.78.

**[Employee Turnover Prediction](./logistic-regression)** — Logistic Regression with L1/L2 comparison. Best accuracy ~87% (L1).

**[Iris Flower Classification](./knn-naive-bayes)** — KNN, Naive Bayes, and Logistic Regression compared side by side. All hit perfect scores (expected given the dataset).

**[CreditWise Loan Approval](./creditwise)** — Compared Logistic Regression, Naive Bayes, and KNN on loan approval data. Logistic Regression performed best (F1: 0.79).

**[ShopSmart Purchase Prediction](./shopsmart)** — Decision Tree predicting purchase likelihood from visitor sessions. F1: 0.634, beating the 0.55 benchmark.

## Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Matplotlib` · `Seaborn`

## Notes

Datasets and problem statements provided by the Apna College AI/ML course are not included in this repo, as that material belongs to the course — each project's README describes the data and problem instead. This repo will keep growing as I work through SVM, ensemble methods, unsupervised learning, deep learning, and RAG/GenAI.
