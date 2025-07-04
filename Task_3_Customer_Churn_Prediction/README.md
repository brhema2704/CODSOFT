# 💼 Customer Churn Prediction - CODSOFT Internship Task

This project is part of my **Machine Learning Internship at CodSoft**, where I built a predictive model to identify whether a customer is likely to churn (leave the service) based on historical customer data.


## 📌 Objective

Develop a machine learning model that predicts customer churn using customer demographic and usage data. This helps subscription-based businesses retain valuable customers by identifying churn risk in advance.


## 📁 Dataset Overview

Dataset: `Churn_Modelling.csv`
Records: 10,000
Target Variable: `Exited` (1 = churned, 0 = retained)

### Key Features Used:
* `CreditScore`, `Geography`, `Gender`, `Age`, `Tenure`, `Balance`
* `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary`


## ⚙️ Models Implemented

 Model                  Accuracy  Precision (Churn)  Recall (Churn)  F1-Score (Churn) 

 Logistic Regression    80.75%    0.60               0.16            0.25             
 Random Forest          86.40%    0.78               0.46            0.58             
 Gradient Boosting      86.75%    0.79               0.48            0.59             


## 🔍 Insights & Observations

* ✅ **Random Forest** and **Gradient Boosting** significantly outperform Logistic Regression in identifying churned customers.
* ⚠️ **Logistic Regression** struggles to recall actual churners, identifying only 16% of them correctly, despite high accuracy overall. This is due to class imbalance.
* 📈 **Gradient Boosting** had the **highest F1-score** for the churn class (0.59), making it the most balanced performer between precision and recall.
* 🎯 All models achieved high accuracy because non-churned customers dominate the dataset. Therefore, **recall and F1-score for class `1` (churn)** are more important than accuracy alone.


## 🧠 Lessons Learned

* Importance of using metrics beyond accuracy for imbalanced classification problems.
* Ensemble methods like Random Forest and Gradient Boosting are powerful for tabular data and churn prediction tasks.
* Feature encoding, class balance awareness, and model selection play a crucial role in business-critical ML applications.


## 📊 Confusion Matrix (Visuals)

Each model included a confusion matrix to evaluate prediction distribution. Gradient Boosting showed the best trade-off between false positives and false negatives.


## 🚀 Technologies Used

Python 🐍
Pandas, NumPy
Scikit-learn
Matplotlib, Seaborn

