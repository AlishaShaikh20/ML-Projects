# Machine Learning Fundamentals

Hands-on implementations from my AI/ML coursework (Apna College) — one folder per project, each with a working notebook, real results, and a short writeup.

## Progress

| Project | Algorithm(s) | Status |
|---|---|---|
| **Supervised Learning** | | |
| Insurance Cost Prediction | Linear Regression | ✅ |
| Employee Turnover Prediction | Logistic Regression | ✅ |
| Iris Flower Classification | KNN, Naive Bayes, Logistic Regression | ✅ |
| CreditWise Loan Approval | Logistic Regression, KNN, Naive Bayes (compared) | ✅ |
| ShopSmart Purchase Prediction | Decision Tree | ✅ |
| SVM | — | 🔜 |
| Ensemble Methods (Boosting, Voting/Stacking) | NovaGen Lab | 🔜 |
| **Unsupervised Learning** | | |
| SmartCart Customer Segmentation | K-Means, Agglomerative Clustering | ✅ |
| Thyroid Anomaly Detection | Isolation Forest, Local Outlier Factor | ✅ |
| **Deep Learning — ANN** | | |
| Date Fruit Classification | ANN | ✅ |
| Power Plant Energy Output Prediction | ANN (Regression) | ✅ |
| **Deep Learning — CNN** | | |
| CIFAR-10 Image Classification | CNN | ✅ |
| **Deep Learning — RNN** | | |
| IMDB Sentiment Analysis | RNN | ✅ |
| **GenAI** | | |
| Transformers, RAG, GenAI | — | 🔜 |

*Updated as each project is finished and pushed.*

---

## Projects

### Supervised Learning

**Insurance Cost Prediction** — Linear Regression predicting medical insurance charges. R² 0.78.

**Employee Turnover Prediction** — Logistic Regression with L1/L2 comparison. Best accuracy ~87% (L1).

**Iris Flower Classification** — KNN, Naive Bayes, and Logistic Regression compared side by side. All hit perfect scores (expected given the dataset).

**CreditWise Loan Approval** — Compared Logistic Regression, Naive Bayes, and KNN on loan approval data. Logistic Regression performed best (F1: 0.79).

**ShopSmart Purchase Prediction** — Decision Tree predicting purchase likelihood from visitor sessions. F1: 0.634, beating the 0.55 benchmark.

### Unsupervised Learning

**SmartCart Customer Segmentation** — K-Means and Agglomerative clustering identifying 4 distinct customer segments (from Moderate Value to Loyal Premium) from spending and engagement data, using PCA and Silhouette Score for evaluation.

**Thyroid Anomaly Detection** — Compared Isolation Forest and Local Outlier Factor to flag anomalous patient records in thyroid health data, purely from data patterns with no labels used during training.

### Deep Learning — ANN

**Date Fruit Classification** — ANN classifying 7 varieties of date fruit from 34 physical features. Test accuracy: 95.0%.

**Power Plant Energy Output Prediction** — ANN regression predicting power plant energy output from environmental conditions. R² Score: 0.9377.

### Deep Learning — CNN

**CIFAR-10 Image Classification** — CNN classifying images into 10 categories using 3 convolutional blocks. Test accuracy: 74.71%.

### Deep Learning — RNN

**IMDB Sentiment Analysis** — RNN classifying movie reviews as positive/negative using TF-IDF features. Test accuracy: 82.85%.

---

## Tech Stack

Python · PyTorch · Scikit-learn · Pandas · NumPy · Matplotlib · Seaborn
