🏦 Customer Churn Prediction (Bank Customers)
📌 Introduction
Customer churn is a major challenge in the banking industry because losing customers leads to reduced revenue and higher acquisition costs. The objective of this project is to develop a machine learning model that predicts whether a customer will leave the bank based on demographic and financial information. These insights can help banks design proactive retention strategies.

📂 Dataset
Name: Churn Modelling Dataset

Size: 10,000 customer records, 14 features

Features include:

Demographics: Age, Gender, Geography

Banking info: CreditScore, Balance, Tenure, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary

Target: Exited (1 = churned, 0 = retained)

🛠️ Methodology
1. Data Cleaning
Dropped irrelevant identifiers: RowNumber, CustomerId, Surname.

Verified no missing values.

2. Feature Encoding
Gender → Label Encoding (Male = 1, Female = 0).

Geography → One-Hot Encoding (France, Spain, Germany).

3. Exploratory Data Analysis (EDA)
Churn distribution shows ~20% customers exited.

Boxplots revealed older customers and inactive members are more likely to churn.

Correlation heatmap highlighted moderate relationships between age, balance, and churn.

4. Model Training
Split dataset: 80% training, 20% testing.

Trained a Random Forest Classifier.

Achieved accuracy: 86.6%.

5. Evaluation
Precision (churned customers): 0.77

Recall (churned customers): 0.46

F1-score (churned customers): 0.57

Confusion matrix showed strong performance on non-churned customers, moderate recall on churned customers.

6. Feature Importance
Top predictors of churn:

Age

Balance

Number of Products

IsActiveMember

Geography (Germany/Spain)

📊 Results
The Random Forest model achieved ~87% accuracy.

Key insight: Older, inactive customers with higher balances are more likely to churn.

Geography also plays a role, with German customers showing higher churn rates.
