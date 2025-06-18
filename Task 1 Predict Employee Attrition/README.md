# Task 1: Predict Employee Attrition Using HR Analytics

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
   - Train classification models (Random Forest, Logistic Regression).
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
