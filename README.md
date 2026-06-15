# Credit Risk Prediction

## Project Overview

This project aims to predict whether a borrower is likely to default on a loan using machine learning techniques. The model is developed using demographic, financial, and loan-related information to support better credit risk assessment.

## Business Problem

Financial institutions face significant losses when borrowers fail to repay loans. Traditional credit assessment methods may not fully capture borrower risk profiles.

The objective of this project is to build a predictive model that can identify high-risk borrowers and support more informed lending decisions.

---

## Dataset Information

Dataset: Credit Risk Dataset

Target Variable:

* loan_status

  * 0 = Non-Default
  * 1 = Default

Features include:

* Borrower age
* Income
* Employment length
* Home ownership status
* Loan amount
* Loan intent
* Loan grade
* Interest rate
* Credit history length
* Loan-to-income ratio

---

## Project Workflow

1. Data Understanding
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing
4. Feature Engineering
5. Model Development
6. Model Evaluation
7. Feature Importance Analysis
8. Business Insights
9. Business Recommendations

---

## Exploratory Data Analysis

Key findings:

* Approximately 21.8% of borrowers defaulted.
* Borrowers with lower income showed higher default rates.
* Higher loan amounts were associated with increased risk.
* Loan-to-income ratio showed a strong relationship with default behavior.
* Interest rate and loan grade were important indicators of credit risk.

---

## Data Preprocessing

The following preprocessing steps were applied:

* Missing value handling using median imputation
* One-hot encoding for categorical variables
* Train-test split (80:20)
* Feature scaling for Logistic Regression

---

## Model Development

Two machine learning models were developed:

### Logistic Regression

* Accuracy: 86.74%
* Precision: 76.78%
* Recall: 56.26%
* F1 Score: 64.94%
* ROC-AUC: 86.93%

### Random Forest

* Accuracy: 93.23%
* Precision: 95.54%
* Recall: 72.36%
* F1 Score: 82.35%
* ROC-AUC: 93.11%

---

## Model Evaluation

Random Forest outperformed Logistic Regression across all evaluation metrics and was selected as the final model.

| Model               | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| Logistic Regression | 86.74%   | 76.78%    | 56.26% | 64.94%   | 86.93%  |
| Random Forest       | 93.23%   | 95.54%    | 72.36% | 82.35%   | 93.11%  |

---

## Feature Importance

Top predictive features:

1. Loan Percent Income
2. Person Income
3. Loan Interest Rate
4. Loan Amount
5. Home Ownership Status
6. Employment Length

These variables play a major role in determining borrower default risk.

---

## Business Insights

* Borrowers with high loan-to-income ratios are more likely to default.
* Lower-income borrowers exhibit higher repayment risk.
* Larger loan amounts increase default probability.
* Higher interest rates are associated with higher risk.
* Renters tend to have higher credit risk compared to homeowners.

---

## Business Recommendations

* Implement stricter screening for applicants with high loan-to-income ratios.
* Introduce risk-based loan approval policies.
* Adjust loan limits according to borrower income levels.
* Use machine learning-based credit scoring to support lending decisions.
* Prioritize monitoring of high-risk borrower segments.

---

## Conclusion

This project successfully developed a credit risk prediction model using machine learning techniques.

The Random Forest model achieved the best performance with:

* Accuracy: 93.23%
* ROC-AUC: 93.11%

The model can help financial institutions identify high-risk borrowers, improve lending decisions, and reduce potential credit losses.

---

## Project Structure

credit-risk-prediction/

├── data/

│ └── credit_risk_dataset.csv

├── credit_risk_prediction.ipynb

├── README.md

└── requirements.txt

---

## Requirements

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* jupyter
