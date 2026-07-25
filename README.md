# codealpha_tasks
Completed internship tasks at CodeAlpha.
# ❤️ Heart Disease Prediction

## 📌 Overview
This project uses machine learning to predict whether a patient is likely to have 
heart disease based on clinical and health data. Built as part of my CodeAlpha 
Machine Learning internship.

## 🎯 Objective
Predict the presence of heart disease in a patient using health parameters such as 
age, cholesterol level, blood pressure, chest pain type, and other clinical features.

## 📊 Dataset
- **Source:** Kaggle — [Heart Disease Prediction](https://www.kaggle.com/datasets/rishidamarla/heart-disease-prediction/data)
 
- **Records:** `17 Rows`

- **Features:** `270 columns`, including age, sex, chest pain type, blood pressure, cholesterol, exercise angina, max heart rate, etc.

- **Target variable:** Presence (1) or absence (0) of heart disease

## 🛠️ Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib
- Google Colab

## 🔍 Approach
1. **Data Cleaning** — checked for duplicates and missing values.

2. **Exploratory Data Analysis (EDA)** — visualized feature distributions, dorminating attributes, column analysis, and correlations with heart disease outcome.

3. **Feature Engineering/Selection** — Feature encoding for prediction, standard scaling, binning for continous feature like `Age` to categorical, One Hot Encoding for binned age.

4. **Model Building** — trained and compared multiple models:
   - Model 1. Random Forest
   - Model 2. XGBoost
   - Model 3. Logistic Regression
   - Model 4. SVM
   
5. **Model Evaluation** — compared models using accuracy, precision, recall,  F1-score, and AUC_ROC

## 📈 Results
| Model | Accuracy |
|---|---|
| Random Forest | 88% |
| XGBoost | 78% |
| Logistic regression | 93% |
| SVM | 93% |

**Best performing model:** Logistic Regression with 93% AUC Score

## 🚀 How to Run
1. Clone the repo: 🐙 [Git Clone](https://github.com/Melchizedek-Madaki/codealpha_tasks.git)

2. Open `Heart_Disease_Prediction.ipynb` in Jupyter or Google Colab

3. Install dependencies:
4. ## Requirements

- python >= 3.10.1
- Jupyter notebook/Google colab

### System Requirements

- **Memory:** 4GB RAM minimum, 8GB recommended

## Installation

### Load Dataset
```bash
from kagglehub import kh
```
### Dependencies
```bash
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
```
### Model Algorithms
```bash
from sklearn.ensemble import RandomForestClassifier
from xgboost import XGBClassifier
from sklearn.linear_model import Logistic Regression
from svm import SVC
```

### Feature Engineering
```bash
from sklearn.preprocessing import OHE
from sklearn.preprocessing import StandardScaler
```

### Evaluation Metrics
```bash
from sklearn.metrics import (
    accuracy_score, precision_score,
    recall_score, f1_score,
    classification_report, confusion_matrix, ConfusionMatrixDisplay, roc_curve, roc_auc_score
)
```

## 📁 Files in this folder
- `Heart_Disease_Prediction.ipynb` — main notebook
- `README.md` — this file

## 🙋 Author
**Melchizedek Madaki**  
CodeAlpha Machine Learning Internship

