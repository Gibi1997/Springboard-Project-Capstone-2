# Credit Card Approval Prediction

## Overview
This project builds a machine learning model to predict credit card approval for bank customers. The goal is to replace a manual review process that takes several days with an instant, automated decision system, improving efficiency and reducing operational costs.

## Problem Statement
Banks need to predict credit card approval within seconds instead of waiting 7+ days using manual evaluation methods.

## Dataset
- Two datasets: **application_details** and **credit_details**
- Merged using customer ID
- Final dataset:
  - **36,457 records**
  - **17 features**
- Target variable:
  - **1 → Good customer**
  - **0 → Bad customer**

## Data Processing
- Cleaned missing and inconsistent values
- Encoded categorical variables
- Handled outliers in employment duration
- Performed feature reduction after EDA
- Addressed class imbalance during model evaluation

## Models Used
- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Random Forest
- **Gradient Boosting (Final Model)**

**Evaluation Metric:** F1-score (Macro)  
**Validation Method:** K-Fold Cross-Validation

## Best Model
**Gradient Boosting Classifier**
- Best balance between majority and minority classes
- Strong generalization on test data
- Stable cross-validation performance

## Results
- Enables instant credit approval decisions
- Improves business efficiency
- Reduces financial risk by identifying ineligible applicants

## Limitations
- Class imbalance impacts minority-class prediction
- Synthetic oversampling may not fully reflect real-world data

## Future Improvements
- XGBoost / LightGBM
- Cost-sensitive learning
- Additional feature engineering
- External data integration
