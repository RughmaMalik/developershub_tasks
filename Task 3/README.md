# Customer Churn Prediction (Bank Customers)

## Objective
Predict whether a bank customer is likely to leave the bank (churn) using machine learning techniques.

## Dataset
- **Source:** Kaggle – Churn Modelling Dataset  
- **Columns:**
   - Gender, Age  
   - Tenure, Balance, CreditScore, Geography   
   - NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary
- **Link:** [Kaggle Dataset](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling)

## Steps Performed

1. Data Preparation: eliminated irrelevant columns (such as RowNumber, CustomerId, and Surname) to simplify the dataset.
2. Encoding Categorical Variables:
   - Applied Label Encoding to the Gender feature.
   - Used One-Hot Encoding for the Geography attribute.
3. Model Development: trained a Random Forest Classifier on the processed data.
4. Feature Contribution Analysis: determined which features most strongly influence customer churn.

## How to Run
1. Open the notebook in Google Colab.  
2. Upload the dataset (`Churn_Modelling.csv`) when prompted.  
3. Run all cells to reproduce results.
