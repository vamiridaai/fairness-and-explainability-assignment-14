# Fairness and Explainability in Machine Learning

This project demonstrates how to build, evaluate, and interpret a machine learning model with a strong focus on **fairness**, **ethics**, and **explainability**. The goal is to assess not only predictive performance but also potential bias and transparency in model decisions.

---

##  Project Overview

- **Objective**: Predict whether an individual earns more than $50K per year
- **Model**: Logistic Regression
- **Dataset**: Adult Census Income Dataset (UCI Machine Learning Repository)
- **Sensitive Attribute**: Gender (`sex`)
- **Key Focus Areas**:
  - Model performance evaluation
  - Fairness analysis across demographic groups
  - Explainability using SHAP and LIME
  - Ethical considerations and bias assessment

---

##  Dataset

**Adult Census Income Dataset**
- Source: UCI Machine Learning Repository
- Target Variable: `income` (>50K or ≤50K)
- Sensitive Attribute: `sex` (Male / Female)
- Features include age, education, work class, occupation, race, hours worked, and more.

---

##  Model Description

- Logistic Regression implemented using scikit-learn
- Data preprocessing includes:
  - Standardization of numerical features
  - One-hot encoding of categorical features
- A pipeline is used to prevent data leakage

---

##  Fairness Analysis

Fairness is evaluated using the **Fairlearn** library with the following metrics:
- Selection Rate
- False Positive Rate
- True Positive Rate

Metrics are compared across gender groups using `MetricFrame` and visualized using bar plots.

---

##  Explainability

- **SHAP**:
  - Global feature importance (summary plot)
  - Local explanations (waterfall plot)
- **LIME**:
  - Local, human-readable explanations for individual predictions

These methods improve transparency and trust in model predictions.

---

##  Setup Instructions

### Option 1: Run on Google Colab (Recommended)
1. Open Google Colab
2. Upload `Fairness_and_Explainability_Assignment_FINAL.ipynb`
3. Run **Runtime → Run all**
4. All required libraries will be installed automatically

### Option 2: Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/vamiridaai/fairness-and-explainability-assignment-14.git
