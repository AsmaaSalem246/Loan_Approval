# Loan Approval Prediction

A machine learning project that predicts whether a customer's loan application will be **Approved** or **Rejected** based on demographic, financial, and credit-related features.

This project includes:
- Logistic Regression and Decision Tree models
- Regularization & hyperparameter tuning with GridSearchCV
- Full report (1–2 pages) summarizing methodology and results

---

## 📌 Dataset Description

The dataset contains **4,269 records** and 13 columns.

### 🔹 Demographic Features
- `no_of_dependents`
- `education`
- `self_employed`

### 🔹 Financial Features
- `income_annum`
- `loan_amount`
- `loan_term`
- `cibil_score`

### 🔹 Asset Features
- `residential_assets_value`
- `commercial_assets_value`
- `luxury_assets_value`
- `bank_asset_value`

### 🎯 Target Variable
- `loan_status` (Approved / Rejected)

---

## 📌 Methodology

### 1. Preprocessing
- Handle categorical features with Label Encoding
- Standardize numerical features where needed
- Train/test split (70/30)

### 2. Models Used
#### ✔ Logistic Regression
- Applied **L1/L2 regularization**
- Tuned using **GridSearchCV**

#### ✔ Decision Tree Classifier
- Tuned hyperparameters:
  - `max_depth`
  - `min_samples_split`
  - `min_samples_leaf`

### 3. Hyperparameter Tuning
- Performed using GridSearchCV with cross-validation

---

## 📌 Results

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 0.9222 |
| Decision Tree | 0.9655 |
| Logistic Regression (GridSearchCV) | 0.9504 |
| Decision Tree (GridSearchCV) | **0.9931** |

➡ **Best Model:** Decision Tree with GridSearchCV  
It captures non-linear relationships and gives the highest accuracy.

---

