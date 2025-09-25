📄 CREDIT RISK MODELING PROJECT
🎯 Project Overview

This repository contains a comprehensive Credit Risk Modeling project, developed in the Jupyter Notebook credit_risk_model.ipynb.

The goal is to predict the probability of loan default (whether a customer will fail to repay).
The notebook covers the full Data Science lifecycle: data ingestion ➝ cleaning ➝ feature engineering ➝ model training ➝ evaluation ➝ deployment.

💾 Data Sources

The model uses three CSV files, joined by the key cust_id.
Ensure these files are placed in the same directory as the notebook.

File Name	Description	Key Features
customers.csv	Customer demographics & financial details	Age, Income, Residence Details
loans.csv	Loan application info & target variable	Loan Amount, Tenure, Default (0/1)
bureau_data.csv	Credit bureau history	Total DPD, Enquiry Count, Utilization
💻 Workflow Highlights

The notebook executes the following critical steps:

Data Loading & Merging → Combine the three datasets into a single master DataFrame.

Strategic Splitting → Train-test split early to prevent data leakage.

Data Cleaning → Handle missing values (e.g., impute residence_type with "Owned"), remove duplicates.

Feature Engineering → Create features like loan_to_income_ratio and age_at_loan_end.

Encoding & Scaling

Target Encoding for high-cardinality (city, state).

One-Hot Encoding for nominal features.

Standard Scaling for numerical features.

Model Training → Logistic Regression for predicting default probability.

Evaluation → Metrics include:

✅ AUC Score

✅ Confusion Matrix

✅ Classification Report

Model Persistence → Save trained model, feature list, and scaler for deployment.

🚀 Live Demo

👉 Try the interactive Streamlit app here:
🔗 Credit Risk Modeling App- https://classification-project-credit-risk-modelling.streamlit.app/




