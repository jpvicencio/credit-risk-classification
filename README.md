# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis is to evaluate the credit risk associated with loan applications using a logistic regression model.
The objective was to develop a model that can accurately classify loans as either healthy (0) or high-risk (1), thereby assisting lenders in making informed decisions regarding loan approvals and risk management.

Financial Information

The dataset is consists of financial information related to loan applications, including various borrower information (ex. income) and loan attributes (ex. loan size). The primary target variable to predict was the loan_status, which indicates whether a loan is healthy (0) or high-risk (1). This classification is crucial for lenders to mitigate potential defaults and manage their portfolios effectively.

Variables Overview

The dataset included several features, such as income, credit score, loan amount, and more. The target variable, loan_status, had the following distribution:
    Healthy Loans (0): 18,759 instances
    High-Risk Loans (1): 625 instances

This significant class imbalance highlights the importance of careful model evaluation to ensure the high-risk loans are accurately predicted.

Stages of the Machine Learning Process

1. Data Preparation
2. Data Splitting into Training and Testing Sets using train_test_split
3. Model Development - Fitted a logistic regression model and saved predictions on the test set 
4. Credit Risk Analysis Report by evaluating the model
   
Methods Used

The primary algorithm employed in this analysis was `LogisticRegression`. This algorithm is well-suited for predicting probabilities and making classifications based on input features, making it an ideal choice for the credit risk evaluation context.


## Results

Accuracy Score: 0.99
Precision for Healthy Loans (0): 1.00
Recall for Healthy Loans (0): 1.00
F1-Score for Healthy Loans (0): 1.00
Precision for High-Risk Loans (1): 0.87
Recall for High-Risk Loans (1): 0.95
F1-Score for High-Risk Loans (1): 0.91

## Summary

Logistic regression is a solid choice for credit risk analysis since credit risk is a binary classification problem (healthy vs. high-risk loans) and logistic regression fits naturally for such scenarios.  It also enables stakeholders to easily interpret the results. Lastly, it is efficient with less resource-intensive compared to more complex models which makes it faster to train and suitable for smaller datasets.

The model shows great performance in predicting healthy loans, with perfect precision and recall. For high-risk loans, while the precision is lower, the recall is still high, which means that it effectively identifies most of the high-risk loans while having some false positives. Over-all, the model  demonstrates excellent accuracy and reliability, but there might still be room for improvement in predicting the high-risk loans.
    Precision - The model perfectly predicts healthy loans (precision of 1.00), but it has a lower precision for high-risk loans, indicating that about 13% of the high-risk predictions were incorrect (false positives).

    Recall - The model perfectly identifies healthy loans but is also quite effective at identifying high-risk loans, capturing 95% of them. However, this means that 5% of high-risk loans were missed (false negatives).

    F1 Score - The model performs very well for healthy loans and reasonably well for high-risk loans.

    Support - There are significantly more healthy loans compared to high-risk loans, which may affect the model's ability to predict the high-risk loan accurately.


