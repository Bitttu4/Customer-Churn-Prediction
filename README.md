# Customer Churn Prediction using Machine Learning and Neural Networks

## Overview

Customer churn prediction is a supervised machine learning problem that aims to identify customers who are likely to discontinue using a company's services.

Customer retention is often more cost-effective than acquiring new customers. By predicting churn in advance, organizations can take proactive measures to improve customer satisfaction and reduce revenue loss.

This project develops and compares two classification models:

- Logistic Regression
- Neural Network (MLP Classifier)

The project covers the complete machine learning workflow, including data preprocessing, exploratory data analysis, model training, evaluation, visualization, and performance comparison.

---

## Problem Statement

The objective of this project is to predict whether a customer will leave the bank based on demographic and account-related information.

Target Variable:

| Value | Meaning |
|---------|----------|
| 0 | Customer Stays |
| 1 | Customer Leaves |

---

## Dataset Information

The project uses the Churn Modelling Dataset containing customer banking information.

### Features

| Feature | Description |
|----------|-------------|
| CreditScore | Customer credit score |
| Geography | Country of residence |
| Gender | Customer gender |
| Age | Customer age |
| Tenure | Years with the bank |
| Balance | Account balance |
| NumOfProducts | Number of products used |
| HasCrCard | Credit card ownership |
| IsActiveMember | Activity status |
| EstimatedSalary | Estimated annual salary |
| Exited | Churn indicator (Target Variable) |

---

## Project Workflow

### 1. Data Collection

- Load customer dataset
- Inspect data structure
- Verify data quality

### 2. Data Preprocessing

- Remove unnecessary columns
- Label Encoding
- One-Hot Encoding
- Feature Scaling
- Train-Test Split

### 3. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand customer behavior patterns and feature relationships.

Visualizations include:

- Customer Churn Distribution
- Gender Distribution
- Age Distribution
- Correlation Heatmap

### 4. Model Development

Two machine learning models were implemented:

#### Logistic Regression

A linear classification model used as a baseline approach.

#### Neural Network (MLP Classifier)

A feed-forward artificial neural network capable of learning nonlinear relationships within the dataset.

### 5. Model Evaluation

Models were evaluated using:

- Accuracy Score
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve
- AUC Score

### 6. Model Comparison

Performance comparison between Logistic Regression and Neural Network models.

### 7. Feature Importance Analysis

Feature importance was analyzed to identify the most influential factors contributing to customer churn.

---

## Technologies Used

| Category | Tools |
|-----------|--------|
| Programming Language | Python |
| Development Environment | Jupyter Notebook |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-Learn |
| Neural Network | MLPClassifier |
| Version Control | Git, GitHub |

---

## Project Structure

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
├── .gitattributes
│
└── README.md
```

---

## Correlation Heatmap

The correlation heatmap helps identify relationships among numerical features and provides insights into variables that influence churn.

![Correlation Heatmap](images/heatmap.png)

---

## Feature Importance Analysis

Feature importance analysis highlights the most influential customer attributes affecting churn prediction.

![Feature Importance](images/feature_importance.png)

---

## Models Implemented

### Logistic Regression

Advantages:

- Fast training
- Easy interpretation
- Computationally efficient
- Strong baseline model

Limitations:

- Assumes linear relationships
- Limited capability for complex patterns

---

### Neural Network (MLP Classifier)

Advantages:

- Learns nonlinear relationships
- Better pattern recognition
- Higher predictive capability

Limitations:

- Requires more computational resources
- Less interpretable than linear models

---

## Evaluation Metrics

The following metrics were used to assess model performance:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve
- AUC Score

These metrics provide a comprehensive understanding of classification effectiveness and prediction quality.

---

## Experimental Results

After training and evaluation:

- Logistic Regression provided a reliable baseline performance.
- Neural Network captured more complex customer behavior patterns.
- ROC Curve analysis was used to compare classification capabilities.
- Feature importance analysis revealed key churn-driving factors.

The final comparison demonstrates how different machine learning approaches perform on the same customer churn dataset.

---

## Key Learning Outcomes

Through this project:

- Applied complete machine learning workflow
- Performed data preprocessing and feature engineering
- Conducted exploratory data analysis
- Implemented classification algorithms
- Built an Artificial Neural Network
- Compared model performance
- Generated business-oriented insights from data
- Visualized model behavior using multiple evaluation techniques

---

## Future Improvements

Potential enhancements include:

- Hyperparameter Optimization
- Cross Validation
- Class Imbalance Handling (SMOTE)
- Random Forest Classifier
- XGBoost Classifier
- LightGBM Classifier
- Deep Learning with TensorFlow/Keras
- Deployment using Flask or FastAPI
- Interactive Dashboard using Streamlit

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/customer-churn-prediction.git
```

Navigate to the project directory:

```bash
cd customer-churn-prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

## Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## Author

Aarya Patel

B.Tech Information Technology

Machine Learning Project – Customer Churn Prediction

---

## License

This project is intended for educational and academic purposes.