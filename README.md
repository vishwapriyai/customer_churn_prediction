# customer_churn_prediction


# Telecommunication Customer Churn Prediction

This project aims to predict customer churn in a telecommunication company using machine learning techniques.

## Overview

Customer churn, also known as customer attrition, occurs when customers stop doing business with a company. Predicting customer churn is crucial for businesses to identify at-risk customers and take proactive measures to retain them.

In this project, we use a dataset from a telecommunication company containing information about customers, such as their demographics, services subscribed to, and churn status. We build a predictive model using a RandomForestClassifier to predict customer churn based on historical data.

## Data

The dataset used in this project is `WA_Fn-UseC_-Telco-Customer-Churn.csv`, containing the following columns:

- `customerID`: Unique identifier for each customer
- `gender`: Customer's gender (Male/Female)
- `SeniorCitizen`: Whether the customer is a senior citizen (0/1)
- `Partner`: Whether the customer has a partner (Yes/No)
- `Dependents`: Whether the customer has dependents (Yes/No)
- `tenure`: Number of months the customer has stayed with the company
- `PhoneService`: Whether the customer has a phone service (Yes/No)
- `MultipleLines`: Whether the customer has multiple lines (Yes/No/No phone service)
- `InternetService`: Customer's internet service type (DSL, Fiber optic, No)
- `OnlineSecurity`: Whether the customer has online security (Yes/No/No internet service)
- `OnlineBackup`: Whether the customer has online backup (Yes/No/No internet service)
- `DeviceProtection`: Whether the customer has device protection (Yes/No/No internet service)
- `TechSupport`: Whether the customer has tech support (Yes/No/No internet service)
- `StreamingTV`: Whether the customer has streaming TV (Yes/No/No internet service)
- `StreamingMovies`: Whether the customer has streaming movies (Yes/No/No internet service)
- `Contract`: The contract term of the customer (Month-to-month, One year, Two year)
- `PaperlessBilling`: Whether the customer has paperless billing (Yes/No)
- `PaymentMethod`: The customer's payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
- `MonthlyCharges`: The amount charged to the customer monthly
- `TotalCharges`: The total amount charged to the customer
- `Churn`: Whether the customer churned or not (Yes/No)

## Methodology

1. **Data Preprocessing**: 
   - Convert categorical variables into dummy/indicator variables.
   - Handle missing values in the `TotalCharges` column.
   - Drop unnecessary columns such as `customerID`.
   
2. **Model Building**: 
   - Split the dataset into training and testing sets.
   - Build a RandomForestClassifier model and train it on the training data.

3. **Model Evaluation**:
   - Make predictions on the testing data.
   - Evaluate the model using accuracy, confusion matrix, classification report, and ROC curve.
   - Visualize the confusion matrix.

## Results

- The RandomForestClassifier model achieved an accuracy of approximately XX% in predicting customer churn.
- The ROC curve indicates good performance of the model with an area under the curve (AUC) of approximately XX%.

## Conclusion

The predictive model developed in this project can effectively identify customers at risk of churn, allowing the telecommunication company to take proactive measures to retain them and improve customer satisfaction and loyalty.

