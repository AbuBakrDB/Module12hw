# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to develop machine learning models to predict loan statuses based on financial information. The dataset contained various financial features, such as loan amount, interest rate, and employment length, along with the loan status indicating whether a loan is healthy or high-risk.

The stages of the machine learning process included data preprocessing, model selection, training, and evaluation. Initially, I explored the dataset to understand its structure and distribution. Then, I preprocessed the data by handling missing values, encoding categorical variables, and splitting the data into training and testing sets. 

For modeling, I experimented with logistic regression models, both with and without resampling techniques. The resampling methods used included oversampling of the minority class (high-risk loans) to address class imbalance.

## Results

### Machine Learning Model 1 (Logistic Regression with Oversampling):

- Balanced Accuracy: 0.96
- Precision (Label 0): 100%
- Recall (Label 0): 99%
- Precision (Label 1): 84%
- Recall (Label 1): 94%

### Machine Learning Model 2 (Logistic Regression without Oversampling):

- Balanced Accuracy: 0.96
- Precision (Label 0): 100%
- Recall (Label 0): 99%
- Precision (Label 1): 84%
- Recall (Label 1): 99%

## Summary

Both machine learning models achieved high accuracy, precision, and recall scores. However, there are differences in their performance metrics:

- Model 1 (with oversampling) has slightly lower recall for high-risk loans (Label 1) compared to Model 2 (without oversampling).
- Model 2 has a higher recall for high-risk loans (Label 1), indicating it is better at correctly identifying high-risk loans.

The choice between the two models depends on the specific priorities of the lending company. If correctly identifying high-risk loans is crucial, Model 2 might be preferred due to its higher recall for Label 1. However, if overall performance balance is more important, Model 1 could be considered, as it achieves a good balance between precision and recall for both labels.

Ultimately, the selection of the model should be based on the specific goals and requirements of the lending company, considering factors such as the cost of misclassifications and the desired balance between precision and recall.
