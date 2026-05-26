# Customer Churn Prediction

## Overview

Customer churn refers to customers leaving a company or discontinuing a service. Predicting churn helps businesses identify at-risk customers and take preventive actions to improve retention.

This project uses Machine Learning techniques to analyze customer information and predict whether a customer is likely to leave the bank. The project includes data preprocessing, exploratory data analysis, model training, evaluation, and feature importance analysis.

---

## Objective

The primary objective of this project is to:

- Analyze customer behavior patterns
- Identify factors contributing to customer churn
- Build a classification model for churn prediction
- Evaluate model performance using standard metrics
- Understand feature importance for business insights

---

## Dataset

The project uses the **Churn Modelling Dataset** containing customer information such as:

| Feature | Description |
|----------|-------------|
| CreditScore | Customer credit score |
| Geography | Customer country/location |
| Gender | Customer gender |
| Age | Customer age |
| Tenure | Number of years with the bank |
| Balance | Account balance |
| NumOfProducts | Number of bank products used |
| HasCrCard | Credit card ownership |
| IsActiveMember | Customer activity status |
| EstimatedSalary | Estimated annual salary |
| Exited | Target variable (Churn Status) |

Target Variable:

- 0 → Customer Stayed
- 1 → Customer Left

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- LightGBM

---

## Project Workflow

### 1. Data Loading

The dataset is imported and inspected for structure, missing values, and overall quality.

### 2. Data Cleaning

- Removed unnecessary columns
- Encoded categorical variables
- Prepared data for model training

### 3. Exploratory Data Analysis (EDA)

Performed data visualization and statistical analysis to understand customer behavior.

Examples:

- Correlation Heatmap
- Customer Distribution Analysis
- Feature Relationships

### 4. Feature Engineering

Generated model-ready features and transformed categorical data into numerical format.

### 5. Model Training

A LightGBM classifier was trained using the processed dataset.

### 6. Model Evaluation

Performance was evaluated using:

- Accuracy Score
- Classification Report
- Confusion Matrix

### 7. Feature Importance Analysis

Identified the most influential factors affecting customer churn.

---

## Visualizations

### Correlation Heatmap

Shows relationships among numerical features and helps identify important correlations.

### Feature Importance Plot

Displays which customer attributes contribute most to churn prediction.

---

## Model Evaluation Metrics

The following metrics are used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## Project Structure

```
Customer-Churn-Prediction/
│
├── data/
│   └── Churn_Modelling.csv
│
├── notebooks/
│   └── Customer_Churn_Prediction.ipynb
│
├── images/
│   ├── heatmap.png
│   └── feature_importance.png
│
├── requirements.txt
│
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/customer-churn-prediction.git
```

Move into the project directory:

```bash
cd customer-churn-prediction
```

Install required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

## Results

The trained model successfully predicts customer churn based on customer attributes and provides insights into the most significant factors influencing customer retention.

Key outcomes:

- Accurate churn prediction
- Business-oriented insights
- Interpretable feature importance
- Practical machine learning workflow implementation

---

## Future Improvements

- Hyperparameter optimization
- Cross-validation
- Class imbalance handling
- Ensemble learning approaches
- Deployment using Flask or FastAPI
- Real-time prediction dashboard

---

## Author

Aarya Patel

B.Tech Information Technology

Academic Machine Learning Project