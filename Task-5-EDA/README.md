# Task 5: Personal Loan Acceptance Prediction
### DevelopersHub Corporation — Data Science & Analytics Internship

**Author:** Yasir Khan  
**Date:** June 2026

---

## 📌 Task Objective
The primary objective of this task is to develop a predictive model that identifies bank customers who are likely to accept a personal loan or term deposit offer. By identifying the key factors influencing acceptance, banks can optimize their marketing strategies, target high-value customer segments, and increase campaign conversion rates.

---

## 📊 Dataset Overview
The project is built on the **Bank Marketing Dataset** (UCI Machine Learning Repository, saved as `bank.csv`). Key variables analyzed include:
* **Demographics:** `age`, `job`, `marital`, `education`
* **Financial Data:** `balance` (yearly average balance), `default` (has credit default?), `housing` (has housing loan?), `loan` (has personal loan?)
* **Marketing Campaigns:** `contact` (communication type), `day`, `month`, `duration` (last contact duration in seconds), `campaign` (number of contacts performed)
* **Historical Outcomes:** `pdays`, `previous`, `poutcome` (outcome of the previous marketing campaign)
* **Target Variable:** `deposit` (whether the client subscribed to a term deposit / accepted the loan: yes or no)

---

## ⚙️ Methodology & Implementation
The workflow implemented in the Jupyter notebook `Task 5: Personal Loan Acceptance Prediction.ipynb` includes:

1. **Environment Setup & Data Import:** Loaded the `bank.csv` dataset and inspected basic stats (`shape`, `info`, `describe`).
2. **Exploratory Data Analysis (EDA):**
   * Plotted age distribution using histograms.
   * Visualized the distributions of customer jobs and marital status.
   * Examined the target class balance (`deposit` count plots).
3. **Data Preprocessing & Scaling:**
   * Split data into target (`y`) and feature matrix (`X`).
   * Encoded categorical attributes into numerical representations.
   * Partitioned the dataset into 80% training and 20% testing sets.
   * Normalized features using `StandardScaler` to ensure optimal performance of the gradient-based Logistic Regression model.
4. **Model Training & Evaluation:**
   * Trained a **Logistic Regression** classifier (with up to 3,000 max iterations for convergence).
   * Computed accuracy,Confusion Matrix, and full Classification Report (Precision, Recall, F1-Score).

---

## 📈 Results & Evaluation
* **Model Used:** Logistic Regression (with Feature Scaling)
* **Classification Accuracy:** **78.99%** (approx. 79%)
* **Confusion Matrix:**
  ```
  [[955  211]   (True Negatives, False Positives)
   [258  809]]  (False Negatives, True Positives)
  ```
* **Detailed Performance Metrics:**
  * **Class 0 (No Acceptance):** Precision: 0.79 | Recall: 0.82 | F1-Score: 0.80
  * **Class 1 (Acceptance):** Precision: 0.79 | Recall: 0.76 | F1-Score: 0.78
* **Key Business Insights:**
  * **Balance Impact:** Customers with higher balances demonstrate a significantly higher likelihood of accepting deposits/loans.
  * **Demographics:** Marital status and education level influence final client decisions.
  * **Professional Segments:** Certain job categories (e.g., management, technicians) respond much more favorably to campaigns.
  * **Targeting:** The bank can leverage these insights to target high-potential customer profiles, maximizing marketing efficiency.

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
2. Place the dataset `bank.csv` in the same directory as the notebook, or update the load path in the notebook:
   ```python
   df = pd.read_csv("bank.csv")
   ```
3. Run Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open and execute `Task 5: Personal Loan Acceptance Prediction.ipynb`.
