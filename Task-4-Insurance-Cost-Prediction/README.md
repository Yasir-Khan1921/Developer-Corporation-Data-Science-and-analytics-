# Task 4: Predicting Insurance Claim Amounts
### DevelopersHub Corporation — Data Science & Analytics Internship

**Author:** Yasir Khan  
**Date:** June 2026

---

## 📌 Task Objective
The objective of this project is to develop a regression model that estimates medical insurance charges/claim amounts based on personal attributes. Accurately estimating these amounts helps insurance companies set appropriate premium rates and anticipate financial expenditures.

---

## 📊 Dataset Overview
The project is built on the **Medical Cost Personal Dataset** (saved as `insurance copy.csv`), containing demographic and behavioral attributes of insurance beneficiaries. Features include:
* `age`: Age of primary beneficiary
* `sex`: Gender (female, male)
* `bmi`: Body Mass Index, providing an indicator of body fat relative to height
* `children`: Number of dependents covered by health insurance
* `smoker`: Smoking status (yes, no)
* `region`: Geographic region in the US (northeast, southeast, southwest, northwest)
* **Target Variable:** `charges`: Medical costs billed by health insurance

---

## ⚙️ Methodology & Implementation
The workflow implemented in the Jupyter notebook `Task 4 Insurance Cost Prediction.ipynb` includes:

1. **Environment Setup & Data Import:** Imported critical data science libraries and loaded `insurance copy.csv`.
2. **Data Inspection:** Checked shape, variables, data types, and verified that no missing values exist.
3. **Feature Preprocessing:**
   * Used `LabelEncoder` to transform categorical attributes (`sex`, `smoker`, `region`) into numerical values.
   * Split the dataset into training (80%) and testing (20%) samples using `train_test_split`.
4. **Exploratory Data Analysis (EDA):**
   * Plotted a correlation heatmap to analyze how personal characteristics associate with final billed charges.
5. **Model Building & Evaluation:**
   * Trained a **Linear Regression** model.
   * Evaluated model predictions using standard regression metrics: Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and the Coefficient of Determination ($R^2$ Score).

---

## 📈 Performance & Results
* **Model Used:** Linear Regression
* **Regression Metrics Achieved:**
  * **Mean Absolute Error (MAE):** **4,186.51**
  * **Mean Squared Error (MSE):** **33,635,210.43**
  * **Root Mean Squared Error (RMSE):** **5,799.59**
  * **Coefficient of Determination ($R^2$ Score):** **0.7833**
* **Key Findings:**
  * The model explains approximately **78.33%** of the variance in medical insurance charges.
  * Smoking status, age, and BMI are highly correlated with increased medical charges. Smoker status is particularly the strongest driver of high insurance claims.

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
2. Place the dataset `insurance copy.csv` on your Desktop, or adjust the path inside the notebook:
   ```python
   df = pd.read_csv("/Users/yasirkhan/Desktop/insurance copy.csv")
   ```
3. Run Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open and execute `Task 4 Insurance Cost Prediction.ipynb`.
