## SmartCart Customer Segmentation System

## Overview
Groups SmartCart's e-commerce customers into meaningful segments based on demographics, spending, and engagement — aimed at replacing generic marketing with personalized, data-driven strategies.

## Problem Statement
SmartCart currently applies the same marketing strategy to all customers, regardless of their behaviour. This leads to inefficient campaigns, missed opportunities to retain high-value customers, and difficulty spotting customers at risk of churn. This project uses unsupervised learning to uncover natural customer groupings from purchasing and engagement data.

## Features Used
Income, Recency, Purchase Counts (Web/Catalog/Store), Web Visits, Customer Complaints, Product Spending Categories, Demographics, Household Information

## Models Compared
- K-Means Clustering
- Agglomerative Clustering

## Results
Four customer segments were identified:

| Cluster | Segment | Key Traits |
|---|---|---|
| 0 | Moderate Value Customers | Medium income, moderate spending, average engagement |
| 1 | High Value Customers | High income/spending, frequent catalog & store purchases |
| 2 | Low Spending Customers | Lower spending, high web visits but low conversion |
| 3 | Loyal Premium Customers | High income/spending, highest engagement — most valuable segment |

Cluster 3 (Loyal Premium Customers) stood out as the most valuable segment for retention efforts, while Cluster 2 (Low Spending Customers) represents the strongest opportunity for targeted promotional campaigns.

## Techniques Used
Data cleaning, feature engineering, feature scaling, Principal Component Analysis (PCA), K-Means clustering, Agglomerative clustering, Silhouette Score evaluation, cluster profiling

## Tech Stack
Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn

## Future Improvements
- Interactive dashboard for cluster exploration
- Predictive churn scoring per segment
- Deployment as a customer-insights API
