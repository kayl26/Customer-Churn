# Customer-Churn

## Business Understanding

1. Identify the business problem and associate a type of analytical problem.

    a. Business Problem: 

     * Some customers from the Telco company are no longer using the phone and internet services provided by the company. They are choosing to leave for a variety of reasons. We want to figure out why they are leaving and try to find ways to prevent others from leaving.

    b.	Analytical Problem: 

      * The company can analyze certain factors that are common between all customers who chose to leave and determine which factor is the most contributing.
  
    c.	Goal: 
      
      * Try to see if the machine learning algorithms can predict whether a customer will churn and if there are any ways, we can prevent the customers from leaving.


## Data Preparation

2. What data will you use and will there be any issues with its collection or preparation?

    a. We found a dataset from IBM that consists of 7000 records and 33 columns, where the target variable is "Churn Label" and indicates whether a customer will stay or leave the company.

    b. We need to check for any missing data as well as drop any columns that may not be providing much value.

    c. The data is skewed more in favor of customers who stayed with the company, need to balance data effectively when creating different datasets.

    d. Created graphs to represent the relationship of variables to the target variable.
   
      * Customer Characteristics: such as gender, whether they have a partner or any dependents and how long they've been with the company.

      * Types of services offered: such as phone, internet and streaming.

      * Contract Length: such as monthly, 1 year or 2 years.

      * Fees, Billing and Payment methods.

      * Data also includes reason for leaving, which can be used to develop possible mitigating actions.


## Modeling

3. What techniques will you use and how will the data correspond to the variables you will need?

    a. Focus on classification techniques to predict based on a variety of factors which customers will stay loyal to the company and which won’t.

    b. Our target variable for this dataset is Churn Label which tell us whether or not a certain customer has stayed or left.

    c. Use some machine learning algorithms such as: Logistic Regression and Random Forest.
	

## Evaluation

4. How will the model be evaluated?

    a. The data will be separated into training, test, and validation sets. 
  
      * The largest portion (I.e., 80%) will be used for training the model, with the test data used to assess the model fit and to tune the parameters. The validation data will be used to determine the final model performance and to determine whether the model can be deployed.
        
   b. Use statistical tools such as Confusion Matrix, F1 score. These metrics include the following:
   
      * TP: our model predicts that customers will stay, and they do

      * TN: our model predicts that customer will leave, and they do

        * Can offer promotions to try to incentivize customers to staying

      * FP: our model predicts customers stay but they leave

        * Worst type because we would lose people, we didn’t think we would

      * FN: our model predicts customer leaves, but they stay


        
   c. Create a ROC graph for a visual representation of model performance.
   

## Deployment

5. How will the model be deployed?

    a. Insightful Promotions:

      * We want to utilize the insights from the model to create personalized offers for customers identified as at-risk of churning. One possible way could be segmentation, where we group customers based on churn probability and tailor promotions for each segment.

    b. Customer Engagement:

      * We will establish mechanisms to gather feedback from customers who were considering leaving but decided to stay due to interventions. Also, conducting regular surveys to gauge customer satisfaction and identify areas for improvement.

    c. Continuous Monitoring:

      * Implement a system for real-time monitoring of customer behavior and model predictions so that we can continuously update the model to adapt to changing customer preferences and market dynamics.

