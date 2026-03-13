# Customer Churn Prediction using Machine Learning

## Project Overview

Customer retention is a major challenge for telecom companies. Losing customers (churn) directly affects revenue and long-term business growth.

This project builds a **machine learning model that predicts whether a customer is likely to churn** based on demographic information, service usage, and billing details.

The goal is to help companies identify at-risk customers early so they can take preventive actions such as targeted offers or improved customer support.

---

## Dataset

The dataset used in this project is the **IBM Telco Customer Churn dataset**.

It contains customer information such as:

* Customer demographics
* Subscription services
* Billing information
* Contract type
* Churn status

Important columns include:

* `Gender`
* `SeniorCitizen`
* `TenureMonths`
* `InternetService`
* `Contract`
* `MonthlyCharges`
* `TotalCharges`
* `ChurnValue` (target variable)

Where:

* **0 → Customer stays**
* **1 → Customer churns**

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Machine Learning Workflow

The project follows a standard machine learning pipeline:

1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Data Encoding
6. Train/Test Split
7. Model Training
8. Model Evaluation
9. Feature Importance Analysis
10. Prediction

---

## Model Used

The model used in this project is:

**Random Forest Classifier**

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

---

## Model Performance

The trained model achieves approximately **80% accuracy** on the test dataset.

Evaluation metrics used:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## Key Insights

Analysis of the model shows that the following factors strongly influence customer churn:

* Contract type (Month-to-month contracts churn more)
* Tenure (new customers churn more often)
* Monthly charges
* Internet service type
* Online security services

These insights can help telecom companies design better customer retention strategies.

---

## Project Structure

```
customer-churn-project
│
├── data
│   └── Telco-Customer-Churn.xls
│
├── notebooks
│   └── churn_analysis.ipynb
│
├── models
│   └── churn_model.pkl
│
└── README.md
```

---

## How to Run the Project

1. Clone the repository

```
git clone <repository-link>
```

2. Install required libraries

```
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
```

3. Run the Jupyter Notebook

```
jupyter notebook
```

4. Open:

```
churn_analysis.ipynb
```

and execute the cells step-by-step.

---

## Future Improvements

Possible improvements for this project include:

* Building a web interface using Flask or FastAPI
* Deploying the model as an API
* Trying advanced models such as XGBoost or LightGBM
* Hyperparameter tuning for better accuracy

---

## Conclusion

This project demonstrates how machine learning can be used to **predict customer churn and provide actionable insights for businesses**. By identifying customers at risk of leaving, companies can take proactive steps to improve retention and customer satisfaction.
