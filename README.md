# Credit Card Fraud Detection Project

## Project Overview
This project implements a machine learning solution for detecting fraudulent credit card transactions using both supervised and unsupervised approaches

## Setup and Installation

### Prerequisites
- Python 3.8 or higher
- Recommended: Anaconda or Virtual Environment

### Required Libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn shap
```

### Dataset
- Dataset: Credit Card Fraud Detection Dataset
- Source: Kaggle Credit Card Fraud Detection Dataset
- Features: Transaction details including amount, merchant, location, etc
- Target Variable: is_fraud

## Key Modeling Approaches

### 1. Supervised Learning
- Models:
  - Logistic Regression (Baseline)
  - XGBoost Classifier
- Techniques:
  - SMOTE for handling class imbalance
  - Class weight balancing
  - Feature scaling

### 2. Unsupervised Learning
- Anomaly Detection:
  - Isolation Forest Algorithm
  - Detects rare or unusual transactions
  - Configured with 1 percent contamination rate

## Preprocessing Steps
- Categorical variable encoding
- Missing value imputation
- Feature engineering:
  - Age calculation
  - Transaction time features
  - Spatial distance calculation

## Evaluation Metrics
- Precision
- Recall
- F1 Score
- ROC AUC
- Confusion Matrix

## Reproducibility
1. Clone the repository
2. Install required libraries
3. Download the dataset
4. Update dataset path in the script
5. Run the Jupyter notebook or Python script

## Key Challenges and Solutions
- Handled class imbalance using SMOTE
- Implemented robust age calculation
- Used SHAP for model interpretability

## Limitations and Future Work
- Explore more advanced feature engineering
- Test with different anomaly detection algorithms
- Implement real time fraud detection pipeline
