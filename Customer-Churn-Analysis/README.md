# Customer Churn Analysis and Prediction

## Project Overview

Customer Churn Analysis and Prediction is a Machine Learning project that analyzes customer data and predicts whether a customer is likely to leave a telecom company.

The project uses customer information such as tenure, monthly charges, contract type, internet services, and payment methods to identify patterns associated with customer churn.

The goal is to help businesses understand why customers leave and identify customers who may need retention offers or additional support.

## Problem Statement

Customer churn is a major challenge for telecom companies. Losing customers can affect revenue and business growth.

This project explores customer behavior and builds Machine Learning models to predict whether a customer will stay or leave the company.

## Dataset

- Dataset: IBM Telco Customer Churn
- Total records: 7,043
- Features: 19 after removing the customer ID
- Target variable: Churn
- Target classes: Yes and No

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. Data Collection – Loaded the telecom customer churn dataset.
2. Data Cleaning – Converted TotalCharges into numeric format and handled missing values.
3. Exploratory Data Analysis – Analyzed churn distribution, contract types, customer tenure, and monthly charges.
4. Feature Preparation – Separated numerical and categorical features.
5. Data Preprocessing – Used median imputation and standard scaling for numerical data, and most-frequent imputation and One-Hot Encoding for categorical data.
6. Model Training – Trained Logistic Regression and Balanced Logistic Regression models.
7. Model Evaluation – Evaluated the models using accuracy, precision, recall, F1-score, confusion matrix, and ROC-AUC.

## Model Results

| Metric | Logistic Regression | Balanced Logistic Regression |
|---|---:|---:|
| Accuracy | 80.55% | 73.81% |
| Churn Precision | 66% | 50% |
| Churn Recall | 56% | 78% |
| Churn F1-score | 60% | 61% |
| ROC-AUC | 0.842 | 0.841 |

## Key Business Insights

- Customers with month-to-month contracts have a higher churn rate (42.71%).
- Customers with two-year contracts have a lower churn rate (2.83%).
- Customers who churned had lower average tenure than customers who stayed.
- Customers who churned had higher average monthly charges.

These findings can help telecom companies identify customer groups that may require better retention strategies.

## Conclusion

The project demonstrates how Machine Learning can be used to analyze customer behavior and predict churn.

The balanced Logistic Regression model identified 78% of actual churners in the test dataset, compared with 56% for the original Logistic Regression model. This makes it useful when identifying potential customer losses is a priority.

## How to Run the Project

1. Clone the repository.
2. Install the required dependencies:

   `pip install -r requirements.txt`

3. Open the Jupyter Notebook:

   `notebooks/customer_churn_analysis.ipynb`

4. Run the notebook cells in order.

## Future Improvements

- Experiment with Random Forest and other classification algorithms.
- Perform hyperparameter tuning.
- Improve churn prediction using additional customer behavior features.
- Build a simple web application to make predictions for new customers.