# 🏦 Loan Default Risk with Business Cost Optimization

## 📌 Project Overview

This project was completed as **Task 4** for the **DevelopersHub Corporation Data Science & Analytics Internship**.

The objective of this project is to predict whether a customer is likely to default on a loan using machine learning techniques and optimize the classification threshold to minimize business costs associated with incorrect predictions.

---

# 🎯 Objectives

- Predict loan default risk using machine learning.
- Clean and preprocess the dataset.
- Perform Exploratory Data Analysis (EDA).
- Train a Logistic Regression classification model.
- Evaluate model performance using multiple evaluation metrics.
- Optimize the prediction threshold using business cost analysis.
- Identify the most important features influencing loan default.

---

# 📂 Dataset

**Dataset Name:** Home Credit Default Risk

**File Used:**

```
application_train.csv
```

The dataset contains customer demographic information, financial history, loan information, and the target variable indicating whether the customer defaulted.

---

# 🛠 Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# 📊 Project Workflow

## 1. Data Loading

- Load dataset using Pandas
- Explore dataset structure

## 2. Data Preprocessing

- Handle missing values
- Encode categorical variables
- Prepare data for machine learning

## 3. Exploratory Data Analysis

- Dataset overview
- Missing value analysis
- Target variable distribution
- Statistical summary

## 4. Feature Selection

- Separate features and target variable
- Split dataset into training and testing sets

## 5. Model Building

- Logistic Regression Classifier

## 6. Model Evaluation

The model is evaluated using:

- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- ROC Curve

## 7. Business Cost Optimization

Different decision thresholds are tested to minimize financial loss caused by incorrect loan approval decisions.

Business costs considered:

- False Positive Cost
- False Negative Cost

The threshold with the minimum total business cost is selected.

## 8. Feature Importance

Model coefficients are analyzed to determine which variables contribute most to loan default prediction.

---

# 📈 Results

The Logistic Regression model successfully predicts customer loan default.

The project demonstrates:

- Effective data preprocessing
- Binary classification
- Model evaluation
- Business cost optimization
- Feature importance analysis

---

# 📁 Project Structure

```
Loan-Default-Risk-Optimization/
│
├── data/
│   └── application_train.csv
│
├── notebooks/
│   └── Loan_Default_Risk.ipynb
│
├── images/
│
├── README.md
│
└── requirements.txt
```

---

# ▶️ How to Run

## Clone Repository

```bash
git clone https://github.com/yourusername/Loan-Default-Risk-Optimization.git
```

---

## Install Required Packages

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Open Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
Loan_Default_Risk.ipynb
```

Run all notebook cells.

---

# 📚 Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis
- Feature Engineering
- Logistic Regression
- Binary Classification
- Model Evaluation
- Business Cost Optimization
- Financial Risk Analysis
- Machine Learning

---

# 📌 Future Improvements

- Random Forest Classifier
- XGBoost
- CatBoost
- Hyperparameter Tuning
- SMOTE for Imbalanced Data
- SHAP Explainable AI
- Streamlit Deployment

---

# 👨‍💻 Author

**Yasir Khan**

Computing Student | Aspiring Data Analyst

### Skills

- Python
- SQL
- Power BI
- Tableau
- Machine Learning
- Data Analytics
- Data Visualization

---

# ⭐ Internship

DevelopersHub Corporation

**Data Science & Analytics Internship**

Task 4 – Loan Default Risk with Business Cost Optimization
