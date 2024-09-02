# Predicting Telecom Customer Churn

## Project Overview

In the rapidly evolving telecom sector in India, understanding customer behavior and predicting churn is crucial for enhancing service quality and customer satisfaction. This project aims to explore the dynamics of customer behavior and demographics to predict churn using two comprehensive datasets from major telecom partners: Airtel, Reliance Jio, Vodafone, and BSNL.

## Dataset Summary

### `telecom_demographics.csv`
Contains information related to Indian customer demographics:

| Variable             | Description                                      |
|----------------------|--------------------------------------------------|
| `customer_id`        | Unique identifier for each customer.             |
| `telecom_partner`    | Telecom partner associated with the customer.    |
| `gender`             | Gender of the customer.                          |
| `age`                | Age of the customer.                             |
| `state`              | Indian state where the customer is located.      |
| `city`               | City where the customer is located.              |
| `pincode`            | Pincode of the customer's location.              |
| `registration_event` | Customer's registration event with the telecom partner.|
| `num_dependents`     | Number of dependents the customer has.           |
| `estimated_salary`   | Customer's estimated salary.                     |

### `telecom_usage.csv`
Contains information about the usage patterns of Indian customers:

| Variable            | Description                                      |
|---------------------|--------------------------------------------------|
| `customer_id`       | Unique identifier for each customer.             |
| `call_duration`     | Total duration of calls made by the customer.    |
| `num_sms_sent`      | Number of SMS messages sent by the customer.     |
| `data_usage`        | Total amount of data used by the customer.       |
| `churn`             | Indicates whether the customer churned (1 = Yes, 0 = No).|

## Project Steps

### 1. Data Preprocessing

- **Data Merging**: Combined demographic and usage data using `customer_id`.
- **Calculating Churn Rate**: Analyzed the churn rate in the dataset.
- **Encoding Categorical Features**: Converted categorical features into numerical values using One-Hot Encoding.
- **Scaling Features**: Standardized features using `StandardScaler` for better model performance.

### 2. Model Building

- **Logistic Regression**: Built and trained a Logistic Regression model to predict customer churn.
- **Random Forest Classifier**: Built and trained a Random Forest model to predict customer churn.

### 3. Model Evaluation

- **Confusion Matrix**: Evaluated models using confusion matrices.
- **Classification Report**: Assessed model performance through precision, recall, F1-score, and accuracy.
- **Model Comparison**: Compared the accuracy of Logistic Regression and Random Forest models to determine which performed better.

### 4. Results

- **Higher Accuracy**: The Random Forest model achieved a higher accuracy compared to Logistic Regression.

## Conclusion

This project provides valuable insights into customer churn behavior in the Indian telecom sector. The findings can help telecom companies enhance customer retention strategies and improve overall service quality.

---
