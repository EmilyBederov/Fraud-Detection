# Fraud Detection Final Project

## Overview
This project focuses on building a machine learning pipeline to detect fraudulent transactions. Using a labeled dataset of financial transactions, various preprocessing techniques, feature engineering, and machine learning models are applied to accurately classify transactions as fraudulent or legitimate. Additionally, autoencoders are trained to detect fraud by identifying patterns that deviate from normal transactions. The goal is to create a robust and accurate model that can help detect and prevent fraud in real-time systems.

## Project Contents

### Files
- **FinalProject_FraudDetectionFINAL.ipynb**: The main Jupyter Notebook containing all stages of the project, from data exploration to model evaluation, including the implementation of autoencoders.
- **dataset.csv**: The dataset used in this project, containing transaction information and labels indicating fraud.

### Key Steps
1. **Data Exploration**:
   - Analyzes the structure, distributions, and patterns within the dataset.
   - Visualizes relationships between features and examines class imbalances between fraudulent and legitimate transactions.

2. **Data Preprocessing**:
   - Handles missing values, outliers, and normalization to prepare data for modeling.
   - Addresses class imbalance using techniques like SMOTE (Synthetic Minority Over-sampling Technique) or undersampling.
   - Encodes categorical features and scales numerical features as required.

3. **Feature Engineering**:
   - Creates new features to capture patterns that may be indicative of fraud.
   - Selects important features through techniques like feature importance scores, correlation analysis, or recursive feature elimination.

4. **Model Training and Selection**:
   - Trains several machine learning models, including:
     - Logistic Regression
     - Decision Trees
     - Random Forests
     - Gradient Boosting (e.g., XGBoost)
     - **Autoencoders**: An unsupervised learning technique to identify outliers by learning normal transaction patterns and detecting deviations that may indicate fraud.
   - Performs cross-validation to evaluate each model’s performance and avoid overfitting.
   - Applies hyperparameter tuning using Grid Search or Optuna for optimal model performance.

5. **Model Evaluation**:
   - Evaluates model performance using metrics such as accuracy, precision, recall, F1 score, and ROC-AUC.
   - Compares models, including autoencoders, to identify the best-performing approach for fraud detection.
