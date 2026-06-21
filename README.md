# Telecom Customer Churn — Data Analytics & Machine Learning

End-to-end Python analysis of customer behaviour and churn drivers in the telecommunications sector, translating analytical findings into actionable retention insights.

## Context

MSc in Statistics & Data Science, University College Dublin. End-to-end project combining exploratory analysis, statistical testing, supervised learning, and unsupervised segmentation on real-world customer data.

## What it does

The project analyses two contract datasets (monthly and yearly) to understand what drives churn and how customers can be segmented for targeted retention strategies:

1. **Exploratory Analysis** — distribution of churn, tenure, charges and service features across both contract types; statistical comparison of key indicators between monthly and yearly cohorts.
2. **Predictive Modelling** — Logistic Regression baseline followed by a Random Forest classifier; feature importance ranking to identify the strongest churn predictors.
3. **Customer Segmentation** — K-means clustering validated with Spectral Clustering; silhouette analysis identifies k = 2 as the optimal solution in both methods.

## Tech stack

| Layer | Tools |
|---|---|
| Language | Python 3 |
| Data wrangling | `pandas` |
| Visualisation | `matplotlib`, `seaborn` |
| Machine learning | `scikit-learn` (LogisticRegression, RandomForestClassifier, KMeans, SpectralClustering) |
| Notebook | Jupyter |

## Key findings

- **Tenure is the dominant churn predictor** across all methods: customers in their first months are substantially more likely to churn than established customers.
- **Two natural customer segments** emerge consistently from both K-means and Spectral Clustering: a high-tenure / high-value group (low churn) and a short-tenure / low-value group (high churn concentration). The two-cluster solution achieves the highest silhouette score across both algorithms.
- Yearly contract customers show significantly lower churn rates than monthly subscribers, confirming contract type as a structural retention lever.
