# Digital-Marketing-Campaigns-Conversion-Prediction
End-to-end conversion prediction system using XGBoost, SMOTE, and SHAP to optimize digital marketing targeting. Includes threshold tuning, decision intelligence engine, probability calibration, and profit-based evaluation to improve ROAS and reduce wasted ad spend.
# 🎯 Conversion Intelligence Engine  
### Profit-Optimized Customer Targeting Using XGBoost + SHAP

An end-to-end machine learning system for predicting customer conversions and optimizing digital marketing spend using probability calibration, threshold optimization, and explainable AI.

---

## 📌 Executive Summary

This project builds a production-ready conversion prediction system that helps marketing teams:

- Predict high-probability converters
- Reduce wasted ad spend
- Optimize targeting using profit-aware thresholds
- Generate explainable predictions with SHAP

Instead of optimizing only for accuracy, this system aligns model decisions with business ROI and ROAS objectives.

---

## 🧠 Problem Statement

Digital marketing campaigns often suffer from:

- Class imbalance (few converters)
- Budget inefficiencies
- Poor probability calibration
- Lack of model explainability

This project addresses these challenges using:

- Stratified cross-validation
- SMOTE (imbalance handling)
- F1-based and profit-based threshold optimization
- SHAP explainability
- Persona-driven targeting strategy

---

## 🏗️ Project Architecture

```
Raw Data
   ↓
EDA & Feature Engineering
   ↓
Preprocessing Pipeline (Scaling + Encoding)
   ↓
SMOTE (inside CV only)
   ↓
Model Training (XGBoost selected)
   ↓
Threshold Optimization
   ↓
Decision Intelligence Engine
   ↓
Business Metrics & SHAP Explainability
```

---

## 🤖 Models Evaluated

| Model | Purpose |
|-------|---------|
| Logistic Regression | Baseline interpretability |
| Random Forest | Non-linear ensemble |
| Gradient Boosting | Boosted tree model |
| XGBoost | Final selected model |

---

## 📊 Evaluation Metrics

Because conversion prediction is imbalanced, we prioritized:

- F1 Score
- Precision
- Recall
- ROC-AUC
- Calibration curves
- Precision–Recall curves

Accuracy was not used as the primary selection metric.

---

## 💰 Business Optimization Layer

### 🎯 F1-Optimal Threshold Search

Instead of using a default 0.5 threshold, the system:

- Searches thresholds from 0.1–0.9
- Identifies the F1-optimal threshold
- Evaluates average ad spend per predicted converter

---

## 🔍 Explainable AI (SHAP)

To ensure transparency and interpretability, we used SHAP (SHapley Additive exPlanations).

- Global feature importance
- Summary plots
- Individual waterfall explanations

---

## 📁 Project Structure

```
conversion-prediction/
│
├── data/
├── notebooks/
├── outputs/
├── models/
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/conversion-prediction.git
cd conversion-prediction
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. Open Jupyter Notebook  
2. Run `conversion_prediction.ipynb`  
3. Outputs will be generated inside `/outputs`  
4. Final model saved inside `/models`

---

## 📌 Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- SHAP
- Matplotlib
- Seaborn

---

Built a production-grade conversion intelligence system using XGBoost, SMOTE, SHAP explainability, and profit-aware threshold optimization to improve ROAS and marketing targeting efficiency.

---
