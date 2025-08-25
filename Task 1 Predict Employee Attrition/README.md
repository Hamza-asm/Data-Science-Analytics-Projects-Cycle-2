
<p align="center">
  <img width="647" height="328" alt="Employee attrition" src="https://github.com/user-attachments/assets/f4064bf2-6248-4b46-8cb1-bf0514b4fdaf" />
</p>


## Overview

This notebook performs exploratory data analysis (EDA), feature engineering, machine learning, and explainable AI on the IBM HR Analytics dataset to uncover patterns, distributions, relationships, and the key drivers behind employee attrition.

## Project Steps

1. **Data Loading:**  
   - Read the HR dataset from CSV using pandas.

2. **Data Cleaning & Preprocessing:**  
   - Drop non-informative columns.
   - Handle missing values and remove duplicates if present.
   - Encode categorical variables and correct data types.

3. **Exploratory Analysis:**  
   - Generate summary statistics (.describe()).
   - Plot distributions using histograms and boxplots to detect outliers.
   - Visualize attrition rate and class imbalance.

4. **Feature Relationships:**  
   - Compute and visualize correlation matrix and heatmap.
   - Examine feature relationships to attrition (e.g., Age, Department, MonthlyIncome).
   - Scatter plots or grouped barplots for key pairs.

5. **Model Building and Explainability:**  
   - Train classification model (Random Forest).
   - Evaluate performance using metrics and confusion matrix.
   - Use SHAP for feature importance and explainability.

6. **Visualization:**  
   - Bar charts, boxplots, pie charts for categorical features.
   - Custom plots using matplotlib and seaborn.

## How to Run

1. Open `Task 1 Predict Employee Attrition.ipynb` in Jupyter Notebook or JupyterLab.
2. Ensure required libraries are installed:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn shap
