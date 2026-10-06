# Credit Card Fraud Prediction

A Machine Learning project that detects fraudulent credit card transactions using Python and Scikit-learn.

## Project Overview

The goal of this project is to predict whether a credit card transaction is fraudulent or legitimate based on transaction and customer-related information.

The project includes data preprocessing, categorical encoding, feature scaling, Random Forest classification, and hyperparameter tuning using GridSearchCV.

## Dataset

The dataset contains credit card transaction information with features such as:

- Transaction Amount
- Transaction Hour
- Merchant Category
- Card Type
- Transaction Channel
- Previous Transactions in 24 Hours
- Card Age
- Customer Age
- Credit Score
- Account Status

Target variable:

- `is_fraud`
  - `0` = Legitimate Transaction
  - `1` = Fraudulent Transaction

## Machine Learning Workflow

1. Load the dataset
2. Check missing values
3. Remove duplicate records
4. Encode categorical features using LabelEncoder
5. Remove unnecessary features
6. Separate features and target
7. Split data into training and testing sets
8. Apply StandardScaler
9. Train Random Forest Classifier
10. Tune hyperparameters using GridSearchCV
11. Evaluate the model
12. Predict fraud for new user-entered transactions

## Model Used

### Random Forest Classifier

Random Forest is an ensemble machine learning algorithm that combines multiple decision trees to make predictions.

For hyperparameter tuning, GridSearchCV was used to find better model parameters.

## Hyperparameter Tuning

The project tunes:

- `max_depth`
- `n_estimators`

GridSearchCV uses 5-fold cross-validation to evaluate different parameter combinations.

## Model Performance

- Training Accuracy: **100%**
- Testing Accuracy: **99%**

The model achieved 99% accuracy on the test dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Random Forest
- GridSearchCV
- StandardScaler
- LabelEncoder

## Project Structure

```text
credit-card-fraud-prediction/
│
├── Credit Card Fraud Prediction.ipynb
├── credit_card_fraud_balanced.csv
└── README.md
