
---

## 📌 Problem Statement

Customer churn is a major challenge in service industries. Retaining existing customers is **more cost-effective** than acquiring new ones. This project focuses on building a machine learning model that can **predict which customers are at risk of leaving**, allowing the business to take proactive measures.

---

## 🔍 Dataset Overview

- **Source**: Telco-style synthetic dataset  
- **Rows**: ~7,000  
- **Target Variable**: `Churn` (Yes/No)  
- **Features**: Customer demographics, account info, usage metrics, and service-related parameters

---

## 🔧 Key Steps & Workflow

### 1. Data Preprocessing 🧼
- Handling missing values
- Encoding categorical features (LabelEncoding & OneHotEncoding)
- Feature scaling (StandardScaler)

### 2. Exploratory Data Analysis 📊
- Univariate and bivariate analysis
- Correlation heatmaps
- Distribution of churned vs retained customers

### 3. Feature Engineering 🛠️
- Removed irrelevant columns
- Created derived features
- Checked feature importance (via Random Forest)

### 4. Model Building & Evaluation 🧠
Tested multiple models:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- XGBoost

**Evaluation Metrics Used**:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

---

## 🏆 Model Performance Summary

| Model               | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression|   0.81   |   0.70    |  0.55  |  0.62    |
| KNN                |   0.76   |   0.60    |  0.40  |  0.48    |
| Decision Tree      |   0.78   |   0.62    |  0.50  |  0.55    |
| **Random Forest**  | **0.83** | **0.74**  |**0.65**|**0.69**  |
| SVM                |   0.80   |   0.00    |  0.00  |  0.00    |
| **XGBoost**        | **0.84** | **0.75**  |**0.68**|**0.71**  |

**Final Recommendation**: Random Forest and XGBoost provide the best balance of recall and precision for business needs.

---

## ✅ Key Learnings

- Real-world ML is 80% preprocessing and evaluation
- Accuracy is not everything — *recall and precision are critical* in churn detection
- Feature importance helps prioritize which attributes drive customer retention
- Tree-based models often outperform linear models in tabular, non-linear problems

---

## 💼 Business Impact

- 🔍 **Retention Strategy**: Identify churn-prone customers and take action (offers, surveys, service fixes)
- 🎯 **Targeted Marketing**: Focus retention campaigns on likely churners → lower cost, better ROI
- 💬 **Customer Feedback Loops**: Track features contributing to churn to improve service (e.g., high complaints, low tenure)
- 📉 **Profit Boost**: Even a 5% drop in churn can increase profits by 25–125% (Bain & Co.)

---

## 🧠 Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📁 How to Run This Project

1. Clone the repo  
2. Install dependencies:
