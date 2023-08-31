# Banking Transactions Fraud Detection

This repository contains code and resources for a machine learning project focused on fraud detection in banking transactions. The primary model used for prediction is the Random Forest Classifier. The project addresses a classification problem with the goal of identifying fraudulent transactions within a banking dataset.

## Data Details

The dataset used for this project includes various features that provide insights into banking transactions. Here are the key features:

* **step**: Represents a unit of time in the real world. Each step corresponds to 1 hour of time, totaling 744 steps (30 days simulation).
* **type**: Describes the type of transaction, which can be CASH-IN, CASH-OUT, DEBIT, PAYMENT, or TRANSFER.
* **amount**: Represents the amount of the transaction in the local currency.
* **nameOrig**: Refers to the customer who initiated the transaction.
* **oldbalanceOrg**: Represents the initial balance before the transaction.
* **newbalanceOrig**: Represents the new balance after the transaction.
* **nameDest**: Refers to the customer who is the recipient of the transaction.
* **oldbalanceDest**: Represents the initial balance of the recipient before the transaction. Note that there is no information for customers starting with M (Merchants).
* **newbalanceDest**: Represents the new balance of the recipient after the transaction. Note that there is no information for customers starting with M (Merchants).
* **isFraud**: A binary label indicating whether a transaction is fraudulent. Transactions made by fraudulent agents aim to take control of customer accounts and attempt to empty funds by transferring to another account and then cashing out of the system.
* **isFlaggedFraud**: This feature flags illegal attempts in the business model, specifically massive transfers from one account to another. An illegal attempt in this dataset is defined as an attempt to transfer more than 200,000 in a single transaction.

## Project Overview

The project aims to build and train a Random Forest Classifier model to predict fraudulent transactions based on the provided dataset. The classification problem involves identifying whether a given transaction is fraudulent or not. The code and resources in this repository provide a step-by-step guide for data preprocessing, model training, evaluation, and performance analysis.

This project also involves feature importance analysis to see which are the features that most effect the model's decision.

Feel free to explore the code, adapt it to your own datasets, and contribute to enhancing the accuracy of fraud detection in banking transactions.
