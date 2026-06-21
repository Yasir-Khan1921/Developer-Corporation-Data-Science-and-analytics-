# Task 2: Credit Risk Prediction
### DevelopersHub Corporation — Data Science & Analytics Internship

**Author:** Yasir Khan  
**Date:** June 2026

---

##  Task Objective
The primary objective of this project is to develop a binary classification model that predicts whether a loan applicant is likely to default on a loan. By identifying credit risks beforehand, financial institutions can make data-driven decisions to approve or reject loans and minimize financial defaults.

---

## 📊 Dataset Overview
The project uses the **Loan Prediction Dataset** (commonly found on Kaggle), which contains historical information about loan applicants. Key features include:
* `Gender`, `Married`, `Dependents`, `Education`, `Self_Employed` (Demographics)
* `ApplicantIncome`, `CoapplicantIncome` (Financial indicators)
* `LoanAmount`, `Loan_Amount_Term`, `Credit_History` (Loan-specific details)
* `Property_Area` (Location)
* **Target Variable:** `Loan_Status` (Y = Approved / Default Risk low, N = Rejected / Default Risk high)

---

##  Methodology & Implementation
The workflow implemented in the Jupyter notebook `Task 2 Credit Risk Prediction.ipynb` includes:

1. **Exploratory Data Analysis (EDA):**
   * Plotted histograms to examine the distribution of applicant income.
   * Built count plots to analyze the balance of loan approvals vs. rejections (`Loan_Status`).
   * Visualized the relationship between education level status and loan approvals.
2. **Data Preprocessing & Cleaning:**
   * Handled missing values using the mode for categorical features (`Gender`, `Married`, `Dependents`, `Self_Employed`) and the mean for numerical features (`LoanAmount`).
   * Encoded categorical features into numerical values using `LabelEncoder`.
   * Partitioned data into training (80%) and testing (20%) sets.
   * Applied `StandardScaler` to normalize features for optimization stability.
3. **Model Training:**
   * Trained a **Logistic Regression** classifier (with up to 5,000 maximum iterations for convergence).
4. **Evaluation:**
   * Calculated model accuracy and outputted the Confusion Matrix.

---

##  Results & Performance
* **Model Used:** Logistic Regression (with Feature Scaling)
* **Classification Accuracy:** **78.86%**
* **Key Findings:**
  * Applicant income and credit history play pivotal roles in determining loan approval status.
  * Historical credit records are strong predictors of future credit risk.
## 🛠️ Tech Stack & Libraries
* **Language:** Python 3
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
* **Environment:** Jupyter Notebook

##  How to Run the Notebook
1. Install requirements:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn notebook
   ```
2. Place the dataset `train.csv` under a `Downloads/` directory relative to this folder, or update the load path in the notebook:
   ```python
   df = pd.read_csv("Downloads/train.csv")
   ```
3. Run Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open and execute `Task 2 Credit Risk Prediction.ipynb`.
