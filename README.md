## Customer Segmentation and RFM Analysis

#### Introduction

In retail, it's always important to analyze customer types (RFM analysis) and predict their future behavior to make better business decisions. In this case study, we will create several machine learning models to answer different problems.

#### RFM Analysis

**RFM** stands for **Recency**, **Frequency**, and **Monetary** value (how recently, how often and how much did they buy). These RFM metrics are important indicators of a user’s behavior because the frequency and monetary value affect a user’s lifetime value, and recency affects retention, a measure of engagement.

RFM factors illustrate these facts:
1. **Recency (R)**: Who has purchased recently? Number of days since last purchase. (Least recency)
2. **Frequency (F)**: Who has purchased frequently? Total number of purchases. (High frequency)
3. **Monetary Value (M)**: Who has a high purchase amount? Total money spent. (High monetary)

Recency                 | Frequency                       | Monetary
----------------------- | ------------------------------- | ------------------------
R-Tier-1 (most recent)  | F-Tier-1 (most frequent)        | M-Tier-1 (highest spend)
R-Tier-2                | F-Tier-2                        | M-Tier-2 
R-Tier-3 (least recent) | F-Tier-3 (only one transaction) | M-Tier-3 (lowest spend)

Each of the three variables (Recency, Frequency, and Monetary) usually consists of 3 equal groups, which creates 27 (3x3x3) different customer segments. 

For more details, click [here](https://rpaudel42.github.io/pages/predicting_customer/predicting_customer.html).

#### File Description

This repository includes three Jupyter notebooks for three case studies using different datasets: 

* "Classification_Purchase-Again.ipynb":
  + Uses two datasets called "transaction_data.xlsx" and "product_data.xlsx"
  + Cleans, processes, and aggregates the data
  + Creates a machine learning model (type: classification, algorithm: support vector machine) to predict whether a customer will purchase again
* "RFM_Segmentation_Online-Retail.ipynb":
  + Uses a dataset called "Online_Retail.xlsx"
  + Determines and visualizes different customer segments and the amount spent by each segment
  + Visualizes high growth customers and the amount spent by this type of customers
* "Classification_Predict-High-Potential-Customer.ipynb":
  + Uses a dataset called "customer.csv"
  + Determines and visualizes different customer segments and the amount spent by each segment
  + Visualizes high growth customers and the amount spent by this type of customers
  + Creates a machine learning model (type: classification, algorithm: logistic regression, with selected features) to predict high potential customers
