# Customer Churn Prediction using Logistic Regression and Neural Networks

Predicting customer churn is one of the most important business applications of machine learning. Companies can significantly reduce customer loss by identifying customers who are likely to leave and taking preventive actions beforehand.

This project implements and compares two machine learning approaches:

- Logistic Regression
- Artificial Neural Network (MLP Classifier)

The complete workflow includes data preprocessing, exploratory data analysis, model training, evaluation, feature importance analysis, ROC curve analysis, and model comparison.

---

# Table of Contents

1. Project Overview
2. Dataset Description
3. Project Structure
4. Exploratory Data Analysis
5. Data Preprocessing
6. Machine Learning Models
7. Model Evaluation
8. Results and Discussion
9. Visualizations
10. Future Improvements
11. Installation
12. Author

---

# Project Overview

Customer churn occurs when a customer decides to stop using a company's service.

The primary objective of this project is to predict whether a customer will leave the bank based on historical customer information.

This prediction allows organizations to:

- Improve customer retention
- Reduce customer acquisition costs
- Increase profitability
- Develop targeted marketing strategies
- Improve customer satisfaction

---

# Dataset Description

The dataset contains customer demographic and financial information.

## Features

| Feature | Description |
|----------|-------------|
| CreditScore | Customer credit score |
| Geography | Customer country |
| Gender | Customer gender |
| Age | Customer age |
| Tenure | Number of years with bank |
| Balance | Account balance |
| NumOfProducts | Number of products used |
| HasCrCard | Credit card ownership |
| IsActiveMember | Customer activity status |
| EstimatedSalary | Estimated annual salary |
| Exited | Target Variable |

---

## Target Variable

| Value | Meaning |
|---------|----------|
| 0 | Customer Retained |
| 1 | Customer Churned |

---

# Project Structure

```text
CUSTOMER-CHURN-PREDICTION/
│
├── Dataset/
│   └── Churn_Modelling.csv
│
├── images/
│   ├── heatmap.png
│   └── feature_importance.png
│
├── notebooks/
│   └── Customer_Churn_Prediction.ipynb
│
├── requirements.txt
│
├── README.md
│
└── .gitattributes
```

---

# Exploratory Data Analysis

Before model development, exploratory data analysis was performed to understand feature relationships and customer behavior patterns.

The following analyses were conducted:

- Customer churn distribution
- Gender distribution
- Age distribution
- Correlation analysis
- Feature relationship analysis

---

# Correlation Analysis

The correlation heatmap visualizes relationships among numerical variables and helps identify influential features.

<p align="center">
  <img src="images/heatmap.png" width="850">
</p>

---

# Data Preprocessing

Several preprocessing techniques were applied before model training.

### Data Cleaning

- Removed RowNumber
- Removed CustomerId
- Removed Surname

### Encoding

#### Label Encoding

Applied to:

- Gender

#### One-Hot Encoding

Applied to:

- Geography

### Feature Scaling

StandardScaler was used to normalize numerical features.

### Dataset Split

Training Set : 80%

Testing Set : 20%

---

# Machine Learning Models

## 1. Logistic Regression

Logistic Regression is a linear classification algorithm widely used for binary classification tasks.

### Advantages

- Simple implementation
- Fast training
- Interpretable coefficients
- Strong baseline model

### Limitations

- Assumes linear relationships
- Limited ability to model complex interactions

---

## 2. Neural Network (MLP Classifier)

An Artificial Neural Network was implemented using Scikit-Learn's MLPClassifier.

Architecture:

```python
hidden_layer_sizes=(64,32)
```

### Advantages

- Learns nonlinear relationships
- Captures complex feature interactions
- Better pattern recognition

### Limitations

- Higher computational cost
- Lower interpretability

---

# Feature Importance Analysis

Feature importance analysis helps identify which variables contribute most to customer churn prediction.

<p align="center">
  <img src="images/feature_importance.png" width="850">
</p>

Key influential features typically include:

- Age
- Balance
- Credit Score
- Number of Products
- Estimated Salary
- Customer Activity Status

---

# Model Evaluation

Both models were evaluated using multiple classification metrics.

### Metrics Used

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve
- AUC Score

These metrics provide a comprehensive evaluation of classification performance.

---

# Results and Discussion

The developed models successfully learned customer behavior patterns and predicted churn likelihood.

Observations:

- Logistic Regression provided a strong baseline.
- Neural Network captured more complex relationships.
- ROC analysis enabled performance comparison.
- Feature importance analysis improved model interpretability.

The comparison demonstrates how different machine learning approaches perform on the same business problem.

---

# Visualizations Generated

The notebook automatically generates:

- Customer Distribution Plot
- Gender Distribution Plot
- Age Distribution Plot
- Correlation Heatmap
- Logistic Regression Confusion Matrix
- Neural Network Confusion Matrix
- ROC Curve Comparison
- Feature Importance Plot
- Model Accuracy Comparison

---

# Future Improvements

Potential future enhancements include:

- Hyperparameter Optimization
- Cross Validation
- Class Imbalance Handling using SMOTE
- Random Forest
- XGBoost
- LightGBM
- Deep Learning with TensorFlow
- Model Deployment using Flask
- Interactive Dashboard using Streamlit

---

# Installation

Clone the repository

```bash
git clone https://github.com/Bitttu4/customer-churn-prediction.git
```

Move into the project directory

```bash
cd customer-churn-prediction
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

---

# Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

# Author

Aarya Patel

B.Tech Information Technology

Machine Learning Project

---

# License

This repository is intended for educational and learning purposes.