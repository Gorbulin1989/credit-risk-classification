# Module 12 Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

ANSWER: The purpose of the analysis is to build and compare machine learning models to predict loan risk using financial information.

* Explain what financial information the data was on, and what you needed to predict.

ANSWER: The data contains information on loans, including loan amount, interest rate, borrower income, number of accounts, and other financial information.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

ANSWER: The task is to predict the risk of a loan, where a loan is classified as high risk if it is likely to default, and low risk otherwise.

* Describe the stages of the machine learning process you went through as part of this analysis.

ANSWER: The stages of the machine learning process include data cleaning and preprocessing, splitting data on features and labels, creating the test and trainig data sets, model selection,  model evaluation, and performance comparison.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

ANSWER: Two main methods were used:
1. Logistic Regression with original data & Logistic Regression with resampled data using RandomOverSampler

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

ANSWER: Two machine learning models were trained and evaluated: a logistic regression model and a RandomOverSampler model.


For the logistic regression model:
For the 0 label, the model has achieved perfect precision, recall, and F1-score of 1.00, indicating that the model has correctly identified all the healthy loans and has not classified any of them as high-risk loans.

For the 1 label, the model has achieved a precision of 0.86, indicating that 86% of the loans predicted as high-risk by the model are actually high-risk. The recall of 0.89 indicates that the model has correctly identified 89% of the high-risk loans. The F1-score of 0.88 indicates that the model has achieved a balance between precision and recall for the high-risk loans.

The accuracy of the model is 0.99, which means that the model has classified 99% of the loans correctly. The macro-averaged F1-score and weighted F1-score are both very high, indicating that the model is performing well overall.

Overall, the logistic regression model is performing very well in predicting both the 0 and 1 labels, with high precision, recall, and F1-score, and a high overall accuracy.


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.


  ANSWER: Based on the classification report, the logistic regression model fit with oversampled data is also performing very well in predicting both the 0 (healthy loan) and 1 (high-risk loan) labels.

For the 0 label, the model has achieved a precision of 1.00, indicating that all the loans predicted as healthy by the model are actually healthy. The recall of 0.99 indicates that the model has correctly identified 99% of the healthy loans. The F1-score of 1.00 indicates that the model has achieved perfect balance between precision and recall for the healthy loans.

For the 1 label, the model has achieved a precision of 0.86, indicating that 86% of the loans predicted as high-risk by the model are actually high-risk. The recall of 1.00 indicates that the model has correctly identified all of the high-risk loans. The F1-score of 0.92 indicates that the model has achieved a good balance between precision and recall for the high-risk loans.

The accuracy of the model is 0.99, which means that the model has classified 99% of the loans correctly. The macro-averaged F1-score of 0.96 and weighted F1-score of 0.99 are also high, indicating that the model is performing well overall.

Overall, the logistic regression model fit with oversampled data is performing very well in predicting both the 0 and 1 labels, with high precision, recall, and F1-score, and a high overall accuracy. The model is also performing better in terms of recall for the high-risk loans, which is an important metric for identifying the high-risk loans correctly.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

ANSWER: Overall, the logistic regression model trained on the oversampled dataset achieved the best performance in terms of both precision and recall for high-risk loans, which is the most important metric for identifying high-risk loans correctly.
The performance of the models varied depending on the resampling method used and the problem being solved.
Based on the analysis, it is recommended to use the logistic regression model trained on the oversampled dataset for predicting loan risk, as it achieved the best performance for identifying high-risk loans.


