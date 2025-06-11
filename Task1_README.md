# 📊 Customer Churn Prediction for a Telecom Company

## 📝 Project Overview

This project aims to predict customer churn for a telecom company using historical customer data. The main goal is to identify customers likely to leave, enabling proactive retention strategies.

Dataset: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

## 🧠 Objectives

* Perform Exploratory Data Analysis (EDA)
* Clean and preprocess the data
* Engineer relevant features
* Train multiple classification models
* Evaluate model performance using key metrics
* Recommend a final model for deployment

---

## 📂 Folder Structure

```
├── data/
│   └── Telco-Customer-Churn.csv
├── notebook/
│   └── Task_1_Customer_Churn_Prediction.ipynb
├── models/
│   └── (trained models can be saved here)
├── task1_README.md
```

---

## 🧪 Steps Performed

### 1. 📊 Exploratory Data Analysis (EDA)

* Data overview and inspection
* Univariate and bivariate visualizations
* Correlation analysis

### 2. 🛠️ Data Cleaning

* Converted `TotalCharges` to float
* Handled missing values and duplicates
* Standardized categorical values

### 3. 🧬 Feature Engineering

* Encoded binary and multi-class categorical variables
* Created `TenureGroup` bins
* Added `NumAdditionalServices` feature

### 4. 🚂 Model Training

Models Trained:

* Logistic Regression
* Random Forest Classifier
* Support Vector Classifier (SVC)
* XGBoost Classifier
* LightGBM Classifier

All models were trained on a stratified train/test split with standard scaling applied to numerical features.

### 5. 📈 Model Evaluation

Metrics used:

* Accuracy
* Precision
* Recall
* F1-Score
* AUC-ROC
* Confusion Matrix
* ROC Curves

---

## 🏆 Final Model Recommendation

**🎯 LightGBM Classifier**

* Best trade-off between precision and recall
* High AUC and strong performance on imbalanced data
* Recommended for deployment to score churn risk daily

---

## 📌 Key Insights

* Customers on **Month-to-month contracts** are most likely to churn.
* Low **tenure** and **TotalCharges** are strongly linked to churn.
* Lack of **OnlineSecurity** and **TechSupport** is a churn signal.
* **Electronic check** users churn more than those using bank or credit card transfers.

---

## 💡 Suggested Actions

* Offer incentives to switch to long-term contracts
* Create onboarding programs for new customers
* Promote high-retention services like security and tech support
* Use the trained LightGBM model for churn risk scoring

---

## 📚 Requirements

* Python 3.7+
* Libraries:

  * pandas
  * numpy
  * seaborn
  * matplotlib
  * scikit-learn
  * xgboost
  * lightgbm

---

## 📧 Contact

For questions or improvements, feel free to reach out or submit a pull request.
email: nasir.aliqureshi555@gmail.com