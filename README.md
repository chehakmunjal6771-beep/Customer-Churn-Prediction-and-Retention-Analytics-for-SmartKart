# 🛒 SmartKart — Customer Churn Prediction & Retention Analytics

## 📌 Project Overview

SmartKart Customer Churn Prediction is an end-to-end machine learning project designed to identify customers who are likely to churn and help the retention team take proactive action.

The project demonstrates a complete **data-to-decision ML pipeline**, starting from a deliberately messy customer dataset and progressing through data cleaning, outlier treatment, feature selection, model development, evaluation, interpretation, and customer-level churn risk scoring.

## 🎯 Business Objective

The primary objective is to predict whether a customer is likely to churn based on key customer attributes and identify the major factors influencing churn.

The resulting churn-risk analysis can help SmartKart:

* Identify high-risk customers
* Prioritise retention efforts
* Understand key churn drivers
* Support targeted customer engagement
* Reduce potential customer loss

## 📊 Dataset

The dataset contains **100 customer records** with the following variables:

| Feature         | Description                              |
| --------------- | ---------------------------------------- |
| `Customer_ID`   | Unique customer identifier               |
| `Age`           | Customer age                             |
| `Monthly_Spend` | Customer's monthly spending              |
| `Complaints`    | Number of customer complaints            |
| `Churn`         | Target variable: 1 = Churn, 0 = No Churn |

The dataset intentionally contains real-world data-quality issues such as missing values, duplicate records, invalid entries, inconsistent formatting, and outliers.

## 🔄 Machine Learning Pipeline

The project follows a structured **15-step ML workflow**:

1. Data Collection
2. Data Understanding & Inspection
3. Data Cleaning
4. Outlier Detection & Treatment
5. Feature Selection
6. Target Variable Definition
7. Target Encoding
8. Train-Test Split
9. Feature Standardisation
10. Model Building
11. Model Training
12. Prediction
13. Model Evaluation
14. Model Interpretation
15. Business-Ready Final Output

## 🤖 Model

**Logistic Regression** is used because churn is a binary classification problem and the model provides interpretable coefficients and churn probabilities.

Selected predictive features:

* Age
* Monthly Spend
* Complaints

`Customer_ID` is excluded from modelling because it is an identifier rather than a predictive feature.

## 📈 Model Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

Recall is particularly important for this business problem because identifying actual churners is critical for proactive retention.

## 🔍 Business Insights

Model coefficients are analysed to understand the factors associated with churn.

The analysis highlights:

* **Complaints:** Higher complaints are associated with increased churn risk.
* **Monthly Spend:** Higher monthly spending is associated with lower churn risk.
* **Age:** Shows a comparatively weaker relationship with churn.

These insights can help SmartKart focus retention efforts on customers experiencing service issues while protecting valuable customer relationships.

## 📁 Project Output

The pipeline generates:

**`smartkart_churn_risk_report.csv`**

The report provides customer-level information including:

* Customer ID
* Customer attributes
* Actual churn
* Predicted churn
* Churn probability
* Risk label

Customers are ranked by churn probability so the retention team can prioritise the highest-risk customers first.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab
* Logistic Regression

## 🚀 How to Run

1. Download or clone the repository.
2. Open the `.ipynb` notebook in Google Colab or Jupyter Notebook.
3. Upload `SmartKart_dirty_100_rows.csv`.
4. Run the notebook cells sequentially.
5. Review the model evaluation and business insights.
6. Generate the final `smartkart_churn_risk_report.csv`.

## 💼 Business Value

This project demonstrates how machine learning can move beyond prediction to support **data-driven customer retention decisions**. It combines data-quality management, interpretable predictive modelling, risk scoring, and actionable business insights into a single workflow.

---

### 👤 Project

**SmartKart Customer Churn Prediction & Retention Analytics**

*End-to-end machine learning pipeline for customer churn prediction and retention decision support.*
