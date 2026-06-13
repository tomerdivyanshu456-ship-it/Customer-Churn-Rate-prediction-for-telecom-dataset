# Customer-Churn-Rate-prediction-for-telecom-dataset
# Customer Churn Prediction using Machine Learning

## Project Overview

Customer churn is one of the most critical business challenges faced by subscription-based companies. Identifying customers who are likely to leave enables organizations to improve retention strategies, reduce revenue loss, and increase customer lifetime value.

This project develops an end-to-end Machine Learning pipeline for customer churn prediction using a synthetic dataset containing 100,000 customer records. Multiple machine learning algorithms were trained and evaluated to determine the most effective model for predicting customer churn.

---

## Problem Statement

The objective of this project is to predict whether a customer will churn based on demographic information, account details, contract type, service usage, and billing characteristics.

### Business Impact

Accurate churn prediction helps organizations:

* Identify at-risk customers
* Improve customer retention
* Reduce acquisition costs
* Increase profitability
* Design targeted marketing campaigns

---

## Dataset Information

Dataset: **synthetic_customer_churn_100k.csv**

### Dataset Size

* Total Records: 100,000
* Target Variable: Churn
* Problem Type: Binary Classification

### Features Used

| Feature         | Description                     |
| --------------- | ------------------------------- |
| CustomerID      | Unique customer identifier      |
| Gender          | Customer gender                 |
| SeniorCitizen   | Senior citizen status           |
| Partner         | Whether customer has a partner  |
| Dependents      | Whether customer has dependents |
| Tenure          | Months with company             |
| PhoneService    | Phone service subscription      |
| InternetService | Internet service type           |
| Contract        | Contract category               |
| PaymentMethod   | Customer payment method         |
| MonthlyCharges  | Monthly bill amount             |
| TotalCharges    | Total amount paid               |
| Churn           | Target variable                 |

### Target Variable

* Yes → Customer churned
* No → Customer retained

---

## Project Workflow

Data Collection

↓

Exploratory Data Analysis (EDA)

↓

Data Cleaning & Preprocessing

↓

Feature Encoding

↓

Train-Test Split

↓

Model Training

↓

Model Evaluation

↓

Model Comparison

↓

Feature Importance Analysis

---

## Exploratory Data Analysis

The following analyses were performed to understand customer behavior and identify factors affecting churn.

### Churn Distribution

Analyzed the class distribution of churned and retained customers.

**Output:** `churn_distribution.png`

### Correlation Analysis

Generated a correlation heatmap to understand relationships among numerical variables.

**Output:** `correlation_heatmap.png`

### Contract Type vs Churn

Investigated how customer contract types influence churn rates.

**Output:** `churn_by_contract.png`

### Monthly Charges vs Churn

Analyzed the relationship between customer monthly charges and churn probability.

**Output:** `monthly_charges_vs_churn.png`

---

## Data Preprocessing

The following preprocessing steps were applied:

### Missing Value Handling

* Numerical Features → Median Imputation
* Categorical Features → Most Frequent Imputation

### Categorical Encoding

* One-Hot Encoding

### Feature Selection

* Removed CustomerID

### Train-Test Split

* Training Data: 80%
* Testing Data: 20%
* Stratified Sampling Applied

---

## Machine Learning Models

The following classification algorithms were trained and evaluated:

### Logistic Regression

* Baseline classification model
* Fast and interpretable

### Decision Tree

* Captures non-linear relationships
* Easy to visualize and explain

### Random Forest

* Ensemble learning approach
* Reduces overfitting
* Provides feature importance scores

### XGBoost

* Gradient boosting algorithm
* High predictive performance
* Industry-standard machine learning model

---

## Evaluation Metrics

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score

---

## Model Comparison

The performance of all models was compared using ROC-AUC and other classification metrics.

**Output:** `model_comparison.png`

## Results Summary

| Model               | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---------            |---------:|---------:|---------:|---------:|---------:|
| XGBoost             | 0.7620 | 0.6682 | 0.5600 | 0.6093 | 0.8040 |
| Decision Tree       | 0.7589 | 0.6656 | 0.5477 | 0.6010 | 0.8018 |
| Random Forest       | 0.7306 | 0.6115 | 0.5134 | 0.5581 | 0.7877 |
| Logistic Regression | 0.7233 | 0.6078 | 0.4658 | 0.5274 | 0.7719 |

---

## Feature Importance Analysis

Feature importance was extracted using ensemble-based models to identify the strongest factors contributing to customer churn.

**Output:** `feature_importance.png`

Example influential features may include:

* Contract Type
* Tenure
* Monthly Charges
* Payment Method
* Internet Service

---

## Confusion Matrix

The confusion matrix was generated for the best-performing model (XGBoost) to evaluate prediction performance in greater detail.

**Output:** `xgboost_confusion_matrix.png`

---

## Results

Generated Visualizations:

* churn_distribution.png
* correlation_heatmap.png
* churn_by_contract.png
* monthly_charges_vs_churn.png
* feature_importance.png
* model_comparison.png
* xgboost_confusion_matrix.png

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost

---

Customer-Churn-Prediction/

├── README.md
├── Requirements.txt
├── churn_prediction.ipynb
├── synthetic_customer_churn_100k.csv
│
├── churn_distribution.png
├── correlation_heatmap.png
├── churn_by_contract.png
├── monthly_charges_vs_churn.png
├── feature_importance.png
├── model_comparison.png
└── xgboost_confusion_matrix.png
## Future Improvements

Potential enhancements include:

* Hyperparameter Tuning using GridSearchCV
* Cross Validation
* SHAP Explainability
* SMOTE for Class Imbalance Handling
* Streamlit Deployment
* Real-Time Prediction API

---

## Key Learnings

Through this project:

* Built an end-to-end machine learning pipeline
* Performed exploratory data analysis
* Compared multiple classification algorithms
* Evaluated models using industry-standard metrics
* Interpreted model predictions using feature importance
* Derived business insights from customer behavior data

---

## Author

**[Divyanshu Tomer]**

