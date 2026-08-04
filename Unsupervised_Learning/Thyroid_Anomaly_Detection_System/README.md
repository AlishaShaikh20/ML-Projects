## Thyroid Anomaly Detection System

## Overview
Detects unusual patient records in thyroid health data using unsupervised anomaly detection — aimed at flagging rare conditions, data quality issues, or patients who need further clinical investigation, without relying on labels during training.

## Problem Statement
Thyroid disorders require early identification for effective treatment, but large medical datasets often contain unusual records that are hard to spot manually. This project applies unsupervised learning to detect anomalous thyroid patient records purely from patterns in the data, with the true labels used only for post-hoc evaluation.

## Features Used
Demographic attributes, Medical history indicators, Thyroid-related laboratory measurements, Treatment-related information (`Outlier_label` used only for evaluation, not training)

## Models Compared
- Isolation Forest
- Local Outlier Factor (LOF)

## Results
The project compares Isolation Forest and Local Outlier Factor for identifying anomalous patient records within the thyroid dataset.

| Algorithm | Approach |
|---|---|
| Isolation Forest | Isolates points via random partitioning — anomalies require fewer splits to isolate |
| Local Outlier Factor | Flags points in regions of significantly lower local density than their neighbors |

PCA-based visualizations were used to inspect the distribution of normal vs. anomalous observations, helping compare how each algorithm separates outliers from the main patient population.

## Techniques Used
Data loading & exploration, feature selection, feature scaling (StandardScaler), Isolation Forest, Local Outlier Factor, Principal Component Analysis (PCA), anomaly visualization, result comparison

## Tech Stack
Python · Pandas · NumPy · Matplotlib · Scikit-learn

## Future Improvements
- Ensemble anomaly scoring across multiple detectors
- Threshold tuning based on clinical cost of false negatives
- Deployment as a flagging tool for clinical review workflows
