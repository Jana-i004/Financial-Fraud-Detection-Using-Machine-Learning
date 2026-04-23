# 💳 AI Fraud Detection using Machine Learning

> مشروع يهدف إلى كشف عمليات الاحتيال المالي باستخدام تقنيات الذكاء الاصطناعي وتعلم الآلة

An end-to-end **AI-powered machine learning project** for detecting fraudulent financial transactions, combining data analysis, visualization, and a real-time Streamlit application.

---
## 🚀 Project Overview

This project builds a **transaction risk detection system** that identifies potentially fraudulent financial activities using machine learning.

The workflow includes:

- 📊 Exploratory Data Analysis (EDA)
- 📈 Data Visualization
- ⚙️ Feature Engineering
- 🤖 Machine Learning Modeling
- 🖥️ Interactive Streamlit Application

---
## 🎯 Objective

To predict whether a transaction is likely to be **fraudulent** based on:

- Transaction type  
- Transaction amount  
- Sender balance  
- Receiver balance  
- Transaction behavior patterns  

---
## 📊 Exploratory Data Analysis

Before modeling, the dataset was analyzed to uncover patterns and better understand fraud behavior.

### Key Visual Insights

#### Fraud Rate by Transaction Type

<img width="587" height="526" alt="Fraud Rate by Transaction Type" src="https://github.com/user-attachments/assets/27beae99-b794-4985-95db-200c861a2613" />

#### Transaction Amount Distribution (Log Scale)

<img width="600" height="457" alt="Transaction Amount (Log Scale)" src="https://github.com/user-attachments/assets/3202f802-07c4-4c8b-951c-e823ba2ff2fe" />

#### Amount vs Fraud

<img width="592" height="457" alt="AmountVSFraud" src="https://github.com/user-attachments/assets/102c4cf5-9d4d-46e1-baf2-a75a6aeaa6ef" />

#### Fraud Over Time

<img width="566" height="457" alt="Fraud Over Time" src="https://github.com/user-attachments/assets/a1f0888b-a10a-4308-889b-dd4e7c591fb0" />

---
## 📈 Key Insights

- Fraud is concentrated in specific transaction types (e.g., **TRANSFER, CASH_OUT**)
- Transaction amounts are highly skewed → log transformation improves analysis
- Fraud detection is a highly **imbalanced problem**
- High **recall** is critical to avoid missing fraudulent transactions

---
## ⚡️ Machine Learning Model

- Algorithm: **Logistic Regression**
- Built using **Scikit-learn Pipeline**
- Includes:
  - OneHotEncoding for transaction type
  - Standard scaling for numerical features
  - Balanced class weights to handle imbalance

---
## ‼️ Imbalanced Data Handling
Fraud detection datasets are highly imbalanced:

- Most transactions are legitimate  
- Fraud cases are rare  

To address this i used :
-  `class_weight="balanced"`
- Focused on **Recall, Precision, and F1-score** instead of accuracy
-  Detecting fraud is more sensitive to **false negatives** than false positives.

---
## 📊 Model Performance

Fraud Recall: 94%
Fraud Precision: 2%
- Model is effective as a **risk-flagging system**


---
## 🖥️ Application

An interactive **Streamlit app** allows users to:

- Enter transaction details  
- Simulate real-world scenarios  
- Get instant fraud risk predictions  

### 🔗 App


---
## 📸 App Preview

<img width="1981" height="1864" alt="image (2)" src="https://github.com/user-attachments/assets/69e8f3f1-6cd7-439e-91b9-8ff37dd4dd9f" />

<img width="1987" height="1958" alt="image (1)" src="https://github.com/user-attachments/assets/9559cda5-988e-4d6a-8060-9498548046c7" />



---
## 🛠️ Tech Tools
- Python (Pandas ,NumPy , Matplotlib , Seaborn , Scikit-learn)  
- Streamlit  
- Joblib  

---

## 📊 Data Source

Dataset sourced from Kaggle:

🔗 https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset

> Note: The dataset is synthetic and designed to simulate real-world financial transactions 
