# Telco Customer Churn Prediction 📉

## Overview
Customer churn is a major challenge for telecom companies.  
This project builds machine learning models to predict whether a customer is likely to churn, allowing businesses to take proactive retention actions.

## Dataset
- Telco Customer Churn dataset (IBM)
- 7,000+ customers
- Binary target: Churn (Yes / No)

## Problem Type
- Binary Classification
- Imbalanced dataset (~26% churn)

## Models Used
- Logistic Regression (with class weighting)
- Random Forest
- Gradient Boosting
- XGBoost

## Evaluation Metrics
Due to class imbalance, accuracy alone is misleading.  
Primary metrics used:
- Recall (Churn)
- F1-score
- ROC-AUC

## Results Summary

| Model | Accuracy | Recall (Churn) | F1-score | ROC-AUC |
|------|---------|----------------|---------|--------|
| Logistic Regression (Balanced) | 0.73 | 0.79 | 0.61 | 0.84 |
| Random Forest | 0.77 | 0.74 | 0.63 | 0.84 |
| Gradient Boosting | 0.80 | 0.53 | 0.58 | 0.84 |
| XGBoost | 0.73 | 0.78 | 0.61 | 0.83 |

## Key Insights
- Customers on month-to-month contracts churn more
- Higher monthly charges increase churn risk
- Long tenure significantly reduces churn probability

## Conclusion
Balanced Logistic Regression and XGBoost performed best in terms of churn recall, making them suitable for churn prevention strategies where missing churn customers is costly.

## Future Improvements
- Threshold tuning to further improve recall
- Cost-sensitive learning
- Model deployment as a REST API

---
