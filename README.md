# Bank Customer Churn Prediction

Machine Learning project for predicting customer churn in a banking environment using classification models and exploratory data analysis.

## Overview

Customer churn is a major challenge for banks because losing customers directly impacts revenue and growth. This project develops a complete machine learning pipeline to identify customers who are likely to leave the bank.

**Churn rate in the dataset:** ~20%, making this a classic class imbalance problem.

---

## Pipeline

```text
Raw Data → Cleaning → Feature Engineering → EDA → Modeling → Evaluation → Insights
```

---

## 1. Data Cleaning

* Standardized column names and text values
* Removed duplicates and impossible values
* Fixed data types and encoded categorical features (One-Hot + Label Encoding)

## 2. Feature Engineering

* Engineered interaction features to improve signal
* Outlier detection and treatment

## 3. Exploratory Data Analysis (EDA)

* Target distribution analysis
* Hypothesis testing across key variables:

  * Age
  * Balance
  * Gender
  * Geography
  * Activity
* Correlation heatmap

## 4. Modeling

* Train/test split with stratification
* Class imbalance handled via **SMOTE (Synthetic Minority Oversampling Technique)**
* StandardScaler applied before distance-based models

## 5. Models Trained

| Model               | ROC-AUC | F1 (Churn Class) |
| ------------------- | ------- | ---------------- |
| Dummy Baseline      | 0.500   | 0.000            |
| K-Nearest Neighbors | ~0.76   | ~0.52            |
| Logistic Regression | ~0.77   | ~0.55            |
| Random Forest       | ~0.86   | ~0.63            |

## 6. Evaluation

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* ROC Curve Comparison Across Models
* Overfitting Check (Train vs Test Scores)
* 5-Fold Cross-Validation
* Feature Importance Analysis

## Key Findings

* Customer churn rate is approximately **20%**
* Age is one of the strongest predictors of churn
* Customers from Germany show significantly higher churn rates
* Inactive members are more likely to leave the bank
* Customers holding 3–4 products exhibit unusually high churn rates
* Top features by importance:

  * Age
  * NumOfProducts
  * EstimatedSalary
  * CreditScore
  * Tenure

## Business Recommendations

* Focus retention campaigns on high-risk customer segments
* Increase engagement initiatives for inactive members
* Develop targeted offers for customers with multiple products
* Monitor churn risk among older customers and German customers

## Tech Stack

### Language

* Python 3.12

### Libraries

* pandas
* numpy
* scikit-learn
* imbalanced-learn (SMOTE)
* matplotlib
* seaborn
