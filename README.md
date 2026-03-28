# 💳 Loan Default Prediction

Machine Learning Models for Loan Granting Decisions

---

## 🔧 Tech Stack

Classification Models · Logistic Regression · Random Forest · XGBoost · Imbalanced Data Handling · Undersampling · SMOTE · Python (Scikit-learn, XGBoost)

---

## Project Overview

### Problem

Accurate prediction of credit default is essential for financial institutions.
However, default events are relatively rare, leading to **strong class imbalance** and making reliable prediction challenging.

---

### Approach

Multiple classification models were implemented and compared, with a specific focus on handling class imbalance through:

* Baseline modeling on imbalanced data
* Random undersampling
* Hyperparameter tuning
* SMOTE (synthetic oversampling)

---

### Key Outcomes

* Baseline models achieved high accuracy (~80%) but **very low recall (~0.07)**
* Undersampling significantly improved recall (**up to ~0.67**)
* **XGBoost consistently delivered the best performance**
* Hyperparameter tuning produced limited improvements
* SMOTE negatively affected performance, particularly for XGBoost

---

## 🏦 Business Context

Credit default prediction supports:

* Risk assessment
* Credit approval decisions
* Portfolio management

Misclassification has asymmetric consequences:

* Undetected defaults → financial losses
* False positives → missed lending opportunities

---

## ❓ Problem Statement

Can machine learning models effectively predict credit defaults in the presence of strong class imbalance?

---

## 📊 Dataset

* Loan application dataset
* Target variable: default vs non-default
* Default rate: <20%
* Key challenge: imbalanced classes

---

## 🧠 Methodology

### Models

* Logistic Regression
* Random Forest
* XGBoost

### Experimental Design

* **Case 1:** Imbalanced data (baseline)
* **Case 2:** Random undersampling
* **Case 3:** Tuned models on undersampled data
* **Case 4:** SMOTE (oversampling)

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score
* ROC AUC

---

## 📈 Results

* Imbalanced data → high accuracy, very low recall
* Undersampling → substantial recall improvement with reduced accuracy
* Hyperparameter tuning → marginal gains
* SMOTE → inconsistent results and performance degradation

Best performance was obtained with **XGBoost on undersampled data**.

---

## 🧠 Key Insight

Accuracy alone is not an adequate metric in imbalanced settings.
**Recall is critical**, as correctly identifying default cases is more valuable than minimizing false positives.

---

## 🚀 Future Improvements

* Cost-sensitive learning approaches
* Enhanced feature engineering
* Ensemble and stacking methods
* Threshold optimization based on business objectives

---

If you want, next step can be:

* even more minimal (1-page ultra-compact version), or
* slightly more “academic tone” to perfectly match the report wording.