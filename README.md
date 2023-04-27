# credit-risk-classification20
Supervised Learning with Logistic Regression

## Overview of the Analysis

The purpose of this project analysis is to use data preprocessing, model selection, and evaluation to identify creditworthiness of borrowers.The dataset I used in this project contains information about loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt,and loan_status. The dataset is split into a training set and a testing set and could be used to predict whether a loan would be paid back or not. It could help lenders make better decisions about when/who to give a loan to.

The data was from a 'dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.'
 
I used a logistic regression model as the baseline model and evaluated it using accuracy, precision, recall, and F1-score. From these, I need to predict whether a loan application should be approved.
 
I separated the data into train and test sets to train the model to predict the value of the target variable (in this case, "loan_status") based on the values. This also allows to look easily at the data, which can help us to better understand the data and identify potential patterns or trends.
 
I used the logistic regression model to transform the data into a probability value between 0 and 1. This probability represents the likelihood that the data was a 0 or 1- good or default. 

Logistic regression is used technique in fields like medicine, economics, and social sciences, for tasks such as predicting the likelihood of a patient having a certain disease, classifying email messages as spam or not spam, or predicting the outcome of a political election.

## Results
A confusion matrix was completed on both the original analysis and the resampled analysis. The four type categories were analyzed. 
* True Positives (TP) represents the number of positive samples that were correctly identified as positive.
* False Positives (FP) represents the number of negative samples that were incorrectly classified as positive. 
* False Negatives (FN) represents the number of positive samples that were incorrectly classified as negative. 
True Negatives (TN) represents the number of negative samples that were correctly identified as negative. 

<b><u>Original data 75/25 split</u></b>

|        |  Precision    |  Recall      |  F1-Score     |
| ------ | ------------- | ------------ | ------------- |
| 0      | 0.997008      | 0.994564     | 0.995785      |
| 1      | 0.846617      | 0.909532     | 0.876947      |

* accuracy    | 0.991849


<b><u>Oversampled data from the smaller dataset of faulty loans</u></b>

|        |  Precision    |  Recall      |  F1-Score     |
| ------ | ------------- | ------------ | ------------- |
| 0      | 0.994916      | 0.994564     | 0.995785      |
| 1      | 0.994546      | 0.994917     | 0.994732      |

* accuracy    | 0.9947314731  112542.000000

## Summary 

Resampling Methods: This involves either oversampling the minority class or undersampling the majority class to create a more balanced dataset. 

In the original sampling, I recieved an accuracy of 99.1%, however, the precision of the loans that were classified as 0 was only 85%. This meant that 15% of loans that defaulted were not classified or predicted that way, resulting in a loss for the bank.

After resampling, the precision of true positives that were predicted as positive for class 0 was 0.994916, which means that out of all the samples predicted as 0, 99.49% were actually 0. For class 1, the precision was 0.994546, which means that out of all the samples predicted as 1, 99.45% were actually 1. This also applies to the F-1 and Recall.  This means that the model was preforming well and correctly idenitifying the good and faulty loans predictions.


