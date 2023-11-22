# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to see how well a logistic regression model could be used to classify the risk level of loans. After creating the initial LR model, I then measured the impact of resampling the data on the LR model's performance.

To make the model, we used the following input data: loan size, interest rate, borrower's income, debt-to-income ratio, how many (credit) accounts the borrower has, previous derogatory marks, total debt, and loan status (risky vs healthy).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1 (Logistic Regression with original data):
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  - Precision: Out of the loans that the model predicted were high-risk, 85% of them actually were.
  - Recall: Out of the loans that were actually high-risk, the model correctly predicted the classification 91% of the time.
  - F1 Score: F1 scores closer to 1 indicate better performance, so an 88% F1 score means that the model does a solid, but not perfect/fantastic job of predicting loan risk level.

* Machine Learning Model 2 (Logistic Regression w/ resampled data):
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  - Precision: Out of the loans that the model predicted were high-risk, 84% of them actually were.
  - Recall: Out of the loans that were actually high-risk, the model correctly predicted the classification 99% of the time.
  - F1 Score: F1 scores closer to 1 indicate better performance, so a 91% F1 score means that the model does a great job of predicting loan risk level.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

Overall, I found that the second LR model using the resampled data had better performance. My recomendation would be to use LR model 2 when trying to predict the risk level of loans, as it correctly predicted the high-risk classification 99% of the time. 

Future improvements to this model might be made by adding more granularity to the risk-levels of loans. For example, instead of only 2 categories healthy vs high-risk, I might create levels of risk based on percentiles, ie with the bottom 10% of loans being the riskiest.