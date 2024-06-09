# Module 12 Report Template

## Overview of the Analysis

- Lending companies provide loans or properties to borrowers with the expectation of repayment. Credit risk arises when borrowers fail to repay, causing financial losses for lenders. To assess this risk, machine learning can be used to analyze historical lending data from a peer-to-peer lending service. The goal is to build a model that identifies the creditworthiness of borrowers.

- In this analysis, a Logistic Regression model was developed to classify loans as either low-risk (healthy) or high-risk (non-healthy) based on their status. The model achieved a 99% accuracy score. However, the recall value for predicting non-healthy loans was 0.91, compared to 0.99 for healthy loans, indicating a better performance in predicting healthy loans. This disparity is attributed to the imbalanced dataset, with a majority of data points classified as healthy loans.

- Out of the 18,765 loan status's that are healthy/low-risk the model predicted 18,663 as healthy correctly and 102 as healthy incorrectly.

- Out of the 619 loan status's that are non-healthy/high-risk, the model predicted 563 as non-healthy correctly and 56 as non-healthy incorrectly.

## Results

- Overall all the model generated an accuracy score of 99%, but much of that was due to an imbalance in the data

- With the imbalance in data the model is more likely to make the following mistakes:
o Classifying a non-healthy (high-risk) loan as a healthy (low-risk) loan.
o Classifying a healthy (low-risk) loan as a non-healthy (high-risk) loan.

- According to the recall score for the model, the model made mistakes 1% of the time when predicting healthy loans but made mistakes 9% of the time when predicting non-healthy loans.
- In terms of precision, the model had a 100% precision when predicting healthy/low-risk loans, but that was not the case when it came to predicting non-healthy/high-risk loans, where the model had an 85% precision

## Summary

A lending company needs a model that accurately classifies healthy and non-healthy loans to avoid costly mistakes:

- Misclassifying healthy loans as non-healthy can result in losing customers.
- Misclassifying non-healthy loans as healthy can result in financial losses.
While the model performed well predicting the healthy loans, it did not have the same level of success predicting non-healthy loans, and the sample size just isn’t sufficient to show that it can be successful doing so in the future.

With that being the case, I would recommend the lending company use the model to quickly decipher if a loan candidate would be a low-risk client, but they should do further evaluations when the model predicts a client maybe high risk, and not simply take what the model says as truth.
