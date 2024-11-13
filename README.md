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
│
├── data/
│   └── creditcard.csv                # Raw dataset
│
├── models/
│   └── best_model.joblib             # Serialized file of the best model
│
├── notebooks/
│   ├── random_forest.ipynb           # ipynb file for Random Forest model
│   ├── logistic_regression.ipynb     # ipynb file for Logistic Regression model
│   └── xgboost.ipynb                 # ipynb file for XGBoost model
│
├── SampleExecutions/           # PDF versions of executed notebooks with output
│   ├── random_forest.pdf
│   ├── logistic_regression.pdf
│   └── xgboost.pdf
│
├── visuals/
│   └── fraud_plot.png                # Important plots or visualizations
│
├── README.md                         # Overview and instructions
├── CreditCardFraud Project Report    # Comprehensive report
└── requirements.txt                  # Python dependencies
