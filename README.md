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

<img width="587" height="526" alt="Fraud Rate by Transaction Type" src="https://github.com/user-attachments/assets/399b9dc7-6fd9-4fc7-850c-fb371b76e21e" />

#### Transaction Amount Distribution (Log Scale)

<img width="600" height="457" alt="Transaction Amount (Log Scale)" src="https://github.com/user-attachments/assets/8edfdcce-ad90-4831-9454-f3d3a1ca3030" />


#### Amount vs Fraud

<img width="592" height="457" alt="AmountVSFraud" src="https://github.com/user-attachments/assets/ef4128b8-b1a9-42d4-931c-7646decdc38d" />


#### Fraud Over Time

<img width="566" height="457" alt="Fraud Over Time" src="https://github.com/user-attachments/assets/2e3f6e6b-0528-4848-939c-429a4a1f33ff" />


---

## 📈 Key Insights

- Fraud is concentrated in specific transaction types (e.g., **TRANSFER, CASH_OUT**)
- Transaction amounts are highly skewed → log transformation improves analysis
- Fraud detection is a highly **imbalanced problem**
- High **recall** is critical to avoid missing fraudulent transactions

---

## 🧠 Machine Learning Model

- Algorithm: **Logistic Regression**
- Built using **Scikit-learn Pipeline**
- Includes:
  - OneHotEncoding for transaction type
  - Standard scaling for numerical features
  - Balanced class weights to handle imbalance

---

## ⚠️ Imbalanced Data Handling

Fraud detection datasets are highly imbalanced:

- Most transactions are legitimate  
- Fraud cases are rare  

To address this:

- Used `class_weight="balanced"`
- Focused on **Recall, Precision, and F1-score** instead of accuracy

> Detecting fraud is more sensitive to **false negatives** than false positives.

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

### 🔗 Live App

[ADD YOUR STREAMLIT LINK HERE]

---

## 📸 App Preview

<img width="1981" height="1864" alt="image (2)" src="https://github.com/user-attachments/assets/5462bd0b-7ad0-4364-9fbe-2a09d5a3e62f" />

<img width="1987" height="1958" alt="image (1)" src="https://github.com/user-attachments/assets/f7bf2f1c-2d9f-4301-85cb-f9591a57c4b7" />



---

## 🛠️ Tech Stack

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Streamlit  
- Joblib  

---

## 📊 Data Source

Dataset sourced from Kaggle:

**Fraud Detection Dataset**

🔗 https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset

> Note: The dataset is synthetic and designed to simulate real-world financial transactions.
