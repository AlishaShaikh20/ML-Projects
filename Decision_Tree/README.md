# ShopSmart — Visitor Purchase Prediction (Decision Tree)

## Overview
Predicts whether an e-commerce visitor session will result in a purchase, using 12,330 sessions of browsing behavior. Since purchases are a minority class, performance is judged on F1 score, not accuracy.

## Problem Context
ShopSmart wants to identify which visitors are likely to buy, to target marketing more efficiently. The benchmark for a viable model is an **F1 score of 0.55**.

## Techniques Used
- Data preprocessing, OneHotEncoding, StandardScaler
- Built as a Pipeline
- Hyperparameter tuning via GridSearchCV + Cross Validation

## Model
Decision Tree Classifier

## Results
**Best F1 Score: 0.634** — clears the 0.55 benchmark.
**Best Parameters:** `max_depth=4`, `min_samples_leaf=50`

The relatively shallow tree (depth 4) and higher `min_samples_leaf` suggest the model benefits from staying simple here — a deeper tree likely overfits to the imbalanced minority class rather than generalizing.

## Tech Stack
`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Jupyter Notebook`

## Future Improvements
- Random Forest / XGBoost for comparison
- Further feature engineering
- Deployment via Flask or Streamlit
