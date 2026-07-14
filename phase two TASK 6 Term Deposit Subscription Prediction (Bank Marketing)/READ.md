# Task 6: Term Deposit Subscription Prediction (Bank Marketing)
### DevelopersHub Corporation — Data Science & Analytics Advanced Internship Tasks

## Overview
This repository contains the implementation for Task 1 of the DevelopersHub Corporation Advanced Internship. The objective of this project is to analyze telemarketing campaign data from a retail bank and build machine learning classifiers to predict whether a customer will subscribe to a term deposit. To provide transparency and trust in the model's decisions, we use Explainable AI (LIME) to interpret individual predictions and derive actionable business strategies.

## Objective
- Predict if a bank customer will subscribe to a term deposit (`deposit` = 'yes' or 'no').
- Train and evaluate Logistic Regression (baseline) and Random Forest (advanced ensemble) classifiers.
- Prevent data leakage by building preprocessing steps into isolated training pipelines.
- Use LIME to explain individual predictions, highlighting the key features driving the positive and negative probabilities.
- Conduct customer behavior analysis to identify highly receptive segments and provide marketing recommendations.

## Dataset
- **Name**: Bank Marketing Dataset (UCI Machine Learning Repository)
- **Shape**: 11,162 rows, 17 columns
- **Features**: Customer demographics (age, job, marital, education), financial status (balance, housing, loan), and campaign metrics (contact type, call duration, days since last contact, previous outcomes).
- **Target**: `deposit` ('yes' / 'no'). The dataset is relatively balanced (52.6% 'no', 47.4% 'yes').

## Tools and Technologies
- **Python 3.14.0**
- **Libraries**: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `lime`
- **Environment**: Jupyter Notebook

## Project Structure
```text
task_1_bank_marketing/
├── data/
│   └── bank.csv
├── notebooks/
│   └── bank_marketing_classification.ipynb
├── README.md
└── requirements.txt
```

## Methodology
1. **Initial Inspection**: Verified shapes, types, missing values, duplicates, and checked for 'unknown' category placeholders.
2. **Train/Test Split**: 80/20 split stratified by target to preserve classes and avoid data leakage.
3. **Preprocessing Pipeline**:
   - Numerical columns: Scaled using `StandardScaler`.
   - Categorical columns: One-Hot Encoded using `OneHotEncoder(handle_unknown='ignore', drop='first')`.
4. **Modeling**: Built preprocessing pipelines with `LogisticRegression` and `RandomForestClassifier`.
5. **Evaluation**: Computed Accuracy, Precision, Recall, F1-Score, ROC-AUC, and plotted Confusion Matrices and ROC curves.
6. **Interpretability (XAI)**: Initialized LIME Tabular Explainer on category-coded inputs. Explained the local boundaries of the first 5 test predictions.
7. **Customer Behavior Analysis**: Grouped categorical behaviors and visualised boxplots/countplots to verify key feature correlations.

## Results
The performance of the trained models on the test set (2,233 instances) is summarized below:

| Metric | Logistic Regression | Random Forest |
| :--- | :---: | :---: |
| **Accuracy** | 82.53% | 85.71% |
| **Precision** | 82.75% | 82.73% |
| **Recall** | 79.77% | 88.28% |
| **F1-Score** | 81.23% | 85.41% |
| **ROC-AUC** | 90.73% | 91.87% |

### Confusion Matrix Comparison
- **Logistic Regression**:
  - True Negative (no): 999 | False Positive (yes): 176
  - False Negative (no): 214 | True Positive (yes): 844
- **Random Forest**:
  - True Negative (no): 980 | False Positive (yes): 195
  - False Negative (no): 124 | True Positive (yes): 934

### Best Model Selection
**Random Forest Classifier** is the superior model. It achieves a significantly higher **Recall (88.28% vs 79.77%)** and **F1-Score (85.41% vs 81.23%)** while keeping accuracy at **85.71%**. In bank marketing, capturing more potential subscribers (Recall) is highly valuable to minimize missed opportunities.

## Key Findings & XAI Insights
By using LIME to analyze predictions, we identified the top drivers for term deposit subscriptions:
1. **Call Duration (`duration`)**: The single most powerful predictor. A longer call represents high engagement. The mean duration for subscribers is **537.0 seconds** (~9 minutes) compared to **221.0 seconds** for non-subscribers.
2. **Previous Success (`poutcome` = 'success')**: Out of the customers who subscribed in a previous campaign, **91.3%** subscribed again.
3. **No Housing Loan (`housing` = 'no')**: Customers without a housing loan subscribe at a **57.0%** rate compared to **36.6%** for those with housing loans.
4. **Mobile Contact (`contact` = 'cellular')**: Leads to a positive impact in the model predictions compared to 'unknown' or traditional landline channels.

## Business Insights & Recommendations
1. **Prioritize Past Conversion Successes**: Re-engage clients whose previous campaign outcome was 'success' (91.3% conversion rate).
2. **Target Debt-Free Profiles**: Target campaign lists on customers without housing loans as they have more disposable income and financial flexibility.
3. **Optimize Calling Scripts**: Sales scripts should be restructured to maintain interest past the 4-minute mark, since call length strongly drives subscription probability.
4. **Prioritize Mobile Numbers**: Cellular contact is associated with positive weights in predictions, so prioritize cell numbers over landlines.

## Conclusion
We developed an end-to-end classification pipeline that predicts customer term deposit subscriptions with **85.71% accuracy** and **91.87% ROC-AUC** using a Random Forest classifier. By integrating LIME, the model's choices are made transparent, allowing the bank to move away from cold calling to targeted, relation-based conversion marketing.

---
*Note: All scores and metrics are calculated from actual execution of the preprocessing and training pipeline on the bank marketing dataset.*
