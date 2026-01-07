# Telecom Customer Churn Analysis

## Project Overview
Customer churn is a major challenge in the telecom industry due to high competition and low switching costs. This project analyzes customer demographics, service usage, and billing information to identify key drivers of churn and build a predictive model to estimate churn risk.

## Dataset
The dataset contains customer-level information including:
- Demographics (e.g., gender, senior citizen status)
- Service subscriptions (internet, streaming, security, support)
- Billing and contract details
- Churn status (Yes / No)

Target variable: **Churn**

## Objectives
- Identify factors associated with customer churn
- Build a churn prediction model using logistic regression
- Translate analytical findings into actionable business recommendations

## Methodology
- Exploratory Data Analysis (EDA)
- Data cleaning and feature engineering
- Logistic regression modeling
- Model evaluation using confusion matrix and ROC–AUC
- Business-oriented interpretation of results

## Key Exploratory Insights
- Senior citizens exhibit significantly higher churn rates than non-senior customers
- Fiber optic internet users have the highest churn rates
- Customers without online security, online backup, or tech support churn at much higher rates
- Contract type is a strong churn driver, with month-to-month customers exhibiting the highest churn
- Streaming services have limited impact on churn behavior

## Modeling & Evaluation
A logistic regression model was trained using a stratified train-test split. Model performance was evaluated using:
- Confusion matrix
- Precision, recall, and F1-score
- ROC–AUC

The model demonstrates good ability to distinguish churners from non-churners.

## Business Recommendations
- Target fiber optic customers with proactive retention strategies
- Incentivize automatic payment methods over electronic checks
- Bundle value-added services such as OnlineBackup and TechSupport
- Focus retention efforts on high-charge, streaming-heavy customers
- Prioritize early engagement for new and non-family customers

## Tools & Technologies
- Python (pandas, numpy)
- Seaborn & Matplotlib
- Scikit-learn
- Jupyter Notebook

## Limitations & Future Work
- Explore tree-based models for non-linear relationships
- Perform threshold tuning to optimize recall
- Incorporate behavioral or time-series customer data
