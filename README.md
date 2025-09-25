📄 Credit Risk Modeling Project
🎯 Project Overview
This repository contains a comprehensive Credit Risk Modeling project developed within the Jupyter Notebook credit_risk_model.ipynb.

The primary objective is to build a machine learning classification model to predict the probability of credit default (i.e., whether a customer will fail to repay a loan). The notebook covers the complete data science lifecycle, from data ingestion and cleaning to model training and persistence.

💾 Data Sources
The model is built by combining data from three distinct CSV files, which should be placed in the same directory as the notebook. All files are joined on the common identifier cust_id.

File Name	Content Description	Key Information
customers.csv	Customer demographic and financial information.	Age, Income, Residence Details.
loans.csv	Loan application details and the target variable.	Loan Amount, Tenure, Target: default (1=Default, 0=No Default).
bureau_data.csv	Customer's credit history details.	Total DPD, Enquiry Count, Credit Utilization Ratio.


💻 Workflow Highlights
The credit_risk_model.ipynb notebook executes the following critical steps:

Data Loading & Merging: Ingestion of the three source files and creation of a unified master DataFrame.

Strategic Splitting: The data is split into training and testing sets early in the process to prevent data leakage during feature engineering.

Data Cleaning: Handles missing values (e.g., imputation of residence_type with the mode 'Owned') and removal of duplicates.

Feature Engineering: Creation of derived features such as loan_to_income_ratio and age_at_loan_end.

Encoding & Scaling:

Target Encoding for high-cardinality features (city, state).

One-Hot Encoding for other nominal features.

Standard Scaling for numerical features.

Model Training: The predictive model is built using the Logistic Regression algorithm.

Evaluation: The model performance is assessed using industry-standard metrics, primarily the AUC Score, alongside the Confusion Matrix and Classification Report.

Model Persistence: The final trained model, the list of features, and the fitted scaler are serialized and saved for future deployment.

Try it here:- https://classification-project-credit-risk-modelling.streamlit.app/

Model Persistence: The final trained model, the list of features, and the fitted scaler are serialized and saved for future deployment.

