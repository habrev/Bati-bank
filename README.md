# Credit Scoring Model for Buy-Now-Pay-Later Service

## Overview
Bati Bank, a leading financial service provider with over 10 years of experience, is partnering with an emerging eCommerce company to introduce a **Buy-Now-Pay-Later (BNPL)** service. This service enables customers to purchase products on credit, provided they qualify based on their creditworthiness.

## Objective
The goal of this project is to develop a **Credit Scoring Model** using transaction and user data provided by the eCommerce platform. The model will estimate the likelihood of a customer defaulting on their payments, ensuring responsible lending practices and compliance with **Basel II Capital Accord**.

## What is Credit Scoring?
Credit scoring is the process of assigning a **quantitative score** to potential borrowers based on statistical analysis of previous borrowers’ financial behaviors. The model predicts the likelihood of future defaults, allowing lenders to make informed decisions.

## Key Steps in Credit Scoring Model Development

### 1. **Data Collection & Preprocessing**
- Gather customer transaction history, demographics, and financial behavior data.
- Clean and preprocess the dataset (handling missing values, outliers, etc.).
- Feature engineering using **RFMS (Recency, Frequency, Monetary, Stability)**.

### 2. **Defining Default Criteria**
- The definition of **default** varies among financial institutions but must comply with **Basel II Capital Accord**.
- Default classification will be based on the **loan repayment history** and **delinquency thresholds**.

### 3. **Exploratory Data Analysis (EDA)**
- Understand distributions, correlations, and data patterns.
- Identify key risk factors contributing to default.

### 4. **Feature Engineering & Weight of Evidence (WoE) Binning**
- Transform categorical and continuous features for better predictive power.
- Apply **Weight of Evidence (WoE) and Information Value (IV)** to improve model interpretability.

### 5. **Model Development**
- Train different classification models such as:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - Gradient Boosting (XGBoost, LightGBM)
  - Neural Networks (if needed)
- Evaluate model performance using **ROC-AUC, Precision-Recall, and F1-score**.

### 6. **Model Validation & Deployment**
- Test on unseen data to assess generalization.
- Deploy the model into Bati Bank’s BNPL decision system.

## Compliance with Basel II Capital Accord
- Basel II guidelines require financial institutions to assess risk based on **credit, operational, and market risks**.
- The credit scoring model must align with Basel II’s **risk-based approach** for loan procedures.

## Expected Outcomes
- A **robust credit scoring model** for the BNPL service.
- Accurate classification of **good vs. bad borrowers**.
- A risk assessment framework aligned with **Basel II regulations**.

---
By implementing this credit scoring system, Bati Bank ensures responsible lending, minimizes default risk, and enhances customer financial accessibility through the BNPL service.