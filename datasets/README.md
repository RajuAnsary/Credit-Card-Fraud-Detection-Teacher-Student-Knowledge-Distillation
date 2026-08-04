# Project Title
Credit Card Fraud Detection

## Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The goal is to build a reliable classification model that can distinguish between legitimate and fraudulent activities with high accuracy and low false positives.

## Features
- Detects suspicious transaction patterns
- Uses anonymized transaction features for fraud prediction
- Evaluates multiple machine learning models
- Includes visualization and result analysis

## Methodology
- Data collection from publicly available fraud detection datasets
- Exploratory data analysis to understand patterns and class imbalance
- Data preprocessing, scaling, and feature handling
- Model training and evaluation using classification metrics

## Pipeline
1. Load and inspect the dataset
2. Perform data cleaning and preprocessing
3. Split the data into training and testing sets
4. Train and compare machine learning models
5. Evaluate performance using accuracy, precision, recall, F1-score, and ROC-AUC
6. Store and interpret results

## Models Used
- Logistic Regression
- Random Forest
- Gradient Boosting
- Other comparative classifiers as applicable

## Results
The model performance and comparison metrics are stored in the project results directory for reference and analysis.

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
Install the required Python libraries:

```bash
pip install -r requirements.txt
```

## How to Run
Open the Jupyter notebook in the notebooks folder or run the project scripts from the repository root.

## Future Work
- Deploy the model as a web application or API
- Improve handling of imbalanced data
- Explore deep learning approaches for fraud detection

## Authors
- Project Team
- Contributors can be added here
