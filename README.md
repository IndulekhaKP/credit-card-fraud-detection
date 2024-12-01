# Credit Card Fraud Detection Project

## Project Overview
This project aims to detect fraudulent credit card transactions using machine learning. Three classification algorithms were implemented and evaluated: Random Forest, Logistic Regression, and XGBoost. The objective is to identify the best-performing model for fraud detection, balancing precision, recall, and accuracy to minimize false positives and false negatives.

## Problem Statement
Credit card fraud is a significant problem in financial transactions, resulting in substantial losses. The goal of this project is to build a model that accurately detects fraudulent transactions, thereby protecting cardholders and financial institutions from unauthorized charges.

## Dataset
The dataset used for this project contains transactions made by European credit cardholders in September 2013. It includes 284,807 transactions, with 492 fraudulent cases. The dataset is highly imbalanced, with fraud cases constituting only 0.172% of all transactions.

- Location: The dataset is available in the `data` folder of this repository.
- Attributes:
  - Time: Time in seconds between this transaction and the first transaction in the dataset.
  - V1-V28: Principal Component Analysis (PCA)-transformed features for privacy.
  - Amount: Transaction amount.
  - Class: Target variable (0 = Non-Fraud, 1 = Fraud).

## Project Structure
The repository is organized as follows:


credit-card-fraud-detection/
├── data/
│   └── creditcard.csv               # Raw dataset
├── models/
│   ├── logistic_model.pkl           # Serialized Logistic Regression model
│   ├── random_forest_model.pkl      # Serialized Random Forest model
│   └── xgboost_model.pkl            # Serialized XGBoost model
├── notebooks/
│   ├── logistic_regression.ipynb    # Notebook for Logistic Regression model
│   ├── random_forest.ipynb          # Notebook for Random Forest model
│   └── xgboost.ipynb                # Notebook for XGBoost model
├── visuals/
│   ├── fraud_plot.png               # Class distribution plot
│   ├── ROC_Curve_Comparison.png     # ROC Curve Comparison
│   ├── Precision_Recall_Curve.png   # Precision-Recall Curve
│   └── feature_importance_rf.png    # Random Forest Feature Importance
├── docs/
│   └── CreditCardFraud_Project_Report.pdf # Project report
├── README.md                        # Project overview and instructions
└── requirements.txt                 # Python dependencies


## Model Performance
| Model              | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 95.8%    | 92.4%     | 85.6%  | 88.8%    |
| Random Forest       | 97.2%    | 94.6%     | 89.3%  | 91.9%    |
| XGBoost             | 98.0%    | 95.4%     | 91.2%  | 93.2%    |
