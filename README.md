# credit-risk-classification

# Module 12 Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The purpose of this analysis is to be able to predict whether a loan application to a financial institution would become at risk of defaulting based on applicant financial criteria.

* Explain what financial information the data was on, and what you needed to predict.

The data contains information on seven financial aspects of a customer's loan application: Loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derrogatory credit marks, and total debt. 

Based on the data of each loan, the `loan_status` column is marked with a 0, meaning that the loan is healthy, and a 1, meaning that the loan is at high risk of default.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

The variable that this model was aimed at predicting was whether a loan application `loan_status` would become at risk at defaulting.

* Describe the stages of the machine learning process you went through as part of this analysis.

I first split the dataset in two, separating the dependent variable `loan_status` from the independent variables in the rest of the dataset.

I then created training and testing sets to use during modeling using `train_test_split` module from sklearn.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

After splitting the data, I fit the model using `LogisticRegression`.

I fit the results to the actual values in a new dataframe to measure the accuracy.

## Results

* Machine Learning Model 1:
    * Testing Accuracy Score: .992
    * Training Accuracy Score: .991
* Confusion Matrix Results:
    * True Negatives: 18679
    * False Positives: 80
    * False Negatives: 67
    * True Positives: 558


## Summary

From the provided results, it seems that the model is correctly predicting a vast majority of the healthy loans (0 label), as evidenced by the high true negative count. However, the count of false positives suggests that there are instances where the model incorrectly predicts a loan as healthy when it is actually high-risk.

For the high-risk loans (1 label), the model seems to perform exceptionally well, with very few false negatives, indicating that it effectively identifies the majority of high-risk loans.

In conclusion, the logistic regression model appears to predict healthy loans (0 label) quite well, but there may be room for improvement in reducing false positives. Nevertheless, its performance in identifying high-risk loans (1 label) is impressive, with a low false negative rate.
