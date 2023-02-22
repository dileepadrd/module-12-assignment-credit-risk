# Module 12 Report Template

## Overview of the Analysis

Credit risk classifications, more often than not, intrinsically unbalanced. The reason for this is that the majority of the loans are healthy loans. The purpose of this analysis is to create a model to identify the creditworthiness of borrowers based on the dataset of historical lending activity from the peer-to-peer lending service company provided. 

Furthermore, the loan status is the variable that is going to be predicted through this model. In order to achieve this,  historical data of loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks and total_debt are being used. 

During the first stage the data is loaded into Panda Dataframe and separated into X and Y data sets. After that the original data is divided into two main categories: testing data set and training data set. The purpose of the training data set is to train the model while the testing data set is used to check the accuracy of the model. 

The next stage is to initialize and fit the LogisticRegression model for the original dataset. After that the predictions of the original dataset are being made by using the predict function of the LogisticRegression model. During the next phase, the accuracy score, confusion matrix and the classification report for the unbalanced dataset are being generated. The next step is to generate a sample via RandomOverSampler and do the same steps for the sample data. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
