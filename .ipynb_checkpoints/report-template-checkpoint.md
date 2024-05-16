# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithm).

### Analysis
The purpose of this analysis was to develop machine learning models to assess credit risk based on financial data. Specifically, we aimed to predict whether a loan is healthy or has a high risk of defaulting based on the available financial information.

The dataset contained various financial attributes, such as loan amount, interest rate, credit score, debt-to-income ratio, and employment length, among others. The target variable, loan_status, had two categories: 0 representing healthy loans and 1 representing high-risk loans.

As part of the analysis, we followed several stages of the machine learning process:

- Data Preprocessing: We started by loading the dataset and separating it into features (X) and labels (y). We then split the data into training and testing sets using the train_test_split function.

- Model Training: We trained logistic regression models using the training data. Logistic regression was chosen due to its simplicity and effectiveness in binary classification tasks.

- Model Evaluation: After training the models, we evaluated their performance using various metrics, including accuracy, precision, and recall.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.


### Results:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00     15001
           1       0.86      0.91      0.88       507

    accuracy                           0.99     15508
   macro avg       0.93      0.95      0.94     15508
weighted avg       0.99      0.99      0.99     15508


Machine Learning Model 1:
Accuracy: 99%
Precision (class 0): 100%
Precision (class 1): 86%
Recall (class 0): 100%
Recall (class 1): 91%



## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

### Summary:

Based on the results, Machine Learning Model 1 performed exceptionally well in predicting healthy loans (class 0), achieving 100% accuracy, precision, and recall. However, for high-risk loans (class 1), while the precision is relatively high (86%), the recall is slightly lower (91%). This indicates that the model correctly identifies most high-risk loans but may miss some.

The performance of the model depends on the problem we are trying to solve. For instance, if our primary concern is identifying high-risk loans accurately to minimize financial losses, we might prioritize improving the recall for class 1. On the other hand, if we aim to minimize false alarms and prioritize precision, we might focus on improving precision for class 1.

Overall, considering the high accuracy and balanced precision-recall trade-off, Machine Learning Model 1 appears to be the most suitable for predicting credit risk in this scenario. However, further optimization could be done to enhance the model's performance, especially in identifying high-risk loans.

