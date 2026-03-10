# Customer Churn Prediction using Machine Learning

## Project Overview

Customer churn is a major concern for banks and financial institutions because losing customers can directly impact revenue and business growth. This project focuses on building a **machine learning model that predicts whether a bank customer will leave the bank or continue using its services**.

The model analyzes customer demographic details, financial attributes, and banking activity to identify patterns associated with customer churn. Predicting churn early allows businesses to take proactive actions to retain valuable customers.

---

## Dataset

This project uses the **Bank Customer Churn Dataset**, which contains **10,000 customer records** and multiple attributes describing customer demographics and banking activity.

### Features in the Dataset

* **CreditScore** – Customer’s credit score
* **Geography** – Customer’s country (France, Germany, Spain)
* **Gender** – Male or Female
* **Age** – Age of the customer
* **Tenure** – Number of years the customer has been with the bank
* **Balance** – Account balance
* **NumOfProducts** – Number of bank products used by the customer
* **HasCrCard** – Indicates whether the customer has a credit card
* **IsActiveMember** – Indicates whether the customer is an active member
* **EstimatedSalary** – Estimated annual salary
* **Exited** – Target variable indicating churn (1 = churn, 0 = stay)

The objective of the project is to **predict the value of the `Exited` column**.

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

The following steps were followed to build the churn prediction model:

1. **Data Loading and Exploration**

   * Inspecting dataset structure
   * Checking feature distributions

2. **Data Preprocessing**

   * Removing unnecessary columns such as RowNumber, CustomerId, and Surname
   * Encoding categorical variables

3. **Feature Engineering**

   * Creating additional features such as balance-to-salary ratio

4. **Handling Class Imbalance**

   * Using **SMOTE (Synthetic Minority Oversampling Technique)** to balance the dataset

5. **Model Training**

   * Training a **Gradient Boosting Classifier**

6. **Model Evaluation**

   * Confusion Matrix
   * Precision
   * Recall
   * F1-score
   * Accuracy

7. **Feature Importance Analysis**

   * Identifying the most influential features affecting churn

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

## Feature Importance

Feature importance analysis revealed that the following variables have a strong influence on customer churn:

* Age
* Balance
* Estimated Salary
* Credit Score
* Number of Products
* Tenure

These insights help understand customer behavior and factors that influence churn decisions.

---

## Project Structure

```
Customer-Churn-Prediction
│
├── Churn_Modelling.csv
├── churn_prediction.ipynb
├── README.md
└── requirements.txt
```

---

## How to Run the Project

1. Clone the repository

```
git clone https://github.com/your-github-username/customer-churn-prediction.git
```

2. Navigate to the project folder

```
cd customer-churn-prediction
```

3. Install required libraries

```
pip install -r requirements.txt
```

4. Run the notebook

```
jupyter notebook churn_prediction.ipynb
```

---

## Future Improvements

Possible improvements for this project include:

* Hyperparameter tuning using GridSearchCV
* Testing advanced models such as XGBoost
* Building a dashboard for churn insights
* Deploying the model using FastAPI or Streamlit

---

## Author

**Navya Saravanan**
AI/ML Student

LinkedIn: https://www.linkedin.com/in/your-linkedin-username
