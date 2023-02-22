# Module 12 Report Template

## Overview of the Analysis

Credit risk classifications, more often than not, intrinsically unbalanced. The reason for this is that the majority of the loans are healthy loans. The purpose of this analysis is to create a model to identify the creditworthiness of borrowers based on the dataset of historical lending activity from the peer-to-peer lending service company provided.

Furthermore, the loan status is the variable that is going to be predicted through this model. In order to achieve this, historical data of loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks and total_debt are being used.

During the first stage the data is loaded into Panda Dataframe and separated into X and Y data sets. After that the original data is divided into two main categories: testing data set and training data set. The purpose of the training data set is to train the model while the testing data set is used to check the accuracy of the model.

The next stage is to initialize and fit the LogisticRegression model for the original dataset. After that the predictions of the original dataset are being made by using the predict function of the LogisticRegression model. During the next phase, the accuracy score, confusion matrix and the classification report for the unbalanced dataset are being generated. The next step is to generate a sample via RandomOverSampler and do the same steps for the sample data.

## Results

In this section, the balanced accuracy scores and the precision and recall scores of the machine learning models used are being described.

> Please note that rounded approximate values have been used in the following section.

- Machine Learning Model 1: With original data

  - Accuracy 95% - all healthy loans and high risk loans have been predicted with 95 percent accuracy.
  - Precision of healthy loans 100% - almost all healthy loans predictions are correct
  - Precision of risky loans is 85% - 85 percent of risky loan predictions are correct
  - Recall of healthy loans is 99% - indicates that 99 percent of the actual healthy loans have been identified
  - Recall of risky loans is 91% - means 91 percent of actual risky loans have been predicted correctly

- Machine Learning Model 2: With sample

  - Accuracy 99% - all healthy loans and risky loans have been predicted with 99 percent accuracy
  - Precision of healthy loans 100% - almost all healthy loan predictions are correct
  - Precision of risky loans is 84% - means 84 percent of risky loan predictions are correct
  - Recall of healthy loans is 99% - indicates 99 percent of actual healthy loans have been predicted correctly
  - Recall of risky loans is 99% - mean 99 percent of actual risky loans have been predicted successfully

## Summary

Both prediction models have worked with acceptable accuracy. However, according to the accuracy, precision and recall scores, the resampled data model works better then the other for the data set provided. The only one exception is the precision of the high risk loans of two models: 85 percent for the original dataset and 84 percent for the resampled data set. Nevertheless, since there is no significant difference between 85 and 84 and all other parameters are better in the BalancedResampled data, it could be concluded that the resample data set would be better for the dataset.

The model that is working best highly depends on the dataset. However, in real-life datasets, the majority of datasets are unbalanced. Therefore, unbalanced resample models could be working for many datasets.

In the context of loan credit risk analysis, identifying risky loans is more important than identifying the healthy loans. When identifying risk loans, the most important question to be answered is how many actual risky loans have been identified correctly. In order to answer this question, the recall score of risk loans is the best indicator. Since, recall score is better in the model with BalancedResampled data set, resampled model could be considered to be the best model for this dataset.
