# TELCO-Customer-Retention
## Overview
TelCo® is one of the main players in the telecommunications market in the United States of America. They mainly provide phone and internet services
Competitors include AT&T, Verizon, Cricket, etc. However, nowadays a significant problem is Customer Churn. Communications companies are now engaged in battles to attract each other’s customers while retaining their own. Customers switching from one company to another is called churn. Churn is expensive all around. One company must spend on incentives to attract a customer while another company loses revenue when the customer departs. 

We are thinking of how to increase customer retention using data science, or in other words, how to detect accurately customers that are likely to churn so as to take measures to retain them? In this project, we apply supervised data mining algorithm to solve the classification problem which would predict whether a customer will churn or not based on historical trends.

## Data Understanding and Manipulation
* Sample size: 7083 observations
* Time Period: 1 month
* Geography: 1 Region
* Features to predict Churn: 19 variables
* Data source: Kaggle
## Model Building
* K-NN
* Decision Tree
* Logistic Regression

(Grid search method is performed for all three algorithms to find the best parameters in the respective corresponding to the algorithm.Cross Validation is performed to select the final best model amongst the three models built.)

We chose the decision tree model to be our final model based on the following criteria:
* The goal is to prevent losing out on predicting customers who could churn i.e. to maximize churn recall.
* Model should be easy to understand and visualize so as to increase credibility with the stakeholders.

## Model Evaluation
Applying accuracy rate and confusion matrix combined with precision, recall and F1-measure, the final model performed 76% accuracy on test data. Besides, the recall rate of 'Churn'(which we think is important) is 0.63, which indicates that how many of real churn customers are detected.

## Insights and Recommendations

According to the model result, the fact that customers in their initial few (1-4) months churn the most has been reinforced by the model results. Besides, We recommend that TelCo® should focus on customers who have month-to-month contract and have chosen ‘Fiber Optic’ for their internet service since they have the most likelihood to churn.
