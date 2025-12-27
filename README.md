# 📊 Credit Card Delinquency Risk Analysis – Geldium (EDA & Modeling)

This repository presents an end-to-end data analysis and predictive modeling workflow for detecting delinquency risk in credit card customers, using Geldium Finance’s dataset. This project is part of a business case study conducted for Tata iQ.

---

# 🔍 Objective

Before deploying machine learning models for credit risk prediction, we performed an in-depth Exploratory Data Analysis (EDA) to understand:

- The quality and integrity of the dataset
- Patterns in customer behavior
- Early indicators of delinquency risk
- Data-driven recommendations for modeling

---

## 📁 Dataset Overview

- **Rows:** 500 customers
- **Target Variable:** `Delinquent_Account` (1 = Missed Payment, 0 = Paid On Time)
- **Key Features:** Age, Income, Credit Score, Credit Utilization, Payment History, Card Type, etc.

---

## ✅ Key Tasks Completed

### 🧼 Data Cleaning & Preparation
- Removed leading/trailing whitespaces
- Handled missing values using median imputation
- Ensured consistent datatypes

### 📉 Missing Data Handling
- Income and Loan Amount showed MAR-type missingness
- No records dropped — median imputed for business continuity

### 🚨 Outlier Detection
- Outliers in `Income` and `Loan Balance` were identified using IQR
- Retained with transformation to preserve data integrity

### 🔍 Pattern Detection
- Distribution plots, boxplots, and correlation heatmaps
- High credit utilization, missed payments, and card type linked to delinquency

### 🧠 Risk Factor Identification (via GenAI + EDA)
- Top risk features:
  - Credit Score
  - Missed Payment Count
  - Credit Utilization Ratio
  - Debt-to-Income Ratio
  - Card Type

---

## 📊 Predictive Modeling Plan

A conceptual ML pipeline was built using GenAI guidance, resulting in the following structure:

- Applied **SMOTE** to balance imbalanced target classes
- Compared multiple classifiers: Logistic Regression, Decision Tree, XGBoost, Neural Networks
- Final model chosen: **XGBoost Classifier** (Best Accuracy: 83%)

## 📄 Documentation

- 📘 [EDA Report – Geldium Delinquency](./EDA_Report_Geldium_Delinquency.docx)


## 📌 Key Insights

- Some anomalies exist (e.g., Student card for age 56)
- High credit utilization and missed payments are critical red flags
- Class imbalance significantly impacts predictive power
- Transparent, fair, and explainable models are essential in financial AI systems

---

## 📎 Deliverables

- [EDA Report (Notebook)](./EDA_Notebook.ipynb)
- [Model Planning Report (PDF)](./Geldium_Predictive_Model_Report.pdf)
- Visualizations: Countplots, Boxplots, Heatmaps, Feature Importance
- SMOTE implementation, Confusion Matrix, and AUC-F1 Score comparisons

---

## 🚀 Next Steps

- Deploy model with real-time data pipelines
- Integrate fairness audits (e.g., via AIF360)
- Build a dashboard to monitor key risk indicators
- Extend to multi-class classification (e.g., Low/Medium/High Risk)

---

## 🙌 Acknowledgments

This project was built with the support of **GenAI tools** (ChatGPT & Google Gemini) as part of a learning challenge by **Tata iQ and Geldium Finance**.  
Special thanks to the AI mentors and domain experts who helped shape this project.

---
