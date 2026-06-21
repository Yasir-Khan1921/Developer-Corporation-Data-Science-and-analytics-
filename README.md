# Data Science & Analytics Internship Portfolio
### DevelopersHub Corporation

**Author:** Yasir Khan  
**Date:** June 2026

---

## 📌 Executive Summary
This portfolio contains five distinct data science and machine learning projects completed during the internship at DevelopersHub Corporation. The projects range from exploratory data analysis and visualization to classification and regression model development, using real-world datasets.

---

## 📅 Project Portfolio Overview

| Task | Title | Type | Key Algorithm | Key Metric | Directory Links |
|:---|:---|:---|:---|:---|:---|
| **Task 1** | [Iris Exploration & Visualization](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-1-Iris-Exploration) | Exploratory Data Analysis (EDA) | N/A (Visualization) | Qualitative Insights | [GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-1-Iris-Exploration) \| [Local](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%201%20-%20Iris%20Exploration) |
| **Task 2** | [Credit Risk Prediction](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-2-Credit-Risk-Prediction) | Binary Classification | Logistic Regression | Accuracy: **78.86%** | [GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-2-Credit-Risk-Prediction) \| [Local](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%202%20-%20Credit%20Risk%20Prediction) |
| **Task 3** | [Customer Churn Prediction](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-3-Customer-Churn-Prediction) | Binary Classification | Random Forest | Accuracy: **86.45%** | [GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-3-Customer-Churn-Prediction) \| [Local](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%203%20-%20Customer%20Churn%20Prediction) |
| **Task 4** | [Insurance Cost Prediction](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-4-Insurance-Cost-Prediction) | Regression | Linear Regression | $R^2$ Score: **0.7833** | [GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-4-Insurance-Cost-Prediction) \| [Local](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%204%20-%20Insurance%20Cost%20Prediction) |
| **Task 5** | [Personal Loan Acceptance](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-5-EDA) | Binary Classification | Logistic Regression | Accuracy: **78.99%** | [GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-5-EDA) \| [Local](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%205%20-%20Personal%20Loan%20Acceptance) |

---

## 🛠️ Unified Tech Stack & Setup

All tasks are implemented in Python within Jupyter Notebook environments.

### Requirements:
Install the dependencies required for all tasks at once:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn notebook
```

### Running the Notebooks:
1. Navigate to the root directory `task wise read me. file `
2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Navigate to any task directory and open the corresponding notebook to run the cells.

---

## 📁 Detailed Task Breakdown

### 🌸 [Task 1: Iris Exploration & Visualization](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-1-Iris-Exploration)
* **Objective:** Conduct a comprehensive Exploratory Data Analysis (EDA) on the Iris dataset to uncover patterns and relationships among species.
* **Dataset:** 150 instances of Iris flowers across three species (*Setosa*, *Versicolor*, *Virginica*) with sepal/petal dimensions.
* **Key Visualizations:** Pair plots, heatmaps, box plots, violin plots, and histograms.
* **Key Findings:** 
  * *Setosa* is linearly separable from the other two species.
  * Petal measurements (length and width) are highly correlated (0.96) and serve as the best indicators for species classification.
* **GitHub Repository:** [Task 1 Folder on GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-1-Iris-Exploration)
* **Local Links:** [Local Notebook](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%201%20-%20Iris%20Exploration/Task_1_Iris_Exploration_and_Visualization.ipynb) | [Local README.md](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%201%20-%20Iris%20Exploration/README.md)

---

### 💳 [Task 2: Credit Risk Prediction](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-2-Credit-Risk-Prediction)
* **Objective:** Predict the likelihood of a loan applicant defaulting based on demographic and financial variables.
* **Dataset:** Kaggle Loan Prediction Dataset containing variables like education, credit history, marital status, and incomes.
* **Model & Preprocessing:** Missing values mode/mean imputation, categorical label encoding, `StandardScaler` feature scaling, and Logistic Regression.
* **Performance:** **78.86%** Accuracy.
* **Key Findings:** Credit history record is the single most critical factor in predicting loan status and default risk.
* **GitHub Repository:** [Task 2 Folder on GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-2-Credit-Risk-Prediction)
* **Local Links:** [Local Notebook](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%202%20-%20Credit%20Risk%20Prediction/Task%202%20Credit%20Risk%20Prediction.ipynb) | [Local README.md](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%202%20-%20Credit%20Risk%20Prediction/README.md)

---

### 📉 [Task 3: Customer Churn Prediction](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-3-Customer-Churn-Prediction)
* **Objective:** Classify bank clients who are likely to close their accounts (churn) to assist proactive retention marketing.
* **Dataset:** Bank Churn Modelling Dataset (10,000 customer records).
* **Model & Preprocessing:** Feature selection, forward fill handling, Label Encoding, Random Forest Classifier (100 estimators).
* **Performance:** **86.45%** Accuracy (Precision: 0.75 / Recall: 0.47 for churned customers).
* **Key Findings:** Customers' age, account balances, activity status, and number of purchased bank products strongly determine the probability of churn.
* **GitHub Repository:** [Task 3 Folder on GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-3-Customer-Churn-Prediction)
* **Local Links:** [Local Notebook](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%203%20-%20Customer%20Churn%20Prediction/Task%203%20Customer%20Churn%20Prediction.ipynb.ipynb) | [Local README.md](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%203%20-%20Customer%20Churn%20Prediction/README.md)

---

### 🏥 [Task 4: Predicting Insurance Claim Amounts](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-4-Insurance-Cost-Prediction)
* **Objective:** Build a regression model to predict personal medical insurance charges using demographic and lifestyle factors.
* **Dataset:** Medical Cost Personal Dataset containing features like smoker status, age, BMI, and location.
* **Model & Preprocessing:** Label Encoding, Linear Regression modeling.
* **Performance:** $R^2$ Score: **0.7833** | MAE: **4,186.51** | RMSE: **5,799.59**.
* **Key Findings:** Smoker status is the strongest determinant of higher premium charges, followed by age and BMI.
* **GitHub Repository:** [Task 4 Folder on GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-4-Insurance-Cost-Prediction)
* **Local Links:** [Local Notebook](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%204%20-%20Insurance%20Cost%20Prediction/Task%204%20Insurance%20Cost%20Prediction.ipynb) | [Local README.md](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%204%20-%20Insurance%20Cost%20Prediction/README.md)

---

### 💰 [Task 5: Personal Loan Acceptance Prediction](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-5-EDA)
* **Objective:** Develop a classification model to target banking customers likely to accept personal loan / term deposit offers.
* **Dataset:** Bank Marketing Dataset containing campaign responses, demographic profiles, and financial indicators.
* **Model & Preprocessing:** Encoding categorical columns, `StandardScaler` normalization, and Logistic Regression (up to 3,000 iterations).
* **Performance:** **78.99%** Accuracy (Precision: 0.79, Recall: 0.76 for deposit subscribers).
* **Key Findings:** High-value customers (high average annual balance), certain job categories (management, technicians), and education level strongly correlate with campaign acceptance.
* **GitHub Repository:** [Task 5 Folder on GitHub](https://github.com/Yasir-Khan1921/Developer-Corporation-Data-Science-and-analytics-/tree/main/Task-5-EDA)
* **Local Links:** [Local Notebook](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%205%20-%20Personal%20Loan%20Acceptance/Task%205:%20Personal%20Loan%20Acceptance%20Prediction.ipynb) | [Local README.md](file:///Users/yasirkhan/Desktop/task%20wise%20read%20me.%20file%20/Task%205%20-%20Personal%20Loan%20Acceptance/README.md)
