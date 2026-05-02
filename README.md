# Customer Churn Prediction (Telco Dataset)

## 📌 Overview

This project focuses on predicting customer churn using machine learning techniques on the IBM Telco Customer Churn dataset. The objective is to identify customers at risk of leaving and provide actionable insights to improve retention strategies.

The dataset contains ~7,000 customer records with demographic, service usage, and billing information, making it suitable for real-world churn prediction analysis. 

---

## 🎯 Objectives

* Perform exploratory data analysis (EDA) to understand churn patterns
* Preprocess data (handling missing values, encoding, scaling)
* Address class imbalance using SMOTE
* Build and optimize machine learning models
* Evaluate performance using multiple metrics
* Extract business insights for customer retention

---

## 📊 Dataset

* Source: IBM Telco Customer Churn Dataset
* Records: ~7,032 after cleaning
* Features: 20+ (expanded to 31 after encoding)
* Target: Churn (Yes / No)

Key characteristics:

* Imbalanced dataset (~73% non-churn, ~27% churn)
* Mix of categorical and numerical features

---

## ⚙️ Methodology

### 🔹 Data Preprocessing

* Converted TotalCharges to numeric
* Removed missing values
* Dropped unnecessary columns (customerID)
* Encoded categorical variables

### 🔹 Feature Engineering

* One-hot encoding for categorical features
* Feature scaling using StandardScaler

### 🔹 Handling Imbalance

* Applied SMOTE (Synthetic Minority Oversampling Technique)
* Balanced dataset from 73:27 → 50:50

### 🔹 Model Building

* Algorithm: Random Forest Classifier
* Hyperparameter tuning using GridSearchCV
* Cross-validation for robust evaluation

---

## 🤖 Models Used

* Random Forest (Primary Model)
* Logistic Regression (Baseline)
* XGBoost (Exploratory)

---

## 📈 Results

* Accuracy: **78%**
* ROC-AUC: **0.820**
* Cross-validation ROC-AUC: **0.931**
* Churn F1-Score: **0.61**

Confusion Matrix:

* True Positives: 236
* True Negatives: 866
* False Positives: 167
* False Negatives: 138

---

## 📊 Key Insights

* **Tenure** is the most important feature (~15%)
* Customers with **short tenure are more likely to churn**
* **Monthly Charges and Total Charges** strongly influence churn
* **Electronic payment users** show higher churn risk
* Long-term contracts reduce churn probability

---

## 💼 Business Impact

* Model helps identify high-risk customers
* Enables targeted retention strategies
* Estimated **59% ROI improvement** in retention campaigns
* Supports data-driven decision-making in telecom industry

---

## 🧠 Tech Stack

Python • Pandas • NumPy • Scikit-learn • SMOTE • Matplotlib • Seaborn

---

## 📁 Project Structure

* Notebook: Customer-Churn-Code.ipynb
* Dataset: Telco Customer Churn CSV
* Visualisations: EDA plots, ROC curve, confusion matrix

---

## 🚀 Future Improvements

* Implement XGBoost for better performance
* Add real-time churn prediction system
* Deploy model using API (FastAPI / Flask)
* Integrate SHAP for explainability

---

## 📌 Conclusion

This project demonstrates a complete end-to-end machine learning pipeline for churn prediction, combining data preprocessing, imbalance handling, model optimisation, and business insight generation.

It reflects real-world problem-solving using data science techniques.
