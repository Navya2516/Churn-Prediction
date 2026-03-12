# Customer Churn Prediction using Machine Learning

## Project Overview

Customer churn is a significant challenge for banks and financial institutions because losing customers directly impacts revenue and business growth. This project develops a **machine learning model to predict whether a bank customer will leave the bank or continue using its services**.

The model analyzes customer demographic details, financial attributes, and banking activity to identify patterns associated with churn. Predicting churn early allows organizations to take proactive actions to retain valuable customers.

---

## Dataset

This project uses the **Bank Customer Churn Dataset**, which contains **10,000 customer records** with multiple features describing customer demographics, financial information, and banking activity.

### Features in the Dataset

* **CreditScore** – Customer’s credit score
* **Geography** – Customer’s country (France, Germany, Spain)
* **Gender** – Male or Female
* **Age** – Age of the customer
* **Tenure** – Number of years the customer has been with the bank
* **Balance** – Account balance
* **NumOfProducts** – Number of bank products used
* **HasCrCard** – Whether the customer owns a credit card
* **IsActiveMember** – Indicates if the customer actively uses bank services
* **EstimatedSalary** – Estimated annual salary
* **Exited** – Target variable (1 = churn, 0 = customer stays)

The objective is to **predict the `Exited` variable** using machine learning techniques.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn (SMOTE)

---

## Machine Learning Workflow

The project follows a structured machine learning pipeline:

1. **Data Loading and Exploration**
2. **Data Preprocessing**

   * Removing irrelevant columns
   * Encoding categorical variables
3. **Feature Engineering**

   * Creating additional features such as balance-to-salary ratio
4. **Handling Class Imbalance**

   * Using **SMOTE (Synthetic Minority Oversampling Technique)**
5. **Model Training**

   * Gradient Boosting Classifier
6. **Model Evaluation**

   * Confusion Matrix
   * Precision, Recall, F1-score
   * Accuracy
7. **Feature Importance Analysis**

---

## Model Performance

**Algorithm Used:** Gradient Boosting Classifier

Accuracy achieved on the test dataset: **89%**

### Classification Metrics

| Metric    | Non-Churn (0) | Churn (1) |
| --------- | ------------- | --------- |
| Precision | 0.88          | 0.90      |
| Recall    | 0.91          | 0.87      |
| F1 Score  | 0.90          | 0.89      |

The model demonstrates balanced performance in predicting both churn and non-churn customers.

---

## Project Structure

```
Customer-Churn-Prediction
│
├── Churn_Modelling.csv
├── churn_prediction.ipynb
├── Churn Prediction.mp4
└── README.md
```

---

---

## Author

**Navya Saravanan**
AI/ML Student

LinkedIn:
https://www.linkedin.com/in/navya-saravanan-8aa481311/

