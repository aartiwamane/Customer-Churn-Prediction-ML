# Customer Churn Prediction using Machine Learning

## Overview

This project implements a Customer Churn Prediction system using **Logistic Regression**, a supervised machine learning classification algorithm.

The model analyzes customer information such as Age, Tenure, Monthly Charges, and Support Calls to predict whether a customer is likely to leave a service.

The project also demonstrates model evaluation and model serialization using the Joblib library, allowing the trained machine learning model to be saved and reused.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Joblib

## Machine Learning Algorithm

**Logistic Regression**

Logistic Regression is a supervised classification algorithm used to predict categorical outcomes. In this project, it is used to classify customers into churn and non-churn categories.

## Dataset Features

The model uses the following input features:

| Feature | Description |
|---|---|
| Age | Customer's age |
| Tenure | Duration of customer association |
| MonthlyCharges | Monthly charges paid by the customer |
| SupportCalls | Number of support calls made |
| Churn | Target variable (0 or 1) |

## Project Workflow

1. Import required Python libraries.
2. Load the customer churn dataset using Pandas.
3. Separate independent features and the target variable.
4. Split the dataset into training and testing sets (80:20).
5. Train the Logistic Regression model.
6. Generate predictions using the testing dataset.
7. Evaluate model performance using:
   - Accuracy Score
   - Confusion Matrix
8. Save the trained model using Joblib.

## Model Persistence using Joblib

One of the important features of this project is saving the trained machine learning model using Joblib.

```python
joblib.dump(model, "ML_Customer_Churn.pkl")
```

This saves the trained model into a `.pkl` file, which can be loaded later without training the model again.

To load the saved model:

```python
import joblib

model = joblib.load("ML_Customer_Churn.pkl")
```

## Project Structure

```text
Customer-Churn-Prediction-ML/
│
├── ML_Customer_churn_Final.py
├── customer_churn.csv
├── ML_Customer_Churn.pkl
├── requirements.txt
└── README.md
```

**Note:** The `.pkl` file is generated after executing the Python script. The dataset must be placed in the same directory as the Python script.

## Installation and Execution

### 1. Clone the Repository

```bash
git clone https://github.com/USERNAME/Customer-Churn-Prediction-ML.git
```

### 2. Navigate to the Project Directory

```bash
cd Customer-Churn-Prediction-ML
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Execute the Python Script

```bash
python ML_Customer_churn_Final.py
```

## Output

The program displays:

- Customer dataset
- Model accuracy score
- Confusion matrix
- Model saving confirmation

The trained model is saved as `ML_Customer_Churn.pkl`.

## Learning Outcomes

- Understanding supervised machine learning classification.
- Implementing Logistic Regression using Scikit-learn.
- Working with training and testing datasets.
- Evaluating classification models.
- Understanding model persistence using Joblib.
- Saving and loading trained machine learning models.

## Author

Aarti Wamane

**Domain:** Machine Learning | Python | Data Science
