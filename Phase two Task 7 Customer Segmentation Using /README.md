# 🏦 Loan Default Risk with Business Cost Optimization

> **DevelopersHub Corporation – Data Science & Analytics Internship**  
> **Task 4: Loan Default Risk with Business Cost Optimization**

---

## 📖 Project Overview

This project aims to predict whether a customer is likely to default on a loan using machine learning techniques. It also focuses on optimizing the decision threshold based on business costs associated with false positives and false negatives.

The project follows a complete machine learning workflow, including data preprocessing, exploratory data analysis (EDA), model training, evaluation, feature importance analysis, and business cost optimization.

---

## 🎯 Objectives

- Predict customer loan default risk.
- Clean and preprocess the dataset.
- Perform Exploratory Data Analysis (EDA).
- Train a Logistic Regression model.
- Evaluate model performance using multiple metrics.
- Optimize the classification threshold to reduce business losses.
- Analyze the most influential features affecting loan default.

---

## 📂 Dataset

**Dataset Name:** Home Credit Default Risk

**Dataset File:**

```text
application_train.csv
```

The dataset contains customer demographic information, financial history, loan records, and a target variable indicating whether the customer defaulted on the loan.

---

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 🚀 Project Workflow

### 1️⃣ Data Loading
- Load the dataset using Pandas.
- Display sample records.
- Explore dataset dimensions.

### 2️⃣ Data Cleaning & Preprocessing
- Handle missing values.
- Encode categorical variables.
- Prepare numerical features.
- Create training and testing datasets.

### 3️⃣ Exploratory Data Analysis (EDA)
- Dataset overview
- Missing value analysis
- Statistical summary
- Target variable distribution
- Data visualization

### 4️⃣ Model Development
A Logistic Regression classifier is trained to predict whether a customer is likely to default on a loan.

### 5️⃣ Model Evaluation
The model performance is evaluated using:

- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- ROC Curve

### 6️⃣ Business Cost Optimization
Instead of using the default probability threshold (0.50), different thresholds are evaluated to minimize business costs.

Business assumptions:

- **False Positive Cost:** 1000
- **False Negative Cost:** 5000

The threshold producing the lowest total business cost is selected as the optimal threshold.

### 7️⃣ Feature Importance
The model coefficients are analyzed to identify the features that have the greatest impact on predicting loan default risk.

---

## 📊 Results

The Logistic Regression model successfully classified customers based on their default risk.

### Key Outcomes

- ✔ Data successfully cleaned and preprocessed.
- ✔ Missing values handled.
- ✔ Categorical variables encoded.
- ✔ Binary classification model developed.
- ✔ Business cost optimization performed.
- ✔ Important predictive features identified.

---

## 📁 Project Structure

```text
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

## ▶️ How to Run the Project

### Clone the Repository

```bash
git clone https://github.com/your-username/Loan-Default-Risk-Optimization.git
```

### Install Required Libraries

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Loan_Default_Risk.ipynb
```

Run all notebook cells in sequence.

---

## 📦 Requirements

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 💡 Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Logistic Regression
- Binary Classification
- Machine Learning
- Model Evaluation
- Business Cost Optimization
- Financial Risk Analysis
- Data Visualization

---

## 🔮 Future Improvements

- Implement Random Forest Classifier
- Train XGBoost and CatBoost models
- Perform Hyperparameter Tuning
- Handle Class Imbalance using SMOTE
- Apply SHAP for Explainable AI (XAI)
- Deploy the model using Streamlit

---

## 👨‍💻 Author

**Yasir Khan**

Computing Student | Aspiring Data Analyst

### Connect with Me

- 💼 LinkedIn: https://www.linkedin.com/in/yasir-khan-057415407/
- 💻 GitHub: https://github.com/YasirKhan-07

---

## 📄 License

This project is developed for educational purposes as part of the **DevelopersHub Corporation Data Science & Analytics Internship**.
