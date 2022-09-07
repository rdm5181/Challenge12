# Module 12 Report

## Overview of the Analysis

The analysis used was logistic regression models.  Logistic regression uses functions such as a sigmoid function to assess the probability that a data point will fall between two values (a binary classification).  For us, this was identifying the loan status of an individual and placing them into either a healthy loan or a high-risk loan.  

The dataset had many features to base the assessment on: loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt.  The data was further split into a "test" set and a "train" set.  Training was done to build the model to make predictions on the probability certain borrowers would fall into healthy or high-risk.  The test set was then used to see the accuracy of the model and allow for other observations of its performance.

Due to the imbalance of known healthy loans to high-risk, oversampling was performed, which made new data similar to the old so that the number of high-risk loans were similar to the number of healthy loans.  This is definitely important as common metrics may be skewed if the data itself is skewed.


## Results


* Machine Learning Model 1:
  * Balanced Accuracy was 95%.  
  * The precision for healthy loans was 100% and the recall for these loans was 99%.  
  * The precision for high-risk loans was 85% and the recall for these loans was 91%.
  * Metrics may not be accurate as only 3% of all the loans were high-risk.



* Machine Learning Model 2:
  * Healthy to high-risk loans is 1:1
  * Balanced Accuracy is 99.3%
  * The precision for healthy loans was 100% and the recall for these loans was 99%.
  * The precision for high-risk loans was 84% and the recall for these loans was 99%.

## Summary

The second model was more accurate and had a better representation of the data.  While the first model supposedly had a better precision with high-risk loans, it is clear that the second model picked them better and had an improved recall score on them.

Because of the nature of the business, it is clear that spotting high-risk loans is important because if someone defaults, that risk and loss is imparted to the business.  Therefore, the second model should be followed as this one did a much better job of finding the high-risk loans without making its other predictive performance suffer (i.e. it still did a good job finding healthy loans).  

