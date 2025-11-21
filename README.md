# Credit Classification Project

A machine learning project to classify creditworthiness (or credit risk) based on financial and demographic features. The analysis, modeling, and evaluation are done in a Jupyter Notebook (`Credit_Classification_Project.ipynb`).

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Motivation](#motivation)  
3. [Dataset](#dataset)  
4. [Methodology](#methodology)  
5. [Models](#models)  
6. [Evaluation](#evaluation)  
7. [How to Run](#how-to-run)  
8. [Dependencies](#dependencies)  
9. [Results & Findings](#results--findings)  
10. [Future Work](#future-work)  
11. [Contributing](#contributing)  
12. [License](#license)  

---

## Project Overview

This project aims to predict credit risk or classify creditworthiness using a data-driven approach. By applying standard machine learning techniques, the goal is to distinguish between “good” and “bad” credit (or other risk categories) to support decision-making in lending or financial assessment.

## Motivation

Credit risk assessment is a critical challenge for financial institutions: lending money safely involves predicting which applicants are likely to default. Automating credit classification using ML can:

- Improve the efficiency of underwriting  
- Reduce human bias  
- Help organizations make data-driven decisions  
- Potentially increase financial inclusion

## Dataset

- Size: 23 columns, each containing 100k values  
- Key features (e.g., age, income, debt, credit history, etc.)  
- Preprocessing steps: cleaning, handling dataypes, handling missing values, feature engineering  

## Methodology

1. **Exploratory Data Analysis (EDA):**  
   - Summary statistics  
   - Feature distributions  
   - visualizing to extract insights  

2. **Data Preprocessing:**  
   - Handling missing values  
   - Encoding categorical variables  
   - Feature scaling / normalization  

3. **Modeling:**  
   - Train-test split  
   - Model training  

4. **Evaluation & Validation:**  
   - Confusion matrix  
   - Precision, recall, F1-score  
   - ROC-AUC

## Models

In the notebook, the following models (or similar) are used:

- Logistic Regression    
- Random Forest  
- Gradient Boosting      

Gradient Boosting had the overall best AUC curve. Therefore, i believe this is best model for prediction.


## Evaluation

For each model:

Logistic Regression (Default Parameters):

Train Accuracy: 0.78755

Test Accuracy: 0.786


Logistic Regression (Tuned Parameters):

Train Accuracy: 0.7892875

Test Accuracy: 0.7877


Logistic Regression (After tuning the threshold for best f1 score):

Accuracy: 0.78155

Precision: 0.6097738876732313

Recall: 0.7116104868913857

F1: 0.6567680100557781



Logistic Regression (confusion matrix):

array([[11451,  2675],
       [ 1694,  4180]])


Logistic Regression (After balancing the data which i believed there wes no need):

Accuracy: 0.77895

Precision: 0.6030058131291649

Recall: 0.7240381341504937

F1: 0.6580026301539413



Randon Forest and GBM (Untuned):

RF Train Accuracy: 0.999975

RF Test Accuracy: 0.89735

GBM Train Accuracy: 0.8329

GBM Test Accuracy: 0.82905



Random Forest (Tuned):

RF Train Accuracy: 0.8495875

RF Test Accuracy: 0.8417



Random Forest (Confusion Matrix):

array([[12957,  1169],
       [ 1997,  3877]])


Gradient Boosting (after alot of tuning):

Training Accuracy: 0.900025

Test Accuracy: 0.87065



GBM (Confusion Matrix):

array([[12973,  1153],
       [ 1434,  4440]])


AUC:

Logistic Regression: 0.82

Random Forest: 0.89

GBM: 0.93





## How to Run

To run this project locally:
1. Clone the repository:

   ```bash
   git clone https://github.com/arminmoradpour77-ux/Credit-Classification-project.git
   cd Credit-Classification-project
