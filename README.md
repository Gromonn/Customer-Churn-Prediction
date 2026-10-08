# Customer Churn Prediction

A machine learning project for predicting customer churn using customer demographic, account, and service-related information.

## Project Objective

Customer churn refers to customers discontinuing a service or relationship with a company.

The objective of this project is to analyze customer characteristics and build artificial neural network (ANN) models that can predict whether a customer is likely to churn.

## Dataset

The dataset contains customer information including:

- Customer demographics
- Tenure
- Contract type
- Internet service
- Monthly charges
- Total charges
- Customer churn status

The target variable is **Churn**, which indicates whether the customer left the service.

## Exploratory Data Analysis

The project explores:

- Dataset structure and data types
- Missing values
- Customer churn distribution
- Churn across different contract types
- Churn across different tenure groups

These analyses help identify patterns associated with customer churn.

## Data Preprocessing

The following preprocessing steps were performed:

- Converted `TotalCharges` to numeric format
- Handled missing values
- Removed the `customerID` column
- Encoded the target variable
- Split the data into training and testing sets
- Standardized numerical features
- One-hot encoded categorical features

## Machine Learning Models

Three Artificial Neural Network (ANN) models were developed and compared:

### Model 1 — Baseline ANN

A basic neural network was developed to establish a baseline performance.

### Model 2 — ANN with Dropout

Dropout regularization was introduced to help reduce overfitting.

### Model 3 

A wider neural network architecture was tested to evaluate whether additional model capacity improved performance.

Early stopping was also used during training to prevent unnecessary training when validation performance stopped improving.

##Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Training performance was also visualized using accuracy plots.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- TensorFlow / Keras
- Google Colab

## 📁 Project Structure

```text
Customer-Churn-Prediction/
│
├── data/
│   └── customer churn dataset
│
├── notebooks/
│   └── customer_churn_prediction.ipynb
│
├── src/
│
└── README.md
