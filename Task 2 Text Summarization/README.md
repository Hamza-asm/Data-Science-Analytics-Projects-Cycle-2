# Task 2: Text Summarization with CNN/Daily Mail Dataset
---

## Overview

This project implements a text summarization pipeline to generate concise summaries from lengthy news articles using both extractive and abstractive methods. The workflow is demonstrated on the CNN/Daily Mail dataset.

---

## Dataset Description

The [CNN/Daily Mail dataset](https://www.kaggle.com/datasets/gowrishankarp/newspaper-text-summarization-cnn-dailymail) is a widely-used benchmark for news summarization tasks. It contains news articles and corresponding human-written summaries (called "highlights").

- **Files included:**  
  - `train.csv` — training split  
  - `validation.csv` — validation split  
  - `test.csv` — test split  
- **Columns:**  
  - `id`: Unique identifier for each article  
  - `article`: Full news article text  
  - `highlights`: Human-written summary

**To download the dataset from Kaggle via API:**  
```bash
kaggle datasets download -d gowrishankarp/newspaper-text-summarization-cnn-dailymail
```

---

## Project Steps

1. **Data Loading & Inspection:**
    - Load the train, validation, and test CSV splits from the CNN/Daily Mail dataset.
    - Inspect the structure, check the presence of required columns (`article`, `highlights`), and confirm data readiness for processing.

2. **Data Preprocessing:**
    - Clean the data by removing rows with missing or empty articles or highlights.
    - Strip extra whitespace and eliminate duplicate entries to ensure a high-quality input for modeling.

3. **Extractive Summarization:**
    - Implement a baseline extractive method by splitting each article into sentences using spaCy.
    - Score sentences based on word frequency and select the most informative ones as the summary.

4. **Abstractive Summarization:**
    - Use a pre-trained transformer model (such as BART) from HuggingFace’s transformers library to generate new, coherent summaries that may paraphrase or rephrase the original article.

5. **Improvement & Tuning:**
    - Experiment with model generation parameters (e.g., summary length, sampling strategies) to enhance summary quality and fluency.
    - Optionally, discuss the possibility of fine-tuning the model on the dataset for further improvement.

6. **Evaluation:**
    - Test the summarization models on the test set.
    - Compare generated summaries to human-written references using ROUGE metrics and manual review of sample outputs.

7. **Key Insights:**
    - Summarize the main results and lessons learned from the project.
    - Discuss the relative strengths and weaknesses of extractive versus abstractive summarization approaches.

---
## How to Run
  - Place the dataset CSVs in a cnn_dailymail folder in your working directory.
  - Open Task 2 Text Summarization.ipynb in Jupyter Notebook or JupyterLab.
  - Install the dependencies as listed below.
```bash
pip install pandas numpy matplotlib seaborn spacy torch transformers rouge-score
python -m spacy download en_core_web_sm
```
  - Run each cell in order, following markdown explanations at each step.
