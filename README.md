:

📊 Credit Card Delinquency Risk Analysis – Geldium (EDA)
This repository contains a complete Exploratory Data Analysis (EDA) project on credit card customer data from Geldium Finance. The goal is to identify data quality issues, missing values, and key risk factors that may contribute to credit card delinquency.

🔍 Objective
Before building any predictive models, it is essential to assess and understand the dataset's structure, completeness, and integrity. This EDA supports Tata iQ and Geldium’s analytics team in:

Evaluating dataset quality

Addressing missing data and outliers

Identifying early risk indicators of delinquency

Recommending strategies for modeling and intervention

📁 Dataset Overview
Rows: 500 customers

Features: Age, Income, Loan Balance, Credit Utilization, Payment History, Card Type, etc.

Target Variable: Delinquent_Account (1 = Missed Payment, 0 = Paid On Time)

✅ Key Tasks Completed
Data Cleaning

Removed irrelevant whitespaces

Checked data types and unique values

Handled missing values via median imputation

Missing Data Handling

Income & Loan Balance had MAR-type missingness

Used imputation (median) based on domain context

Outlier Detection

Detected and transformed extreme Income values using IQR

Avoided deletion to preserve sample size

Pattern Detection & Risk Factors

Used distribution plots, boxplots, and correlation matrix

Identified high credit utilization, missed payments, and card type as major risk indicators

Insights from GenAI

Used ChatGPT to suggest imputation strategies, identify anomalies, and interpret skewness

📌 Key Findings
Some features had unexpected values (e.g., “Student” card at age 56)

High credit utilization and missed payments are strongly associated with delinquency

Right-skewed income distribution with significant outliers

Dataset suitable for modeling after preprocessing

📎 Deliverables
EDA Summary Report (Word format)

Jupyter/Colab notebook with all analysis steps

Visualizations (distribution plots, heatmaps, boxplots)

🚀 Next Steps
Apply classification models (e.g., Logistic Regression, Random Forest)

Address class imbalance using SMOTE or other techniques

Build a dashboard to track delinquency risk indicators

🙌 Acknowledgments
This project was conducted as part of a hands-on analytics exercise for Tata iQ and Geldium Finance, with guidance from GenAI.

