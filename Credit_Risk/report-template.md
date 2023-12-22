# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of the analysis is to create a ML model that can determin whether a loan is considered low-risk and healthy or high-risk based off of historical lending data. The goal is to use Logistic Regression to determine if it can be accurate to determin the loan status using original data and resampled data. 

* Explain what financial information the data was on, and what you needed to predict.
The data contained information about the loan including the size, interest rate, and information about the borrower like their income, debt to income and total debt. We needed our model to predict the loan status that the historical data provided.  

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
We used value_counts to see how many loans were healthy (0) vs. risky (1) in the data set. 
Original Data
0    75036
1     2500

Oversampled Data
0    56271
1    56271

* Describe the stages of the machine learning process you went through as part of this analysis.
1. Prepare data for analysis
2. Separate the data into labels (y) and features (x)
3. Check the balance of the labels
4. Split the data into training and testing datasets using train_test_split
5. Choose the machine learning model for classification - Logistic Regression
6. Fit the model using training data 
7. Make prediction using the testing data 
8. Evaluate the model's performance using accuracy score, confusion matrix, and classification report

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
SKLearn Logistic Regression
train_test_split
confusion_matrix
classification_report


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * Accuracy: 0.95
  * Class 0: Precision - 1.00, Recall - 0.99
  * Class 1: Precision - 0.85, Recall - 0.91


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Accuracy: 0.99
  * Class 0: Precision - 1.00, Recall - 0.99
  * Class 1: Precision - 0.84, Recall - 0.99
  
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* The oversampled model performed better than the original model. The oversampled model identified the healthy loans almost identical to the first model. When it came to the risky loans, the oversampled model had equivalent precision but a lot higher recall at 99% compared to 91% in the original model and saw an increase in 3% in f1 score. The accuracy of the resampled also increased from 95% to 99%. 

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
With class 1 the precision is 0.84 and recall is 0.91 in the original data. We should still be mindful of false positives and negatives and look at more data before fully deciding to utilize the model. 


If you do not recommend any of the models, please justify your reasoning.
