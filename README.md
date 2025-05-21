# credit_cardfraud
Credit Card Fraud Detection System
This project involves the development and deployment of a machine learning model to detect fraudulent credit card transactions using customer data fields (A1 to A14). The goal is to accurately predict whether a transaction is fraudulent or legitimate, using classification techniques with strong performance metrics.

To build a robust classifier that can:

Accurately detect fraud (maximize recall and AUC)

Generalize well using Repeated K-Fold Cross Validation

Handle class imbalance using oversampling techniques like RandomOverSampler

Steps Performed
Data Preprocessing

Removed CustomerID from features

Handled missing/null values

Encoded categorical variables (if present)

Feature scaling (if applicable)

Exploratory Data Analysis (EDA)

Distribution of class labels (Fraud vs Non-Fraud)

Correlation between features

Model Training & Evaluation

Algorithms used:

Logistic Regression (L1 & L2)

KNN

Decision Tree (Gini & Entropy)

Evaluation with RepeatedKFold Cross Validation

Metrics: Accuracy, ROC AUC, Confusion Matrix, Classification Report

Best Model Selected:
 Decision Tree Classifier with Gini Criterion

Accuracy: ~83%

ROC AUC: ~83%

Feature Importance Analysis

Extracted important features from Decision Tree

Helped identify which factors contribute most to fraud

Oversampling with RandomOverSampler

Applied inside the cross-validation loop

Balanced minority class (fraud cases)

Model Deployment (UI)

Built an interactive Streamlit app

Hosted via Ngrok tunnel for public access

Users can enter A1–A14 and predict if a transaction is fraudulent
