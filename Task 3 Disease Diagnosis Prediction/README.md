<p align="center">
  <img width="579" height="328" alt="HeartDise" src="https://github.com/user-attachments/assets/6bf59332-c640-42e5-9e33-a46c95f08475" />
</p>


---

## Overview

This project develops a machine learning model to predict the likelihood of heart disease based on patient medical data. The workflow covers exploratory analysis, feature selection, model training, evaluation, and provides actionable insights for healthcare professionals.

---

## Dataset Description

The [Heart Disease Dataset](https://www.kaggle.com/datasets/bansalstuti/heart-disease-data) is a commonly used benchmark for medical diagnosis tasks. It contains 303 records of patients, each with clinical features such as age, blood pressure, cholesterol, and more, along with a target variable indicating the presence of heart disease.

**To download the dataset using KaggleHub:**
```python
import kagglehub

# Download latest version
path = kagglehub.dataset_download("bansalstuti/heart-disease-data")

print("Path to dataset files:", path)
```
## Project Steps

1. **Data Loading & Inspection:**
   - Load the heart disease dataset and review its structure and content.
     
2. **Exploratory Data Analysis (EDA):**
   - Visualize feature distributions and analyze relationships between medical variables and disease outcome.

3. **Feature Selection & Scaling:**
   - Assess feature importance, retain all relevant columns, and standardize numeric features to prepare for modeling.
     
4. **Model Training:**
   - Train a Gradient Boosting Classifier to predict heart disease based on patient features.
     
5. **Model Evaluation:**
   - Evaluate the model using F1 Score, AUC-ROC, and confusion matrix to ensure robust predictive performance.
     
6. **Healthcare Insights:**
   - Translate model results into actionable recommendations for early detection, personalized prevention, and resource optimization in healthcare.
---
## How to Run
  - Download the dataset using the KaggleHub code above and place heart_disease_data.csv in your working directory.
  - Open Task 3 Disease Diagnosis Prediction.ipynb in Jupyter Notebook or JupyterLab.
  - Install dependencies as listed below.
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
  - Run each cell sequentially and review the markdown explanations for each step.
