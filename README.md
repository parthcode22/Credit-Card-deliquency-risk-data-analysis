# 📊 Credit Card Delinquency Risk Analysis

An end-to-end **Exploratory Data Analysis (EDA)** and **predictive modeling** project focused on identifying **credit card delinquency risk** using a real-world inspired dataset from **Geldium Finance**.  
This project was developed as part of a **business case study for Tata iQ**.

---

## 🔍 Problem Statement

Financial institutions face significant losses due to **late or missed credit card payments**.  
The goal of this project is to:
- Understand customer behavior patterns
- Identify early risk indicators of delinquency
- Build a reliable ML model to predict delinquent accounts

---

## 🎯 Objectives

- Perform in-depth **Exploratory Data Analysis**
- Detect data quality issues, outliers, and patterns
- Identify high-risk customer segments
- Build and evaluate predictive models for delinquency detection
- Provide business-ready insights and recommendations

---

## 📁 Dataset Overview

- **Total Records:** 500 customers  
- **Target Variable:**  
  - `Delinquent_Account`  
    - `1` → Missed Payment  
    - `0` → Paid on Time  

### Key Features
- Age  
- Income  
- Credit Score  
- Credit Utilization Ratio  
- Missed Payment Count  
- Loan Balance  
- Debt-to-Income Ratio  
- Card Type  

---

## 🧼 Data Cleaning & Preparation

- Removed leading and trailing whitespaces
- Handled missing values using **median imputation**
- Ensured consistent data types
- Preserved records to maintain business continuity

---

## 🚨 Outlier Analysis

- Identified outliers in **Income** and **Loan Balance** using the **IQR method**
- Outliers retained with transformations to avoid information loss

---

## 📊 Exploratory Data Analysis (EDA)

- Distribution plots & boxplots
- Correlation heatmaps
- Category-wise delinquency comparison
- Behavioral pattern identification

### Key Risk Indicators
- Low credit score
- High credit utilization
- Frequent missed payments
- Certain card types linked with higher risk

---

## 🤖 Predictive Modeling

### Techniques Used
- **SMOTE** for class imbalance handling
- Model comparison:
  - Logistic Regression
  - Decision Tree
  - XGBoost
  - Neural Networks

### Final Model
- **XGBoost Classifier**
- **Accuracy:** ~83%
- Evaluated using:
  - Confusion Matrix
  - F1-score
  - AUC-ROC

---

## 📌 Key Insights

- High credit utilization is a strong delinquency signal
- Missed payment history is the most influential predictor
- Class imbalance significantly affects model performance
- Explainability is crucial for financial decision systems

---

## 📂 Repository Structure

📦 Credit-Card-delinquency-risk-analysis
├── README.md
├── Tata_EDA.ipynb
├── docs/
│ ├── EDA_Report.md
│ ├── Business_Summary.md
│ └── Predictive_Model_Report.md


---

## 🚀 Future Improvements

- Deploy model using real-time data pipelines
- Add fairness & bias audits (e.g., AIF360)
- Build an interactive dashboard for monitoring risk
- Extend to multi-class risk classification (Low / Medium / High)

---

## 🙌 Acknowledgments

This project was developed with the support of **GenAI tools** (ChatGPT & Google Gemini) as part of a learning challenge by **Tata iQ** and **Geldium Finance**.  
Special thanks to mentors and domain experts for their guidance.

---

## 👤 Author

**Parth Indulkar**  
GitHub: [parthcode22](https://github.com/parthcode22)

