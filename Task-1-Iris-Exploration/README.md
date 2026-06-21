# Task 1: Exploring and Visualizing the Iris Dataset
### DevelopersHub Corporation — Data Science & Analytics Internship
**Author:** Yasir Khan  
**Date:** June 2026
## Task Objective
The primary objective of this task is to perform an in-depth Exploratory Data Analysis (EDA) on the classic **Iris Dataset** to analyze, summarize, and visualize the relationships and distribution of characteristics of three species of Iris flowers:
* *Iris Setosa*
* *Iris Versicolor*
* *Iris Virginica*
##  Dataset Overview
The dataset contains **150 samples** (50 per species). For each sample, the following four numerical features were recorded:
1. **Sepal Length** (in cm)
2. **Sepal Width** (in cm)
3. **Petal Length** (in cm)
4. **Petal Width** (in cm)
##  Methodology & Implementation
The workflow implemented in the Jupyter notebook `Task_1_Iris_Exploration_and_Visualization.ipynb` includes:
1. **Environment Setup & Data Import:** Loaded the dataset using `pandas` and checked the basic attributes using `.shape`, `.columns`, and `.head()`.
2. **Data Cleaning & Quality Check:**
   * Checked for missing values (`.isnull().sum()`).
   * Checked for duplicate entries (`.duplicated()`).
   * Verified data types.
   * *Outcome:* The dataset is perfectly clean with no missing values, correct data types, and a balanced class distribution.
3. **Exploratory Data Analysis (EDA):**
   * **Scatter Plots:** Explored relationships between variables (e.g., Sepal Length vs Sepal Width, Petal Length vs Petal Width).
   * **Pair Plots:** Generated pairwise distributions across all features to see multi-dimensional clusters.
   * **Histograms:** Checked frequency distributions and density trends of each feature.
   * **Box Plots:** Analyzed the spread of values and identified outliers across species.
   * **Correlation Heatmap:** Checked the linear relationships between numeric features using Pearson Correlation.
   * **Violin Plots:** Combined box plots and kernel density estimation to view probability density distributions.
##  Key Insights
* **Species Separability:** *Iris Setosa* forms a highly distinct cluster and can be separated easily from the other two species using any combination of sepal and petal features.
* **Top Distinguishing Features:** *Petal Length* and *Petal Width* provide the clearest boundary separation between *Versicolor* and *Virginica*, which otherwise show minor overlaps in sepal dimensions.
* **High Correlations:** A strong positive correlation exists between **Petal Length** and **Petal Width** (0.96), and between **Petal Length** and **Sepal Length** (0.87).
* **Outliers:** A few outliers were detected in *Virginica* for the Sepal Width feature.
##  Tech Stack & Libraries
* **Language:** Python 3
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`
* **Environment:** Jupyter Notebook
##  How to Run the Notebook[Uploading Task_1_Iris_Exploration_and_Visualization.ipynb…]()

1. Install requirements:
   ```bash
   pip install pandas numpy matplotlib seaborn notebook
   ```
2. Navigate to this directory and launch Jupyter:
   ```bash
   jupyter notebook
   ```
3. Open `Task_1_Iris_Exploration_and_Visualization.ipynb` and run all cells.

