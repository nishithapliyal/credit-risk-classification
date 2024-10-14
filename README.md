# Credit Risk Analysis Report

## Overview

- The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers when it comes to loans.
- The financial information included in this dataset included loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks and total debt. All this information is per borrower where each row corresponds to a borrower. The information that is to predicted is the loan status of the borrower.
- The variable to predict is the loan status of the borrower. Where "0" refers to a healthy loan and "1" refers to a high risk loan. In the entire dataset, before splitting into training and test data, there are 75036 borrowers that have a healthy loan (0) status. There are 2500 borrowers that have a high risk loan status. There are significantly more borrowers that have a healthy loan status than those who have a high risk loan status. 
- The analysis started with isolating the features from the value to predict. X was set to the all the features that would be used to predict y (loan status). Then, the dataset was split into training and test data. Then, a logistic regression model was fit to the training data. This model was used to predict values for the X_test data. Finally, a confusion matrix and a classification report was generated to compare the predictions made by the logistic regression model and the true y_test values.
- I used a few methods throughout this analysis. I used the train_test_split method to split my data into training and testing data. I used the LogisticRegression method to create a logistic regression model to train and predict data. I used the confusion_matrix to create a confusion matrix for the predicted data and y_test data. And finally, I used the classification_report method to create a classification report to report the precision, recall, and accuracy for the predicted data and the y_test data.

## Results

- The overall accuracy score of the logistic regression model is 0.99. This means that the model is able to predict the loan status with 99% accuracy.
- For the healthy loans, the model predicts with 100% precision and 99% recall.
  - This means out of all healthy loan predictions, 100% of them are correct.
  - And out of all the healthy loans in the testing dataset, 99% of them were predicted correctly.
- For the high risk loans, the model predicts with 85% precision and 91% recall.
  - This means out of all high risk loan predictions, 85% of them are correct.
  - And out of all the high risk loans in the testing dataset, 91% of them were predicted correctly.

## Summary

The machine learning model predicts with a 99% accuracy overall. It is better at predicting healthy loan statues than high risk loan statues. However, the precison and recall for high risk loan predictions reamins relatively high. I recommend this model for use by the company because of its ability to predict loan statues with high accuracy. 
