# Credit-Risk-Classification
### Background

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
### Before You Begin

Create a new repository for this project called credit-risk-classification. Do not add this homework to an existing repository.
Clone the new repository to your computer.
Inside your credit-risk-classification repository, create a folder titled "Credit_Risk."
Inside the "Credit_Risk" folder, add the credit_risk_classification.ipynb and lending_data.csv files found in the "Starter_Code.zip" file.
Push your changes to GitHub.

## Instructions

The instructions for this Challenge are divided into the following subsections:
- Split the Data into Training and Testing Sets
- Create a Logistic Regression Model with the Original Data
- Write a Credit Risk Analysis Report
- Split the Data into Training and Testing Sets

Open the starter code notebook and use it to complete the following steps:
- Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
        ### NOTE
        A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.
        Split the data into training and testing datasets by using train_test_split.
- Create a Logistic Regression Model with the Original Data

Use your knowledge of logistic regression to complete the following steps:
- Fit a logistic regression model by using the training data (X_train and y_train).
- Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
- Evaluate the model’s performance by doing the following:
- Generate a confusion matrix.
- Print the classification report.

Answer the following question: 
- How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

Write a Credit Risk Analysis Report
-Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.
Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:
- An overview of the analysis: Explain the purpose of this analysis.
- The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
- A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.


# Loan Risk Prediction Analysis

## Overview of the Analysis

The purpose of this analysis is to build a machine learning model to predict loan risk based on various borrower-related factors such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. By accurately predicting whether a loan is high-risk (1) or healthy (0), financial institutions can make more informed lending decisions and mitigate potential risks.

The model selected for this analysis is a logistic regression model due to its simplicity and effectiveness in binary classification problems.

## Results

The performance of the logistic regression model is evaluated based on the following metrics:
- Accuracy Score: The overall accuracy of the model in predicting both healthy and high-risk loans.
- Precision: The percentage of loans predicted as high-risk that are actually high-risk.
- Recall: The percentage of actual high-risk loans that the model correctly identified.

## Model Performance:
- Accuracy Score: 99%
- Precision for Class 0 (Healthy Loan): 1.00 (100%)
- Recall for Class 0 (Healthy Loan): 1.00 (100%)
- F1-Score for Class 0 (Healthy Loan): 1.00
- Precision for Class 1 (High-Risk Loan): 0.86 (86%)
- Recall for Class 1 (High-Risk Loan): 0.91 (91%)
- F1-Score for Class 1 (High-Risk Loan): 0.88

## Summary

The logistic regression model demonstrates strong performance with an overall accuracy of 99%. The model performs exceptionally well in predicting healthy loans, with perfect precision and recall for the 0 label. For high-risk loans, the model achieves a precision of 86% and a recall of 91%, indicating that while it is very good at identifying high-risk loans, there is still room for improvement.

## Recommendation:
Given the high overall accuracy and strong performance on both healthy and high-risk loans, this model is a viable option for use by the company. It can accurately identify high-risk loans in most cases, allowing the company to make more informed lending decisions. However, if even greater precision in predicting high-risk loans is desired, further refinement (such as balancing the dataset or exploring other algorithms) could be pursued.