# Superstore Marketing Campaign Analysis

## Project Overview
This project focuses on building a machine learning classification model to predict whether existing customers of a superstore are likely to subscribe to a newly launched Gold Membership offer. The membership provides a 20% discount on all purchases at a discounted price during a year-end campaign.
To optimize campaign costs and improve conversion rates, the business aims to identify customers with a higher likelihood of accepting the offer. This project uses exploratory data analysis (EDA) and Logistic Regression to uncover influential factors and predict customer responses effectively.



## Business Objective
- Predict the probability of a customer accepting the Gold Membership offer
- Identify key demographic, behavioral, and purchasing factors influencing customer decisions
- Support targeted marketing campaigns to reduce operational costs


  
## Dataset Description
- Source: Historical campaign data from the previous year
- Rows: 2,240 customers
- Columns: 22 features
- Target Variable: Response (Accept / Refuse)



## Data Cleaning & Preparation
- Handled missing values by removing rows with null Income
- Verified absence of duplicate customer IDs
- Converted categorical target variables (Response, Complain) into meaningful labels
- Removed outliers (customers aged over 100 years)
- Encoded categorical variables using Label Encoding
- Dropped non-informative columns (Customer ID, enrollment date)



## Exploratory Data Analysis (EDA)
Key analyses performed include: 
- Income distribution and its impact on campaign response
- Customer complaints vs campaign acceptance
- Purchase behavior comparison between accepting and non-accepting customers
- Product-wise spending patterns
- Engagement metrics across web, catalog, and store channels
- Age and recency analysis to understand purchasing behavior
Visualizations were created using Matplotlib and Seaborn to highlight trends and relationships.


## Modeling Approach
- Algorithm Used: Logistic Regression
- Imbalance Handling: SMOTE (Synthetic Minority Oversampling Technique)
- Train-Test Split: 80% training / 20% testing
- Evaluation Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC
- Model Performance
Training Accuracy: ~75%
Testing Accuracy: ~75%
- Balanced precision and recall across both classes
- ROC curve demonstrates stable classification performance
  



## Key Insights
- Higher income customers show a greater likelihood of accepting the membership
- Customers with recent purchases are more responsive to campaigns
- Spending on meat, gold, and catalog purchases strongly correlates with positive response
- Customers with teenagers at home are less likely to accept the offer



## Future Enhancements
- Experiment with advanced models (Random Forest, XGBoost)
- Perform feature selection and hyperparameter tuning
- Deploy the model as a REST API
- Integrate real-time campaign scoring
