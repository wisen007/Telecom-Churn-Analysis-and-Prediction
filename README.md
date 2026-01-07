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


- ## Key Exploratory Insights

From exploratory data analysis, the following churn patterns were observed:

1. **Senior citizens show higher churn than non-senior citizens**  
   Churn among senior citizens is higher than non-senior citizens (**41.68% vs 23.61%**).

2. **Fiber optic customers have the highest churn**  
   Customers using fiber optic internet have a higher churn rate than customers using DSL and no internet service combined (**41.89% vs 26.36%**).

3. **Online security is strongly associated with churn**  
   Customers with **no online security** churn at nearly double the rate of those with online security (**41.77% vs 22.01%**).

4. **Online backup reduces churn risk**  
   Customers without online backup churn at nearly twice the rate of those with online backup (**39.93% vs 21.53%**).

5. **Tech support is a strong retention factor**  
   Customers without tech support churn at almost three times the rate of those with tech support (**41.64% vs 15.17%**).

6. **Streaming services show limited impact on churn**  
   Churn rates are relatively similar for customers with and without streaming TV (**33.07% vs 30.07%**). A similar pattern is observed for streaming movies.

7. **Contract type is one of the strongest churn drivers**  
   Month-to-month customers churn at a much higher rate than customers on one-year and two-year contracts combined (**42.71% vs 14.10%**).


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
