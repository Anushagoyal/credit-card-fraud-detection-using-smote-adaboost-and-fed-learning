# Credit Card Fraud Detection with Federated Learning and AdaBoost
This project demonstrates credit card fraud detection using a federated learning approach with AdaBoost as the base model. It addresses the challenge of imbalanced datasets and aims to improve fraud detection accuracy.

## Installation
Install the required libraries using pip:
1.Data Handling: pandas, numpy
2.Machine Learning: scikit-learn, imblearn
3.Model Persistence: joblib
4.Visualization: matplotlib
5.System Interaction: os

## Usage

1. **Data Preparation:**
   - Load the credit card transaction dataset (creditcard.csv).
   - Preprocess the data, including handling missing values and scaling if needed.

2. **Federated Learning:**
   - Split the data into multiple nodes.
   - Apply SMOTE for data balancing at both global and local levels.
   - Train AdaBoost models on each node's data.

3. **Model Aggregation:**
   - Aggregate predictions from individual node models to create a global model.

4. **Evaluation:**
   - Evaluate the global model's performance using metrics like accuracy, precision, recall, and F1-score.

5. **Prediction:**
   - Use the global model to predict fraud on new transactions.

## Data

The project uses the "creditcard.csv" dataset, which contains credit card transactions with a binary label indicating fraudulent or genuine transactions. It can be obtained from https://github.com/Anushagoyal/credit-card-fraud-detection-using-smote-adaboost-and-fed-learning/blob/main/drive/MyDrive/MAJOR%20PROJECT/data/raw/creditcard%20dataset%20download

## Model

The project employs AdaBoost as the base model for fraud detection. Hyperparameters such as the number of estimators and learning rate can be adjusted.

## Evaluation

The model's performance is evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
