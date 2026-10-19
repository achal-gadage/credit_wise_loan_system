# credit_wise_loan_system

## Overview
CreditWise Loan System is a machine learning project that predicts loan approval outcomes based on applicants' financial information, credit scores, employment details, and other relevant attributes.
The project aims to support faster and more consistent loan assessments by identifying patterns in historical loan application data.

## Problem Statement
SecureTrust Bank faces challenges with manual loan verification, including time-consuming assessments, inconsistent decisions, and financial risks. CreditWise uses machine learning classification models to predict whether a loan application should be **Approved or Rejected**, supporting the final decision made by a loan officer.

## Dataset
Each row represents a loan applicant.

Key features include:
- Financial: Applicant income, co-applicant income, savings, and existing loans.
- Credit: Credit score and Debt-to-Income (DTI) ratio.
- Loan Details: Loan amount, loan term, and loan purpose.
- Personal: Age, gender, marital status, dependents, education level, and property area.
- Target Variable: `Loan_Approved`

## Tools & Technologies
- Python: Core programming
- Pandas & NumPy: Data manipulation and preprocessing
- Matplotlib & Seaborn : Exploratory data analysis and visualization
- Scikit-learn:  Machine learning and model evaluation
- Jupyter Notebook: Development and experimentation

## Project Workflow
1. Data Loading & Exploration: Loaded the dataset and examined data types, summary statistics, and missing values.
2. Data Cleaning: Handled missing numerical values using mean imputation and categorical values using mode imputation.
3. EDA: Analyzed loan approval distribution, income patterns, credit scores, DTI ratios, savings, and outliers.
4. Feature Engineering: Encoded categorical variables, removed the applicant ID, and created squared features for credit score and DTI ratio.
5. Model Training: Split the data into training and testing sets and applied feature scaling.
6. Model Evaluation: Trained and compared Logistic Regression, K-Nearest Neighbors (KNN), and Gaussian Naive Bayes using classification metrics.

## Machine Learning Models
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes
The notebook identifies **Gaussian Naive Bayes as the preferred model based on precision**.

## Results
The models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

These metrics help assess classification performance and the risks of incorrect loan approval predictions.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/achal-gadage/credit_wise_loan_system.git
   ```
2. Navigate to the project directory:
   ```bash
   cd credit_wise_loan_system
   ```
3. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
4. Ensure the dataset `loan_approval_data.csv` is available in the expected project directory.
5. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
6. Open `credit_loan.ipynb` and run the cells in sequence.

## Project Focus: Data Cleaning | EDA | Feature Engineering | Classification | Machine Learning | Model Evaluation
