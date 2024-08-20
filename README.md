# Credit Risk Analysis Report

## An Overview of the Analysis

  The goal of this analysis is to create a machine learning algorithm that uses a Linear Regression model to predict if a borrower is more likely to have a healthy or high-risk loan using a dataset of historical lending activity. The dataset used for the predicitions contains more than 77,000 rows of loan data that indicate the borrower's income, interest rate, loan size, debt to income ratio, number of accounts, loan status, and derogatory marks. For this analysis, we were trying to predict the loan status; whether a borrower would have a healthy loan or a high-risk loan. A healthy loan appears as a '0' and a high-risk loan appears as a '1'. 

  
  For the machine learning process, the data is imported and stored in a Pandas dataframe so the columns can be evaluated. Then the data is separated into features and labels. The labels determine the status of loan, healthy (0) or high-risk (1). The features are used to train and test the model. The train_test_split function is then implemented to separate the features and labels data into training and testing datasets. The training dataset is used to train the model, and the testing dataset is used to evaluate the model. A Logisitic Regression model is then imported, instantiated, and fitted with the training data. After fitting the model with the training data, a list of predictions is generated using the testing data. These predictions are then evaluated based on accuracy score, a confusion matrix, and a classification report. 
  
## The Results

Machine Learning, Logistic Regression
- Accuracy: 99%
- Precision:
  * Healthy Loans: 100%
  * High-Risk Loans: 85%
- Recall
  * Healthy Loans: 99%
  * High-Risk: 91%

## Summary

The logistic regression model does a very good job at prediciting healthy loans with a perfect precision score. Though there are not as many high-risk loans in the dataset, the model still does an adequate job of prediciting unhealthy loans. The imbalance in data for high-risk loans could be the cause of disparities in the scores.
