# Credit Card Fraud Detection

## 📌 Project Overview
This project focuses on detecting **fraudulent credit card transactions** using machine learning techniques.  
The primary objective is to identify fraud cases in a **highly imbalanced dataset**, while minimizing false negatives — a critical requirement in real-world financial systems.

---

## 📊 Dataset
- **Source:** Credit Card Fraud Detection Dataset (Kaggle)  
  https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

- **Description:**
  - Transactions made by European cardholders in September 2013
  - Highly imbalanced dataset
  - Features `V1`–`V28` are PCA-transformed for confidentiality
  - **Target variable:** `Class`  
    - `0` → Non-Fraud  
    - `1` → Fraud

---

## Approach & Methodology
- Performed Exploratory Data Analysis (EDA) to understand:
  - Class imbalance
  - Feature distributions
- Applied feature scaling to `Time` and `Amount`
- Used stratified train–test split to preserve class distribution
- Focused on **Recall** and **ROC-AUC** as primary evaluation metrics
- Performed threshold tuning to balance recall and precision for fraud detection

---

## Models Used
- Logistic Regression (baseline)
- Random Forest
- XGBoost (primary model)

---

## 📈 Evaluation Metrics
Due to the imbalanced nature of the dataset, the following metrics were prioritized:
- ROC-AUC Score
- Recall (Fraud Class)
- Precision
- F1-Score
- Confusion Matrix

This ensures the model effectively identifies fraudulent transactions while controlling false positives.
