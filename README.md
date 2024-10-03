# Capstone Project: Fraud Detection with Machine Learning
Christopher Tan  
Western Governors University  

## Background and Overview
This project aims to identify fraudulent transactions in bank accounts using machine learning. Four models were evaluated—**Logistic Regression, Random Forest, Neural Networks**, and **XGBoost**—using Kaggle’s **Bank Account Fraud Dataset Suite (NeurIPS 2022)**. The dataset has 1 million records and 32 features, making it suitable for training and testing. The **AUC-ROC** metric was the primary evaluation criterion, and ensemble methods were applied to improve model accuracy.

## Data Structure Overview
The dataset includes:
- **Transaction ID**: Unique identifier.
- **Transaction Amount**: The monetary value of transactions.
- **Date/Time**: Temporal details used for splitting data into training (months 0-5) and testing (months 6-7).
- **Fraud Label**: Binary target variable (1 for fraud, 0 for non-fraud).
  
Data preprocessing included handling missing values and encoding categorical variables with one-hot encoding. Temporal splitting ensured real-world applicability.

## Executive Summary
After extensive data preparation and hyperparameter tuning, the models achieved the following AUC scores:
- **Logistic Regression**: 0.8719
- **Random Forest**: 0.8887
- **Neural Networks**: 0.8793
- **XGBoost**: 0.8897

Ensemble methods like **Simple Averaging** and **Weighted Voting** improved AUC to **0.8945**, demonstrating the potential of combining models to enhance fraud detection accuracy.

## Insights Deep Dive
1. **Model Comparisons**: XGBoost consistently outperformed other models, but Random Forest improved significantly with hyperparameter tuning.
2. **Feature Importance**: Key features driving fraud predictions include **housing status**, **credit risk score**, and **device operating system**.
3. **Ensemble Methods**: Combining models (simple averaging/weighted voting) achieved the highest AUC, showing the value of diverse model aggregation.

This project highlights the strengths of each model and the effectiveness of ensemble methods in improving fraud detection.
