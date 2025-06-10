# 🧠 Customer Churn Prediction using Machine Learning Models

> Predicting which customers are likely to churn so businesses can take proactive steps to retain them. 💸🧍‍♂️🧍‍♀️

---

## 📌 Project Description

This project aims to predict customer churn in a telecommunications company using supervised machine learning models. The dataset includes customer demographics, account information, and service usage patterns. The project walks through the full ML pipeline — from data cleaning to evaluation — and compares the performance of **Logistic Regression**, **Random Forest**, and **XGBoost** classifiers.

---

## 🔍 Problem Statement

Customer retention is crucial for subscription-based businesses. Losing existing customers is expensive, so identifying the ones who are likely to churn helps target interventions before it’s too late.

---

## 📂 Dataset

- **Source:** [Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Records:** ~7,000 customers
- **Features:** Demographics, account details, and service usage
- **Target:** `Churn` (Yes/No)

---

## 🧪 ML Pipeline

### ✅ 1. Data Preprocessing
- Dropped unnecessary columns
- Treated missing values
- Label encoding for binary categorical columns
- One-hot encoding for multi-category features
- Standardized numerical features using `StandardScaler`

### 🧠 2. Models Trained
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### ⚖️ 3. Handling Class Imbalance
- Applied **SMOTE** to upsample the minority class (`Churn = Yes`)
- Ensures balanced model learning without overfitting majority class


### 🧮 4. Evaluation Metrics

For a comprehensive view of performance, the following metrics were calculated for each model:

- ✅ Accuracy
- ✅ Precision
- ✅ Recall
- ✅ F1 Score
- ✅ ROC AUC Score
- ✅ Confusion Matrix
- ✅ ROC Curve Plots


### 🔮 5. Single Prediction Analysis

We randomly selected a single customer record to:
- 🔍 Predict churn probability
- 🔄 Compare predictions from all 3 models
- 🎯 Visualize model confidence in their decisions


### 📸 Visualizations

- 📈 **Class Distribution** before and after SMOTE
- 🔥 **Confusion Matrices** using heatmaps
- 🎯 **ROC Curve Plots** for side-by-side model comparison

---

## 🚀 How to Run Locally

```bash
git clone https://github.com/DharmaTeja2002/customer-churn-prediction.git
cd customer-churn-prediction
pip install -r requirements.txt
jupyter notebook
