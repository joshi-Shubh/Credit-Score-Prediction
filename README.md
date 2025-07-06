# 💳 Credit Score Prediction – Bank GoodCredit

## 🏦 Business Case

Bank **GoodCredit** wants to predict credit scores for their current credit card customers. The goal is to determine a customer’s **creditworthiness** and reduce **credit default risk** by identifying high-risk profiles early using predictive analytics.

---

## 📁 Dataset Information

The project uses a multi-table database with the following components:

### 🔹 `Cust_Account`
- Customer’s historical accounts and payment data.
- Credit utilization, payment timelines, and account age.

### 🔹 `Cust_Demographics`
- Obscured demographic features due to privacy policy.
- Includes age, income, location, and other behavioral indicators.

### 🔹 `Cust_Enquiry`
- Historical inquiry data like:
  - Purpose of credit inquiries
  - Requested credit amount
  - Frequency and type of enquiries

---

## 🎯 Target Variable: `Bad_label`

| Label | Description                    |
|--------|--------------------------------|
| `0`    | Customer has **Good** credit history |
| `1`    | Customer has **Bad** credit history (30+ days past due) |

---

## 💡 Domain Analysis

Credit analysis evaluates a customer's **risk of default** based on:
- Financial records
- Enquiry behavior
- Account usage history

This project helps answer:
> Which features most impact a customer's default risk?  
> Can we reliably classify a customer as risky or safe?

By integrating account, demographic, and enquiry data, we can build robust models to assess risk and support better lending decisions.

---

## 🧪 ML Pipeline

### 📊 EDA & Feature Engineering
- Multi-table merging
- Handling missing data
- Domain-specific variable transformation

### 🤖 Machine Learning Models
- Logistic Regression
- Random Forest
- XGBoost Classifier etc..
- Evaluation with:
  - Confusion Matrix
  - Precision-Recall



---

## ✅ Results
- Top Risk Drivers:
  - Enquiry frequency
  - Outstanding amount
  - Credit utilization

---

## 🔧 Requirements

```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
