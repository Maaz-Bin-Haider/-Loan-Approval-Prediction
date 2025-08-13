# 🏦 Loan Approval Prediction

## 📌 Project Overview
This project predicts whether a loan application will be approved based on applicant details.  
It was completed as part of my **Elevvo Internship** task, focusing on binary classification and handling imbalanced data.

## 📂 Dataset
- **Source:** Loan Approval Prediction Dataset (Kaggle)
- **Target Variable:** `loan_status` (0 = Not Approved, 1 = Approved)
- **Shape:** Rows × Columns depend on the dataset version.
- **Features:** Applicant demographics, income, loan details, and asset values.

## 🛠️ Steps Performed
1. **Load Dataset** using Pandas.
2. **Handle Missing Values**:
   - For categorical columns → filled with **mode**.
   - For numeric columns → filled with **median**.
3. **Encode Categorical Features** using **Label Encoding**.
4. **Split Features & Target**:
   - Dropped `loan_id` (identifier).
   - `loan_status` used as target `y`.
5. **Check Class Imbalance** and applied **SMOTE** to balance the classes.
6. **Train/Test Split** to evaluate model performance on unseen data.
7. **Train Models**:
   - Logistic Regression
   - Decision Tree Classifier
8. **Evaluate Models** using:
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix

## 📊 Tools & Libraries
- **Python**
- **pandas**
- **matplotlib**
- **seaborn**
- **numpy**
- **scikit-learn**
- **imbalanced-learn** (SMOTE)
