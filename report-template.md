# Module 12 Report Template

## Overview of the Analysis
The purpose of this analysis was to observe the accuracy of supervised machine learning models on the real world example of loan risks. In this example we used logarithmic regression models to classify data with financial information such as borrowers loan size, income, and total debt into healthy or high-risk loan categories.  There were 77,535 total records with 75,036 of the records being classified as healthy loans while 2,500 records were classified as high-risk.  For the analysis, we split the data with 75% being used for training and 25% being used for testing.  In the first test, we fit the logistic regression model to the training data and used the testing data to test the model.  In the second test, we resampled the training data so there was an even split of 56,277 in both the healthy and high-risk categories and once again fit the logistic regression model to the resampled training data and used the testing data to test the model.

## Results

* Machine Learning Model 1:
  * Balanced accuracy: 0.944 which is the average of the recall of both classes and takes into account how well the model classified both healthy and high-risk loans.
  * Precision: 1.0 and 0.87. 1.0 meaning that about 100% of the loans it classified as healthy loans were healthy, 0.87 meaning that about 87% of the loans it classified as high risk loans were high risk.
  * Recall: 1.0, 0.89. 1.0 meaning about 100% of the loans that were healthy were classified as healthy, 0.89 meaning about 89% of the loans that were high-risk were classified as high-risk.

* Machine Learning Model 2:
  * Balanced accuracy: 0.996 which is the average of the recall of both classes and takes into account how well the model classified both healthy and high-risk loans.
  * Precision: 1.0, 0.87. 1.0 meaning that about 100% of the loans it classified as healthy loans were healthy, 0.87 meaning that about 87% of the loans it classified as high risk loans were high risk.
  * Recall: 1.0, 1.0. 1.0 meaning about 100% of the loans that were healthy were classified as healthy, 1.0 meaning about 100% of the loans that were high-risk were classified as high-risk.

## Summary
While both models are very accurate, the second model that used the resampled data was more accurate than the first overall and therefore appears to perform best.  An important consideration is that we are using loan data so it is more risky to get false negatives than false postives being that the bank wants to minimize the chance of the loan defaulting.  Because of this, I would recommend the second model as it has significantly less false negatives meaning less risk for the bank and an overall higher accuracy.

