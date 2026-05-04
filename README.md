# 🏦 Loan Default Prediction

## 📌 Project Overview

This project aims to predict whether a customer will **default on a loan** based on their financial and personal information. It uses machine learning techniques to help identify high-risk customers and support better decision-making.

---

## 🎯 Objective

To build a classification model that can:

* Predict loan default (Yes/No)
* Minimize risk by identifying potential defaulters
* Provide insights into factors influencing default

---

## 📊 Dataset Features

The dataset includes variables such as:

* Customer Age
* Income
* Home Ownership
* Employment Duration
* Loan Intent
* Loan Grade
* Interest Rate
* Credit History Length

---

## ⚙️ Data Preprocessing

* Handled categorical variables using:

  * One-Hot Encoding (nominal features)
  * Label Encoding (ordinal features)
* Converted binary variables to numeric (0/1)
* Removed irrelevant features (e.g., customer_id)
* Checked correlations using heatmap

---

## 🤖 Models Used

### 1. Logistic Regression

* Applied feature scaling
* Handled class imbalance using `class_weight='balanced'`
* Result:

  * Accuracy: ~85%
  * High recall for default class

---

### 2. Random Forest Classifier (Final Model)

* Tuned hyperparameters to reduce overfitting:

  * max_depth = 10
  * min_samples_split = 5
  * min_samples_leaf = 2
* Result:

  * Accuracy: **94%**
  * Recall (Default): **96%**
  * Balanced and stable model

---

## 📈 Model Evaluation

### Confusion Matrix Insights:

* Very few missed defaulters
* Slight trade-off with false positives

### Key Metrics:

* Precision (Default): 0.79
* Recall (Default): 0.96
* F1 Score: 0.87

---

## 🔍 Feature Importance

Random Forest helped identify key drivers of default:

* Loan-to-income ratio
* Interest rate
* Credit history length

---

## 💡 Key Insights

* Customers with higher loan burden are more likely to default
* Credit history plays a major role in risk assessment
* Model prioritizes catching defaulters (high recall)

---

## 🚀 Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

## 🎤 Conclusion

This project demonstrates a complete ML workflow:

* Data preprocessing
* Feature engineering
* Model training & evaluation
* Business insights

The final model achieves strong performance and can be used for **risk assessment in financial systems**.

---

## 📬 Future Improvements

* Hyperparameter tuning (GridSearchCV)
* Try advanced models (XGBoost)
* Deploy model using Flask/Streamlit

---
