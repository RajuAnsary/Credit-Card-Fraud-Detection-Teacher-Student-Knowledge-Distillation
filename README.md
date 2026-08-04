# Credit Card Fraud Detection

## Project Overview
This repository contains a notebook-based workflow for detecting fraudulent credit card transactions using machine learning and evaluation techniques. The project loads uploaded datasets, preprocesses features, handles class imbalance, trains predictive models, and compares results using multiple metrics.

## Features
- Colab-ready notebook workflow
- Automatic label detection and binary target normalization
- Preprocessing for numerical and categorical features
- Class imbalance handling with oversampling methods such as BorderlineSMOTE
- Evaluation using accuracy, precision, recall, F1-score, ROC-AUC, PR-AUC, MCC, balanced accuracy, and kappa
- Optional explainability support with SHAP

## Methodology
1. Load and inspect uploaded datasets
2. Clean and preprocess transaction features
3. Split the data into training, validation, and testing sets
4. Apply imbalance-handling strategies and train models
5. Evaluate performance and compare results

## Pipeline
- Data loading from CSV or ZIP files
- Missing value handling and feature transformation
- Train/validation/test splitting
- Model training and benchmarking
- Result saving and performance comparison

## Models Used
- Logistic Regression
- XGBoost
- Additional comparison models used in the notebook workflow

## Results
The notebook stores and compares benchmark results for different runs and evaluation metrics.

## Dataset Links
Dataset 1: Credit Card Fraud Detection Dataset (2023)
- Total Transactions: 284,807
- Features: Time, Amount, V1–V28, Class
- Target Variable: Class (0 = Legitimate, 1 = Fraud)
- Data Type: PCA-transformed anonymized credit card transaction records
- Kaggle Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data

Dataset 2: Fraudulent Online Shops Dataset
- Total Transactions: 1141
- Features: ID, Amount, V1–V28, Class
- Target Variable: Class (0 = Legitimate, 1 = Fraud)
- Data Type: PCA-transformed anonymized credit card transaction records
- Kaggle Link: https://data.mendeley.com/datasets/m7xtkx7g5m/1

## Installation
Install the required Python packages:

```bash
pip install -r requirements.txt
```

If you are using Google Colab, install the extra packages used in the notebook:

```bash
pip install imbalanced-learn xgboost shap torch-geometric
```

## How to Run
1. Open the notebook in the notebooks folder.
2. Upload the required dataset files when prompted.
3. Run the cells sequentially to load data, preprocess it, train models, and evaluate results.

## Future Work
- Deploy the final model as an API or web application
- Improve imbalanced-data handling further
- Add real-time fraud monitoring and alerting

## Authors
- Your Name
- Project Team
