# Codealpha Credit Scoring — Predicting Creditworthiness

This directory contains an exploratory analysis and modeling notebook for predicting creditworthiness using a Kaggle dataset. The notebook performs EDA, data cleaning, feature inspection, and initial modeling to classify applicants as `good` or `bad` credit risks.

## Files

- `Predicting_Creditworthiness.ipynb` — Jupyter/Colab notebook with the full analysis, visualizations and modeling pipeline.

## Dataset

The notebook uses the "Predicting Creditworthiness" dataset from Kaggle:

- https://www.kaggle.com/datasets/bbjadeja/predicting-creditworthiness

In the notebook the dataset is downloaded using `kagglehub`:

```python
data_path = kh.dataset_download('bbjadeja/predicting-creditworthiness')
df = pd.read_excel(data_path + '/CreditWorthiness.xlsx')
```

If you prefer to download the dataset manually, download the Excel file and place it in the same directory or update the notebook to point to the local file path.

## Quick overview

- Rows: 1000
- Columns: 21
- Target: `Credit Score` (values: `good`, `bad`) — class distribution: 700 good / 300 bad (approx 70/30)
- Notable columns: checking account balance (`Cbal`), credit duration (`Cdur`), loan amount (`Camt`), savings balance (`Sbal`), employment duration (`Edur`), age, number of existing credits (`NumCred`), etc.

The notebook includes an initial EDA using `skimpy`, checks for missing values and duplicates, basic correlations for numeric features, and discusses class imbalance.

## How to run

Option 1 — Colab (recommended):

- Open the notebook in Colab (the notebook includes a Colab badge linking to the GitHub copy):

  https://colab.research.google.com/github/Melchizedek-Madaki/codealpha_tasks/blob/main/Codealpha_CreditScoring/Predicting_Creditworthiness.ipynb

- Run the cells. The notebook uses `kagglehub` in the first steps to download the dataset into the Colab cache.

Option 2 — Local

1. Install dependencies (example):

```bash
pip install pandas numpy openpyxl skimpy kagglehub
```

2. Download the Kaggle dataset (either with the Kaggle website or the Kaggle CLI) and place `CreditWorthiness.xlsx` in an accessible path.

3. Open `Predicting_Creditworthiness.ipynb` and update the `data_path` / loading cell to point to the local file.

## Requirements

The notebook uses the following Python packages (not exhaustive):

- pandas
- numpy
- skimpy
- kagglehub (used in the notebook to download the dataset)
- openpyxl (for reading Excel files)

Add more packages as needed if you run into import errors.

## Notes & next steps

- The dataset has a moderate class imbalance (70/30). Consider evaluation metrics beyond accuracy (precision, recall, F1, AUC) and resampling techniques or class-weighted models.
- The notebook currently performs EDA and basic checks. You can extend it with feature engineering, encoding categorical variables, model training (cross-validation), and explainability (SHAP/LIME).

## Contact

Repository: https://github.com/Melchizedek-Madaki/codealpha_tasks

If you want the README expanded (run instructions, badges, or a requirements.txt), tell me what you'd like and I will add it.
