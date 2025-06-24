# Customer-Churn-Analysis

## Overview

This project analyzes customer churn behaviour in a telecom company using python and machine learning techniques. The goal is to identify patterns and drivers of churn so the business can take strategic actions to customer retention.

## Objectives
clean and preprocess the dataset

explore customer behaviour paaterns

build classification models to predict churn 

evaluate model performance

provide business insights and actionable strategies

## Tools Used 
**Python**: (pandas, seaborn, scikit-learn)

**Google Colab**

**Machine Learning models**: Logistic regression, Random Forest

**Techniques**: data scaling, class balancing(SMOTE)

## Data prepration
dropped irrelevant columns like 'customerID'

converted 'TotalCharges' to numeric 

handled missing values 

scaled features using 'standardScaler'

addressed class imbalance using SMOTE

## Exploratory Data Analysis (EDA)
### churn distribution 
around 26% of customers churned
### contract type
most churners were on month to month contracts
### monthly charges 
higher monthly charges are associated with higher churn 

### 1. **Logistic Regression** (with SMOTE)
| Metric        | Value |
|---------------|--------|
| Accuracy      | 77%    |
| Recall (Churn)| **53%** 
| Precision     | 61%    
| F1-score      | **0.56** 

### 2. **Random Forest** (with SMOTE)
| Metric        | Value |
|---------------|--------|
| Accuracy      | **79%** 
| Recall (Churn)| 45%    
| Precision     | **67%** 
| F1-score      | 0.54    

## Model Choice
while random forest achieved slightly better accuracy and precision , **logistic regression** was chosen because:

> higher recall for churn - more likely to detect customer at risk
> in churn prediction , missing churners is costlier than false positives.

## Conclusion
This project highlights how machine learning can effectively predict customer churn and support business decisions. By analyzing telecom data, we identified churn drivers and improved churn detection using SMOTE and logistic regression. The model enables targeted retention strategies, making it a valuable tool for reducing customer loss and boosting revenue.

