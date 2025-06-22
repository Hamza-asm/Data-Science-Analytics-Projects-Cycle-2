# Task 4: Loan Default Prediction – Lending Club

---

## Overview

This project builds a machine learning model to predict the likelihood of loan default using financial data from Lending Club. The workflow covers data preprocessing, class imbalance handling, model training, evaluation, and provides practical recommendations for lenders to minimize default risk.

---

## Dataset Description

The [Lending Club Loan Dataset (2007–2011)](https://www.kaggle.com/datasets/imsparsh/lending-club-loan-dataset-2007-2011) contains detailed financial and application data for thousands of loans issued over several years. Each record represents an applicant and includes features like loan amount, interest rate, term, grade, employment information, credit history, and the final loan status (default or fully paid).

- **Data Dictionary:**  
  Accompanied by a `Data_Dictionary.xlsx` file, which provides definitions and explanations for all columns in the main data file. This helps clarify the meaning of each field and supports proper feature selection and interpretation.

**To download the dataset using KaggleHub:**
```python
import kagglehub

# Download latest version
path = kagglehub.dataset_download("imsparsh/lending-club-loan-dataset-2007-2011")

print("Path to dataset files:", path)
```
## Project Steps

1. **Data Loading & Inspection:**
   - Load the Lending Club loan dataset (`loan.csv`) and review its structure and contents.
   - Use the data dictionary file (`Data_Dictionary.xlsx`) to clarify the meaning of each column for proper feature selection and interpretation.

2. **Data Preprocessing:**
   - Handle missing values by dropping columns with excessive gaps and imputing values where appropriate.
   - Drop irrelevant or sparse columns (e.g., IDs), encode categorical variables, and convert the target loan status to a binary default indicator.
   - Address class imbalance with SMOTE to ensure the model learns from both defaulted and non-defaulted loans.

3. **Model Training:**
   - Train a LightGBM classifier on the cleaned, balanced dataset to predict whether an applicant will default on their loan.

4. **Model Evaluation:**
   - Evaluate model performance using precision, recall, F1 score, and a confusion matrix to assess both sensitivity and reliability of predictions.

5. **Reporting and Recommendations:**
   - Summarize model results and generate actionable recommendations for lenders, such as integrating predictive risk tools into the loan approval process and prioritizing manual review for high-risk applicants.

---

## How to Run
  - Download the dataset using the KaggleHub code above and place loan.csv and Data_Dictionary.xlsx in your working directory.

  - Open Task 4 Loan Default Prediction.ipynb in Jupyter Notebook or JupyterLab.

  - Install dependencies as listed below.
```bash
pip install pandas numpy matplotlib seaborn scikit-learn lightgbm imbalanced-learn
```
  - Run each notebook cell in sequence, following the markdown explanations for each step.
