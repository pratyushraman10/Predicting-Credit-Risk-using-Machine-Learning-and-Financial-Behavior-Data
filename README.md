Predicting Credit Risk using Machine Learning and Financial Behavior Data
=========================================================================

Overview:
---------
This project explores the use of supervised machine learning techniques to assess and predict credit default risk based 
on customer financial behavior. The objective is to build a predictive model that can assist financial institutions 
in identifying high-risk clients in advance, thereby reducing loan losses and enhancing credit decision processes.

The model is trained on the "Default of Credit Card Clients" dataset from the UCI Machine Learning Repository, which 
contains detailed records of 30,000+ credit card holders. The dataset includes demographic information, credit limits, 
bill payment history, and past repayment behavior. The project uses XGBoost for classification and SHAP for model 
interpretability.

Dataset:
--------
- Source: UCI Machine Learning Repository
- Records: 30,000+ customers
- Features: Credit limit, repayment history, bill amounts, education level, marital status, age, and payment delays
- Target: Binary indicator of whether a customer will default on their payment in the next month (1 = default, 0 = no default)

Approach:
---------
- Data Cleaning: Removal of redundant columns and renaming of target variable
- Feature Scaling: Standardization of numerical features using Scikit-Learn
- Class Imbalance Handling: Application of SMOTE (Synthetic Minority Over-sampling Technique)
- Model Training: XGBoost Classifier selected for its performance and suitability for tabular data
- Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, ROC AUC used to measure classification performance
- Explainability: SHAP (SHapley Additive exPlanations) applied to interpret feature contributions and explain model behavior

Implementation Details:
-----------------------
- Tools and Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn, xgboost, shap
- Preprocessing: One-hot encoding not required; numeric-only features used directly
- SMOTE: Applied only to training set to avoid data leakage
- SHAP Analysis: Used to visualize feature importance and individual prediction explanations

Applications:
-------------
- Credit risk assessment and early warning systems
- Loan approval automation
- Fintech decision engines for creditworthiness evaluation
- Regulatory explainability and transparency in ML-based financial services

Author:
-------
Pratyush Raman  
B.Tech, National Institute of Technology Rourkela  
LinkedIn: https://www.linkedin.com/in/pratyushraman10
