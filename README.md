# Bank Customer Churn Prediction

### Machine Learning project for predicting customer churn in a banking environment using classification models and exploratory data analysis.

### Project Overview

Customer churn is a major challenge for banks because losing customers directly impacts revenue and growth. This project develops a complete machine learning pipeline to identify customers who are likely to leave the bank.

### The notebook covers:

Data loading and exploration   
Data cleaning and preprocessing    
Feature engineering  
Exploratory Data Analysis (EDA)  
Model training and evaluation  
Model comparison  
Business insights and recommendations  

### Dataset
The dataset contains customer information such as:

Credit Score  
Geography  
Gender  
Age  
Tenure  
Balance  
Number of Products  
Has Credit Card  
Is Active Member  
Estimated Salary  

### Target Variable:
Exited (1 = Customer Churned, 0 = Customer Stayed)  

### Technologies Used
Python  
Pandas  
NumPy  
Matplotlib  
Seaborn  
Scikit-learn   
Imbalanced-learn (SMOTE)  

### Models Evaluated
Dummy Baseline  
K-Nearest Neighbors (KNN)  
Logistic Regression  
Random Forest  

### Key Findings
Customer churn rate is approximately 20%.   
Age is one of the strongest predictors of churn.  
Customers from Germany show significantly higher churn rates.  
Inactive members are more likely to leave the bank.  
Customers holding 3–4 products exhibit unusually high churn rates.  

### Business Recommendations
Focus retention campaigns on high-risk customer segments.  
Increase engagement initiatives for inactive members.  
Develop targeted offers for customers with multiple products.  
Monitor churn risk among older customers and German customers.  
