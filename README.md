# CredX : Credit Risk Modeling

## Overview

**CredX** is a Credit Risk Modeling application built using **Streamlit** and **Scikit-Learn**. The application uses a machine learning model to predict the credit risk of a borrower based on various features such as income, loan amount, delinquency ratio, and more. It calculates the **default probability**, **credit score**, and provides a **rating** for the user.

## Features

- **Input Form** for users to enter financial data:
  - Age
  - Income
  - Loan Amount
  - Loan Tenure (months)
  - Average DPD (Days Past Due)
  - Delinquency Ratio
  - Credit Utilization Ratio
  - Number of Open Loan Accounts
  - Residence Type (Owned, Rented, Mortgage)
  - Loan Purpose (Education, Home, Automobile, Personal)
  - Loan Type (Secured, Unsecured)
  
- **Credit Risk Predictions**:
  - Default Probability
  - Credit Score
  - Rating (Poor, Average, Good, Excellent)

## Requirements

Before running the application, make sure you have the following dependencies installed:

- Python
- Streamlit
- Pandas
- Scikit-Learn
- Joblib
- Numpy

### Installing Dependencies

You can install the required libraries using the following:

```bash
pip install -r requirements.txt
```

## How to Use

1. Clone the repository or download the source code.

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Streamlit application:
   ```bash
   streamlit run main.py
   ```

4. The app will open in your browser where you can input various financial details, and upon pressing the **"Calculate Risk"** button, the app will display:
   - Default Probability
   - Credit Score
   - Rating

## Model Details

The model is a **logistic regression** model trained on various features including:
- Demographics of the borrower (age, income)
- Loan-related data (loan amount, tenure)
- Credit history (delinquency ratio, credit utilization)

It outputs:
- **Default Probability**: The likelihood of default.
- **Credit Score**: A score ranging from 300 to 900.
- **Rating**: A rating such as 'Poor', 'Average', 'Good', or 'Excellent'.
