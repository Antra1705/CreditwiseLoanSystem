# Creditwise Loan System

## Overview

The **Creditwise Loan System** is a machine learning project designed to predict whether a loan application will be approved or denied based on an applicant's financial and demographic information. The project leverages Python and various data science libraries to perform data preprocessing, exploratory data analysis (EDA), feature engineering, and predictive modeling.

---

## Dataset

The project uses the `loan_approval_data.csv` dataset, which contains **1,000 records** and **20 features**.

### Financial Features
- Applicant_Income
- Coapplicant_Income
- Credit_Score
- Savings
- Collateral_Value
- Existing_Loans
- DTI_Ratio

### Loan Details
- Loan_Amount
- Loan_Term
- Loan_Purpose

### Demographic Features
- Age
- Gender
- Marital_Status
- Dependents
- Education_Level
- Employment_Status
- Employer_Category
- Property_Area

### Target Variable
- Loan_Approved (Yes/No)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Requirements

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Project Workflow

### 1. Data Loading & Inspection
- Loaded the dataset using Pandas.
- Examined data types and missing values.
- Generated descriptive statistics to understand data distribution.

### 2. Data Preprocessing
#### Handling Missing Values
- Numerical features were imputed using the mean value.
- Categorical features were imputed using the most frequent value.

### 3. Exploratory Data Analysis (EDA)
- Analyzed the distribution of the target variable (`Loan_Approved`).
- Visualized feature relationships using:
  - Histograms
  - Bar plots
  - Pie charts
  - Correlation heatmaps
- Identified patterns and trends affecting loan approval decisions.

### 4. Feature Encoding
#### Label Encoding
Applied to:
- Education_Level
- Loan_Approved

#### One-Hot Encoding
Applied to:
- Employment_Status
- Marital_Status
- Loan_Purpose
- Property_Area
- Gender
- Employer_Category

### 5. Feature Scaling
- Standardized numerical features using `StandardScaler`.
- Ensured all features contributed equally during model training.

### 6. Model Training
- Split the dataset into training and testing sets using `train_test_split`.
- Trained a **Logistic Regression** classifier.
- Evaluated model performance on unseen test data.

---

## Model Used

### Logistic Regression
Logistic Regression was selected as the baseline classification model due to its:
- Simplicity
- Interpretability
- Efficiency on structured tabular data

The model predicts whether a loan application is likely to be **Approved** or **Rejected**.

---

## Project Structure

```text
CreditwiseLoanSystem/
│
├── credit_wise.ipynb
├── loan_approval_data.csv
├── README.md
└── .gitignore
```

---

## How to Run

### Clone the Repository

```bash
git clone https://github.com/Antra1705/CreditwiseLoanSystem.git
```

### Navigate to the Project Directory

```bash
cd CreditwiseLoanSystem
```

### Launch Jupyter Notebook

```bash
jupyter notebook credit_wise.ipynb
```

### Execute the Notebook

Run all cells sequentially to:
- Preprocess the data
- Perform exploratory data analysis
- Train the machine learning model
- Evaluate prediction performance

---

## Future Improvements

- Implement additional machine learning models such as:
  - Random Forest
  - XGBoost
  - Support Vector Machine (SVM)
- Perform hyperparameter tuning.
- Build a web application using Flask or Streamlit.
- Deploy the model for real-time loan approval prediction.

---

## Author

**Antra Singh**

GitHub: https://github.com/Antra1705
