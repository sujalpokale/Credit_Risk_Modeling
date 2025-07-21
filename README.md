# 💳 Credit Risk Modeling

This project focuses on predicting the **probability of loan default** by using a borrower’s financial and credit history. The model is designed to help lenders assess risk before issuing a loan.

---

## 🎯 Objective

Build a predictive model that can accurately estimate the likelihood that a customer will **default on a loan**, using real-world credit data and financial indicators.

---

## 🧠 Models Used

- **Logistic Regression** – interpretable baseline model  
- **LightGBM** – gradient boosting model for high performance  
- **Scorecard-style approach** – using feature importance for interpretability

---

## 🧾 Dataset

**Dataset Used**:  
📊 [Default of Credit Card Clients Dataset (UCI ML Repository)](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)

### Key Features:
- Demographics (age, gender, education, marital status)
- Credit limit and usage
- Payment history over 6 months
- Default label: `default.payment.next.month` (0 = no default, 1 = default)

---

## 🛠 Feature Engineering

- `credit_utilization`: bill amount relative to credit limit  
- `repayment_ratio`: total payment / total bill  
- Aggregated bill and payment behavior over multiple months  
- Categorical encoding (LabelEncoder, one-hot)  
- Standard scaling on continuous variables  

---

## ⚖️ Imbalance Handling

- Used **SMOTE (Synthetic Minority Over-sampling Technique)** to balance default vs non-default classes.

---

## 📈 Model Evaluation

- **Classification Report** (Precision, Recall, F1-score)  
- **AUC Score** for model performance  
- **Feature Importance** from LightGBM (scorecard-style insight)

---

## 🧰 Libraries Used

- `pandas`, `numpy`
- `scikit-learn`
- `lightgbm`
- `imbalanced-learn` (for SMOTE)
- `matplotlib` / `seaborn` (optional for visualization)

