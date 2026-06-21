# Task 3: Customer Churn Prediction
### DevelopersHub Corporation — Data Science & Analytics Internship

**Author:** Yasir Khan  
**Date:** June 2026

---

## 📌 Task Objective
The objective of this project is to develop a predictive model that identifies bank customers who are most likely to leave the bank (churn). Understanding churn helps banks formulate proactive retention strategies, personalize customer outreach, and ultimately reduce customer attrition.

---

## 📊 Dataset Overview
The project utilizes the **Churn Modelling Dataset** (comprising 10,000 customer records). Features include:
* `CreditScore`, `Age`, `Tenure`, `Balance`, `NumOfProducts`, `EstimatedSalary` (Financial & Account metrics)
* `Geography`, `Gender` (Demographics)
* `HasCrCard` (Credit card status), `IsActiveMember` (Activity indicator)
* **Target Variable:** `Exited` (1 = Churned, 0 = Retained)

---

## ⚙️ Methodology & Implementation
The workflow implemented in the Jupyter notebook `Task 3 Customer Churn Prediction.ipynb.ipynb` includes:

1. **Data Cleaning & Preparation:**
   * Loaded the dataset and handled missing values using forward fill (`ffill`).
   * Dropped non-predictive identity columns (such as `RowNumber`, `CustomerId`, and `Surname`).
   * Encoded categorical features (like `Geography` and `Gender`) to prepare them for machine learning models.
2. **Exploratory Data Analysis (EDA):**
   * Plotted count plots to analyze the customer churn distribution.
   * Investigated age distribution using histograms to identify demographic trends.
3. **Model Selection & Training:**
   * Partitioned the dataset into training (80%) and testing (20%) subsets.
   * Trained a **Random Forest Classifier** (with 100 estimators) to capture non-linear relationships.
4. **Evaluation:**
   * Evaluated model accuracy.
   * Computed the Confusion Matrix and Classification Report (Precision, Recall, F1-Score).

---

## 📈 Results & Evaluation
* **Model Used:** Random Forest Classifier
* **Overall Classification Accuracy:** **86.45%**
* **Detailed Performance Metrics:**
  * **Class 0 (Retained):** Precision: 0.88 | Recall: 0.96 | F1-Score: 0.92
  * **Class 1 (Churned):** Precision: 0.75 | Recall: 0.47 | F1-Score: 0.58
* **Key Findings:**
  * Random Forest performs very well in predicting customer retention.
  * Customer age, account balance, active member status, and number of products are significant features influencing customer decision to churn.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
* **Environment:** Jupyter Notebook

---

## 🚀 How to Run the Notebook
1. Install requirements:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn notebook
   ```
2. Place the dataset `Churn_Modelling.csv` on your Desktop, or adjust the path inside the notebook:
   ```python
   df = pd.read_csv("/Users/yasirkhan/Desktop/Churn_Modelling.csv")
   ```
3. Run Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open and execute `Task 3 Customer Churn Prediction.ipynb.ipynb`.
