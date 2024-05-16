# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The purpose of this analysis is to be able to predict whether a loan application to a financial institution would become at risk of defaulting based on applicant financial criteria.

* Explain what financial information the data was on, and what you needed to predict.

The data contains information on seven financial aspects of a customer's loan application: Loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derrogatory credit marks, and total debt. 

Based on the data of each loan, the "loan_status" column is marked with a 0, meaning that the loan is healthy, and a 1, meaning that the loan is at high risk of default.f

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.

I first split the dataset in two, separating the dependent variable "loan_status" from the independent variables in the rest of the dataset.



* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
