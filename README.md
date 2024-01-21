# credit-risk-classification
Creating machine learning models to classify the risk level of given loans.

## Background

Lending services companies allow individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market.

You will be using this data to create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier.

## Instructions

#### Retrieved the Data

* From `lending_data.csv`

Imported the data using Pandas. Displayed the resulting dataframe to confirm the import was successful.

#### Predicting Model Performance

Created and compared two models on this data: a Logistic Regression, and a Random Forests Classifier. Before creating, I made a prediction as to which model I thought would perform better.

#### Split the Data into Training and Testing Sets

Created the features DataFrame, `X`, by removing the `loan_status` column. Created `y`, the labels set, by using the `loan_status` column. Split the data into training and tested datasets by using the `train_test_split` function.

#### Created, Fitted and Compared Models

Created a Logistic Regression model, fitted it to the training data that I created in the previous step. Then, determined the model's score by using the `score` function and the tested the data from the previous step. Did the same for a Random Forest Classifier.

Reviewed the scores of each model. Noted which model performed better, and how it compared to my prediction.
