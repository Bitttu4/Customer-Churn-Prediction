# Customer Churn Prediction Project Execution Guide

This document explains how to run the complete Customer Churn Prediction project from setup to result generation.

---

# Step 1: Clone Repository

Clone the repository from GitHub.

```bash
git clone https://github.com/Bitttu4/Customer-Churn-Prediction.git
```

Move into the project directory.

```bash
cd Customer-Churn-Prediction
```

---

# Step 2: Create Virtual Environment (Optional)

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

Linux / macOS:

```bash
python3 -m venv venv
source venv/bin/activate
```

---

# Step 3: Install Dependencies

Install all required packages.

```bash
pip install -r requirements.txt
```

---

# Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

Navigate to:

```text
notebooks/
```

Open:

```text
Customer_Churn_Prediction.ipynb
```

---

# Step 5: Run Notebook Sections Sequentially

Execute notebook cells in the following order.

### Section 1

Introduction

---

### Section 2

Import Required Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

### Section 3

Load Dataset

Dataset:

```text
Dataset/Churn_Modelling.csv
```

Operations:

- Dataset preview
- Dataset shape
- Dataset information
- Statistical summary
- Missing value analysis

---

### Section 4

Exploratory Data Analysis

Visualizations generated:

- Customer Churn Distribution
- Gender Distribution
- Geography Distribution
- Age Distribution
- Balance Distribution
- Correlation Heatmap

Generated File:

```text
images/heatmap.png
```

---

### Section 5

Data Preprocessing

Operations:

- Remove unnecessary columns
- Label Encoding
- One-Hot Encoding
- Feature Scaling
- Train-Test Split

---

### Section 6

Feature Engineering

Operations:

- Training feature preparation
- Target variable analysis
- Feature matrix validation

---

### Section 7

Logistic Regression Model

Operations:

- Model training
- Prediction generation
- Accuracy calculation
- Classification report
- Confusion matrix

---

### Section 8

Neural Network Model

Operations:

- MLPClassifier training
- Prediction generation
- Accuracy calculation
- Classification report
- Confusion matrix

---

### Section 9

Model Evaluation

Metrics:

- Accuracy
- Precision
- Recall
- F1 Score

---

### Section 10

ROC Curve Analysis

Generated File:

```text
images/roc_curve.png
```

---

### Section 11

Feature Importance Analysis

Generated File:

```text
images/feature_importance.png
```

Operations:

- Extract feature importance
- Rank features
- Visualize importance scores
- Identify influential variables

---

### Section 12

Model Comparison

Generated File:

```text
images/model_comparison.png
```

Operations:

- Accuracy comparison
- Best model identification
- Performance summary

---

### Section 13

Conclusion

Project findings:

- Customer churn prediction performance
- Important customer attributes
- Model comparison results
- Business insights

---

# Final Outputs

After successful execution, the following visualizations will be available.

```text
images/
│
├── heatmap.png
├── feature_importance.png
├── roc_curve.png
└── model_comparison.png
```

---

# Project Completion

The notebook execution produces:

- Exploratory Data Analysis
- Logistic Regression Model
- Neural Network Model
- Feature Importance Analysis
- ROC Curve Evaluation
- Model Performance Comparison
- Customer Churn Insights

The project demonstrates a complete machine learning workflow for solving a real-world customer retention problem.