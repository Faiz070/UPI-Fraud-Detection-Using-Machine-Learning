# 💳 UPI Fraud Detection Using Machine Learning

## 📘 Project Overview
The **UPI Fraud Detection System** is a Machine Learning–based solution designed to identify and prevent fraudulent transactions in digital payment systems such as UPI (Unified Payments Interface).  
The project aims to improve transaction security using data-driven fraud detection techniques, ensemble learning, and real-time predictive analysis.

This model utilizes **XGBoost**, **Random Forest**, and **Logistic Regression** to classify transactions as legitimate or fraudulent, focusing on achieving a balanced trade-off between **precision**, **recall**, and **F1-score**.

---

## 🎯 Objectives
- Detect fraudulent UPI transactions with high accuracy.  
- Handle data imbalance using **SMOTETomek resampling**.  
- Build an **ensemble ML model** that combines multiple algorithms for better performance.  
- Evaluate performance using **Precision, Recall, F1-score, and ROC-AUC**.  
- Optimize thresholds for practical fraud detection in real-time.  
- Prepare the system for **real-time deployment** using REST APIs.

---

## 🧠 Key Features
- **Data Preprocessing:** Cleans, encodes, and normalizes transaction data.  
- **Feature Engineering:** Creates temporal, behavioral, and relational features to capture fraud patterns.  
- **SMOTETomek Sampling:** Balances the dataset by combining oversampling and undersampling.  
- **Ensemble Learning:** Combines XGBoost, Random Forest, and Logistic Regression.  
- **Threshold Tuning:** Dynamically adjusts fraud probability thresholds.  
- **Evaluation Metrics:** Confusion Matrix, ROC-AUC, PR-AUC, and detailed classification report.  
- **Scalability:** Prepared for cloud deployment and real-time inference.

---

## 🏗️ System Architecture
The project follows a **layered architecture** consisting of:
1. **Data Layer:** Stores and retrieves transaction data (Parquet/CSV format).  
2. **Processing Layer:** Handles data cleaning, feature extraction, and transformation.  
3. **ML Layer:** Trains the ensemble model and performs validation.  
4. **Application Layer:** Executes predictions and applies threshold-based decision logic.  
5. **Output Layer:** Displays fraud probability, classification result, and evaluation metrics.

---

## 📊 Dataset Information
- **Source:** IEEE-CIS Fraud Detection Dataset (adapted for UPI transactions)  
- **Format:** `.parquet` and `.csv`  
- **Total Records:** ~500,000 transactions  
- **Key Fields:**  
  - Transaction ID  
  - Payer ID, Payee ID  
  - Transaction Amount  
  - Device ID, IP Address  
  - ProductCD, Card Type, Email Domain  
  - Transaction Timestamp  
  - Fraud Label (0 = Legitimate, 1 = Fraud)

---

## ⚙️ Technologies Used

 **Programming Language** | Python 3.9+ 
 **IDE / Notebook** | Jupyter Notebook / Anaconda 
 **Machine Learning** | XGBoost, Random Forest, Logistic Regression 
 **Data Processing** | Pandas, NumPy, Scikit-learn 
 **Resampling Techniques** | SMOTE, Tomek Links (Imbalanced-learn) 
 **Visualization** | Matplotlib, Seaborn, Plotly 
 **Model Deployment** | Flask / FastAPI (for real-time API integration) 
 **Version Control** | Git, GitHub 

---
