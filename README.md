# FindDefault (Prediction of Credit Card fraud) 

## Project Overview
This project aims to detect fraudulent credit card transactions using machine learning. Three classification algorithms were implemented and evaluated: Random Forest, Logistic Regression, and XGBoost. The objective is to identify the best-performing model for fraud detection, balancing precision, recall, and accuracy to minimize false positives and false negatives.

## Problem Statement
A credit card is one of the most used financial products to make online purchases and 
payments. Though the Credit cards can be a convenient way to manage your finances, they can 
also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit 
card information to make purchases or withdraw cash. 
It is important that credit card companies are able to recognize fraudulent credit card 
transactions so that customers are not charged for items that they did not purchase.  

The goal of this project is to build a model that accurately detects fraudulent transactions, thereby protecting cardholders and financial institutions from unauthorized charges.

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

```
credit-card-fraud-detection/
├── data/
│   └── creditcard.csv                     # Raw dataset
├── models/
│   ├── logistic_model.pkl                 # Serialized Logistic Regression model
│   ├── random_forest_model.pkl            # Serialized Random Forest model
│   └── xgboost_model.pkl                  # Serialized XGBoost model
├── notebooks/
│   ├── CreditCardFraudDetection_LogisticRegression.ipynb    # Logistic Regression notebook
│   ├── CreditCardFraudDetection_XGBoost.ipynb               # XGBoost notebook
│   ├── CreditCardFraudDetection_randomforest.ipynb          # Random Forest notebook
│   └── Model_Evaluation_and_Deployment.ipynb                # Model evaluation and deployment notebook
├── visuals/
│   ├── Comparison Plots                 # Folder containing comparison plots
│   ├── LogisticRegression plots         # Folder containing Logistic Regression plots
│   ├── Randomforest plots               # Folder containing Random Forest plots
│   └── XGboost plots                    # Folder containing XGBoost plots
├── docs/
│   └── CreditCardFraudDetection_ProjectReport.pdf  # Project report
├── README.md                              # Project overview and instructions
└── requirements.txt                       # Python dependencies

```

## Model Performance
| Model              | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 95.8%    | 92.4%     | 85.6%  | 88.8%    |
| Random Forest       | 97.2%    | 94.6%     | 89.3%  | 91.9%    |
| XGBoost             | 98.0%    | 95.4%     | 91.2%  | 93.2%    |
