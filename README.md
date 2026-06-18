# Telecom Customer Churn Prediction

## Project Overview

Customer churn is a significant challenge in the telecommunications industry, as losing existing customers directly impacts revenue and increases customer acquisition costs. This project aims to predict customer churn using machine learning techniques and identify the key factors that influence customer retention.

The project involves data preprocessing, exploratory data analysis (EDA), model development, and performance comparison using multiple classification algorithms.

---

## Business Problem

Telecom companies face substantial financial losses when customers switch to competitors. The objective of this project is to develop a predictive model that identifies customers who are likely to churn, enabling businesses to implement proactive retention strategies.

### Business Benefits

* Reduce customer attrition
* Improve customer retention
* Increase customer lifetime value (CLV)
* Optimize marketing campaigns
* Support data-driven decision-making
* Improve overall profitability

---

## Dataset Description

The dataset contains customer demographic information, service subscriptions, billing details, customer value metrics, and churn status.

### Features

| Feature          | Description                       |
| ---------------- | --------------------------------- |
| customerID       | Unique customer identifier        |
| gender           | Customer gender                   |
| SeniorCitizen    | Senior citizen status             |
| Partner          | Whether customer has a partner    |
| Dependents       | Whether customer has dependents   |
| tenure           | Number of months with the company |
| PhoneService     | Phone service subscription        |
| MultipleLines    | Multiple phone lines subscription |
| InternetService  | Internet service type             |
| OnlineSecurity   | Online security subscription      |
| OnlineBackup     | Online backup subscription        |
| DeviceProtection | Device protection subscription    |
| TechSupport      | Technical support subscription    |
| StreamingTV      | Streaming TV subscription         |
| StreamingMovies  | Streaming Movies subscription     |
| Contract         | Contract type                     |
| PaperlessBilling | Paperless billing status          |
| PaymentMethod    | Payment method used               |
| MonthlyCharges   | Monthly bill amount               |
| TotalCharges     | Total amount charged              |
| CLV              | Customer Lifetime Value           |
| AvgMonthlySpend  | Average monthly spending          |
| Churn            | Target Variable                   |

### Target Variable

**Churn**

* Yes → Customer left the company
* No → Customer retained the service

---

## Exploratory Data Analysis (EDA)

Comprehensive exploratory data analysis was conducted to understand customer behavior and identify factors associated with churn.

### Analysis Performed

* Churn distribution analysis
* Customer tenure analysis
* Contract type analysis
* Monthly charges analysis
* Total charges analysis
* Customer Lifetime Value (CLV) analysis
* Average Monthly Spend analysis
* Internet service analysis
* Payment method analysis
* Correlation analysis
* Feature relationship visualization

### Key Findings

* Customers with shorter tenure were more likely to churn.
* Month-to-month contract customers exhibited the highest churn rates.
* Customers with higher monthly charges showed increased churn probability.
* Customers with lower CLV demonstrated a higher tendency to leave.
* Electronic check payment users showed relatively higher churn rates.
* Long-term contract customers displayed stronger retention behavior.
* Average Monthly Spend emerged as an important indicator of customer loyalty.

---

## Data Preprocessing

The following preprocessing steps were performed:

* Removed unnecessary identifiers
* Handled missing values
* Encoded categorical variables
* Feature transformation and cleaning
* Train-test split
* Data scaling where applicable

---

## Machine Learning Models

### Logistic Regression

Logistic Regression was used as a baseline classification model to predict customer churn.

**Advantages**

* Simple and interpretable
* Fast training time
* Provides probability estimates

---

### Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve predictive performance.

**Advantages**

* Handles nonlinear relationships
* Reduces overfitting
* Provides feature importance scores

---

### XGBoost Classifier

XGBoost is a gradient boosting algorithm widely used for classification tasks due to its strong predictive capabilities.

**Advantages**

* High predictive power
* Handles feature interactions effectively
* Built-in regularization

---

## Model Evaluation Metrics

The models were evaluated using:

* Accuracy Score
* Confusion Matrix
* Precision
* Recall
* F1 Score

---

## Model Performance Comparison

| Model               | Accuracy   |
| ------------------- | ---------- |
| Logistic Regression | **80.13%** |
| Random Forest       | **78.64%** |
| XGBoost             | **78.92%** |

### Performance Analysis

* Logistic Regression achieved the highest accuracy of **80.13%**.
* XGBoost achieved an accuracy of **78.92%**.
* Random Forest achieved an accuracy of **78.64%**.
* Logistic Regression outperformed the ensemble models, suggesting that customer churn behavior in this dataset can be effectively captured through linear relationships among customer attributes.

---

## Important Predictors of Churn

Based on exploratory analysis and model interpretation, the most influential features included:

* Contract Type
* Tenure
* Monthly Charges
* Total Charges
* Customer Lifetime Value (CLV)
* Average Monthly Spend
* Internet Service Type
* Payment Method
* Tech Support
* Online Security

These variables significantly influenced customer retention and churn behavior.

---

## Business Recommendations

Based on the findings, telecom companies can:

1. Focus retention efforts on customers with low tenure.
2. Encourage customers to switch from month-to-month contracts to longer-term plans.
3. Closely monitor customers with declining CLV.
4. Offer personalized incentives to high-value customers.
5. Improve customer engagement programs for customers identified as high churn risk.
6. Strengthen technical support services to improve customer satisfaction.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost

---

## Results

The project successfully developed predictive models to identify customers likely to churn.

Among all evaluated models, **Logistic Regression emerged as the best-performing model with an accuracy of 80.13%**, outperforming both Random Forest and XGBoost.

The findings demonstrate that customer demographics, subscription behavior, billing patterns, Customer Lifetime Value (CLV), and spending behavior provide valuable insights into customer retention.

The model can assist telecom companies in proactively identifying at-risk customers and implementing targeted retention strategies to reduce revenue loss and improve customer loyalty.

---

## Future Improvements

* Hyperparameter tuning using GridSearchCV
* SMOTE for class imbalance handling
* Cross-validation
* SHAP-based model explainability
* Customer segmentation analysis
* Deployment using Streamlit
* Real-time churn prediction dashboard

---

## Conclusion

This project demonstrates how machine learning can be applied to solve a real-world customer retention problem in the telecommunications industry. By leveraging customer demographics, service subscriptions, billing information, Customer Lifetime Value (CLV), and spending behavior, the developed model successfully predicts customer churn and provides actionable insights that can support strategic business decisions and improve long-term profitability.
