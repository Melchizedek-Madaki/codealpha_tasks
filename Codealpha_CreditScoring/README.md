# 💳 Credit Scoring Prediction

## 📌 Overview
This project uses machine learning to predict an individual's creditworthiness 
based on their past financial data. Built as part of my CodeAlpha Machine Learning
internship.

## 🎯 Objective
Predict an individual's creditworthiness using past financial data.

## 📊 Dataset
- **Source:** [Kaggle Data Source](https://www.kaggle.com/datasets/bbjadeja/predicting-creditworthiness)
- **Records:** `Rows = 1000`
- **Features:** `Features/Columns = 21`
  
- Target variable: Good = 1, Bad = 0

## 🛠️ Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Google Colab

## 🔍 Approach
1. **Data Cleaning** — handled missing values, checked for outliers/duplicates
2. **Exploratory Data Analysis (EDA)** — Univariate, and Bivariate Analysis, and log-transform for skewness

3. **Feature Engineering** —  One Hot Encoding, and Label Encoding

4. **Model Building** — trained and compared:
   - Logistic regression
   - Random Forest
   - XGBoost
   - SVC
5. **Model Evaluation** — compared using accuracy, precision, recall, F1-score, and AUC-ROC, and Confusion Matrix

## 📈 Results
| Model |Class-weighted Recall|
|---|---|
| Logistic Regression | 68% |
| Random Forest | 30% |
| XGBoost | 53% |
| SVC | 75% |

**Best performing model:** SVC with 75% recall

## 🚀 How to Run
1. Clone the repo: [Clone Repo](https://github.com/Melchizedek-Madaki/codealpha_tasks.git)
2. Open `Predicting_CreditWorthiness.ipynb` in Jupyter or Google Colab
3. Install dependencies:

### Production Build

```bash
install numpy as np
install pandas as pd
from sklearn.metrics import (
    precision_score, recall_score, f1_score,
    roc_auc_score, confusion_matrix, classification_report
)

```

# Algorithms
```bash
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from svm import SVC
from xgboost import XGBClassifier
```

4. Run all cells

## 📁 Files in this folder
- `Credit_Scoring.ipynb` — main notebook
- `README.md` — this file

## 🙋 Author
**Melchizedek Madaki**  
CodeAlpha Machine Learning Internship
