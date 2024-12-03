# **Credit Card Fraud Detection**  

This project aims to detect fraudulent credit card transactions using machine learning techniques. Given the highly imbalanced nature of the dataset, we explore methods like **SMOTE (Synthetic Minority Oversampling Technique)** to handle class imbalance effectively.

---

## **🔍 Project Overview**  

### Problem Statement:  
Predict fraudulent transactions to minimize financial losses for banks and customers.  

### Key Challenges:  
- **Imbalanced Dataset**: Only 0.17% of transactions are fraudulent.  
- **Feature Scaling**: Ensure numerical stability in the model.  
- **Metric Selection**: Use ROC-AUC for performance evaluation due to imbalanced data.

---

## **📊 Tools & Technologies**  
- **Python**: Data preprocessing and model development.  
- **scikit-learn**: For implementing classification models and SMOTE.  
- **matplotlib & seaborn**: Data visualization.  
- **imbalanced-learn**: Handling imbalanced datasets.

---

## **📂 Project Structure**  

```plaintext
fraud-detection/
│
├── data/
│   ├── creditcard.csv    # Raw dataset
│
├── notebooks/
│   ├── preprocessing.ipynb    # Data preparation and EDA
│   ├── smote_model.ipynb      # Model with SMOTE
│   ├── normal_model.ipynb     # Model without oversampling
│
├── models/
│   ├── logistic_regression.pkl  # Trained logistic regression model
│   ├── xgboost_model.pkl        # Trained XGBoost model
│
├── README.md
└── LICENSE
```
## **🚀 Approach**
**Data Preprocessing**

1. Removed the Time column as it showed no specific pattern.
2. Scaled the Amount column using StandardScaler.
3. Class Imbalance Handling

## **SMOTE**: Generated synthetic data to balance classes.
Built separate models for balanced (SMOTE) and imbalanced data.
## **Model Building**

Explored logistic regression and XGBoost.
Evaluated models using ROC-AUC and F1-Score.

## **📊 Key Results**
Model	ROC-AUC Score (Train)	ROC-AUC Score (Test)	F1-Score
Logistic Regression	0.97	0.96	0.77
SMOTE + Logistic	0.99	0.98	0.81
## **📝 Insights**
SMOTE significantly improves sensitivity and F1-Score for fraudulent transactions.
XGBoost achieves higher precision but is computationally expensive compared to logistic regression.
