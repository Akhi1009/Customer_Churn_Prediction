# Customer Churn Prediction
This project leverages machine learning to predict customer churn, enabling businesses to identify and retain customers at risk of leaving. The model uses a Voting Classifier, combining Random Forest and Logistic Regression to achieve optimal performance. The goal is to provide a data-driven solution for churn prediction with high precision and recall.

## Project Overview

Customer churn prediction involves forecasting which customers are likely to stop using a company's service. The model was built to predict whether a customer will churn based on historical data.

Key Steps:
1. **Data Collection:** Utilized customer data including features such as demographics, account details, and customer behavior.
2. **Data Preprocessing:** Handled missing values, outliers, and feature scaling to ensure optimal model performance.
3. **Model Evaluation:** Evaluated multiple machine learning algorithms and selected the best performing model.

## Data Preprocessing

The following preprocessing steps were performed:
- Handled missing values using **mean imputation** for numerical columns.
- Categorical features were **encoded** using one-hot encoding.
- Data was **normalized** using **MinMax scaling** to prepare for model training.

## Model Selection & Evaluation

Several machine learning models were evaluated, including:
- Logistic Regression
- Random Forest
- Decision Tree
- AdaBoost Classifier
- Gradient Boosting Classifier
- K-Nearest Neighbors (KNN)

Models were evaluated based on **accuracy, precision, recall, F1-score, and AUC-ROC**. After testing multiple models, the **Voting Classifier** was selected for its ability to combine the strengths of **Random Forest** and **Logistic Regression**, resulting in the highest AUC-ROC score of **0.8612**.

## Final Model: Voting Classifier

The **Voting Classifier** was selected as the final model for its:
- **Balanced Performance:** Combines precision from Random Forest and recall from Logistic Regression.
- **AUC-ROC Score of 0.8612**: Demonstrates the model's ability to effectively distinguish churners from non-churners.
- **Robust Predictions:** Reduces overfitting by leveraging multiple algorithms.
