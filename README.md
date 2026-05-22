# Credit Risk Prediction – Financial Machine Learning Project

## Business Problem

Financial institutions must evaluate the risk of loan applicants to minimize financial losses from defaults. 

This project builds a machine learning model to classify customers as **high-risk** or **low-risk**, helping improve lending decisions and reduce credit risk exposure.

---

## Dataset

The project uses the German Credit dataset, which includes:
- Customer demographics (Age, Job, Gender)
- Financial attributes (Checking account, Saving accounts)
- Loan details (Credit amount, Duration, Purpose)

---

## Approach

### Data Preparation
- Removed unnecessary index column
- Handled missing values in financial variables
- Encoded categorical variables using one-hot encoding

### Model
- Random Forest Classifier was used due to its strong performance on tabular data and ability to capture non-linear relationships

---

## Model Performance

- **Accuracy:** 69%
- **Recall (High-Risk customers):** 83% ✅
- **Recall (Low-Risk customers):** 48%

### Interpretation
The model performs well in identifying high-risk customers, which is critical in financial applications since failing to detect risky borrowers can result in financial losses.

---

## Feature Importance

The most important features influencing prediction were:
- Credit amount
- Loan duration
- Age

### Insight
- Larger loans increase default risk
- Longer loan duration increases uncertainty and risk
- Age may reflect financial stability and repayment capability

---

## Key Insights

- The model prioritizes identifying high-risk customers, which aligns with financial risk management strategies
- Financial variables such as checking and saving accounts contribute to predicting credit risk
- There is a trade-off between identifying risky customers and correctly classifying safe customers

---

## Model Tuning Insights

Increasing model complexity (e.g., deeper trees and more estimators) led to lower test accuracy, indicating **overfitting**.

A simpler model provided better generalization performance.
