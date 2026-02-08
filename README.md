# Churn Prediction

## Overview
This project builds and compares multiple classification models to predict customer churn using the Telco Customer Churn dataset. The notebook walks through data loading, cleaning, exploratory analysis, feature engineering, model training, and evaluation.

## Dataset
The notebook expects the Telco dataset at:

`datasets/WA_Fn-UseC_-Telco-Customer-Churn.csv`

If you don't have it locally, download it and place it in the `datasets/` folder before running the notebook.

## Notebook Workflow
The notebook (`churn_prediction.ipynb`) covers:

- Data loading and quick inspection
- Missing value handling and `TotalCharges` type correction
- Exploratory analysis (churn distribution, tenure/charges by churn, contract type, payment method, internet service)
- One-hot encoding of categorical features
- Train/test split with stratification
- Feature scaling
- Model training and evaluation

## Models Evaluated
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting

## Evaluation
The notebook evaluates models with:

- Accuracy
- Precision / Recall / F1
- ROC AUC
- Confusion matrices
- ROC curve comparison

The results in the notebook show Gradient Boosting providing the best overall discrimination, with Logistic Regression serving as a strong, interpretable baseline.

## Project Structure
- `churn_prediction.ipynb`
- `datasets/WA_Fn-UseC_-Telco-Customer-Churn.csv` (local data file)

## Requirements
Core Python packages used in the notebook:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## How to Run
1. Ensure the dataset is available at `datasets/WA_Fn-UseC_-Telco-Customer-Churn.csv`.
2. Open the notebook and run all cells:

```bash
jupyter notebook churn_prediction.ipynb
```

## Notes
- The notebook is self-contained and includes all preprocessing and evaluation steps.
- If you want a reproducible environment, consider creating a virtual environment and pinning package versions.
