# Customer Churn Prediction using Machine Learning

## 📌 Project Overview

This project focuses on predicting whether a customer will leave a company or service using Machine Learning techniques.

The project uses the **Telco Customer Churn Dataset** and applies different Machine Learning models along with Ensemble Learning techniques such as **Bagging, Boosting, and Stacking**.

The performance of the models is compared using **Accuracy and F1 Score** to identify the best prediction model.

## 🎯 Objectives

- Predict customer churn.
- Train different Machine Learning models.
- Apply Ensemble Learning techniques.
- Compare model performance.
- Find the best prediction model.

## 📊 Dataset

**Dataset:** Telco Customer Churn Dataset

- Total Customers: 7,043
- Total Columns: 21
- Target Variable: `Churn`
- Target Values: `Yes / No`

### Important Features

- Tenure
- Monthly Charges
- Total Charges
- Contract
- Internet Service
- Payment Method

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

1. Load the dataset using Pandas.
2. Remove the `customerID` column.
3. Convert `TotalCharges` into numeric format.
4. Remove missing values.
5. Apply Label Encoding to categorical values.
6. Split the dataset into 80% training data and 20% testing data.

## 🤖 Machine Learning Models

Three basic Machine Learning models were used:

### 1. Logistic Regression

Logistic Regression predicts the probability of customer churn.

### 2. Decision Tree

Decision Tree uses conditions or questions to reach a final prediction.

### 3. K-Nearest Neighbors (KNN)

KNN predicts the result using similar customers and majority voting.

## 🔥 Ensemble Learning

Ensemble Learning combines multiple models to improve prediction performance.

### Bagging – Random Forest

Random Forest is used for Bagging. Multiple models work independently and their results are combined.

### Boosting – Gradient Boosting

Gradient Boosting trains models sequentially, where later models try to improve the errors made by previous models.

### Stacking

Stacking combines predictions from:

- Logistic Regression
- Decision Tree
- KNN

A final **Logistic Regression model** is used as the meta-model to combine their predictions.

## 🔄 Implementation Flow

```text
Customer Churn Dataset
        ↓
Data Preprocessing
        ↓
Train / Test Split
        ↓
Logistic Regression | Decision Tree | KNN
        ↓
Bagging | Boosting | Stacking
        ↓
Compare Accuracy & F1 Score
        ↓
Select Best Model
```

## 📈 Model Performance

| Model | Accuracy | F1 Score |
|---|---:|---:|
| Logistic Regression | 78.54% | 0.551 |
| Decision Tree | 72.49% | 0.501 |
| KNN | 77.26% | 0.509 |
| Random Forest (Bagging) | 79.25% | 0.556 |
| Gradient Boosting | **79.53%** | **0.561** |
| Stacking | 79.46% | 0.559 |

## 🏆 Best Model

**Gradient Boosting** performed the best among the tested models.

- Accuracy: **79.53%**
- F1 Score: **0.561**

Therefore, Gradient Boosting was selected as the best prediction model for this project.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook
- Machine Learning
- Ensemble Learning

## 📁 Project Files

```text
Customer-Churn-ML-Ensemble/
│
├── customer_churn.csv
├── Untitled.ipynb
├── Customer_Churn_ML_Ensemble_Presentation.pptx
└── README.md
```

## 📌 Conclusion

Customer churn prediction was successfully implemented using Machine Learning.

Three basic Machine Learning models were trained, followed by Bagging, Boosting, and Stacking techniques. Accuracy and F1 Score were used to compare the models.

Among all the tested models, **Gradient Boosting achieved the best performance with 79.53% accuracy and 0.561 F1 Score**.

## 👨‍💻 Author

**Pranav Thorat**

MSc Computer Science

Machine Learning Practical
