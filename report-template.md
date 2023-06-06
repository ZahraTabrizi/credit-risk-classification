# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

- The purpose of this analysis was to create a model that would identify how high-risk or healthy a borrower is for the creditor.
- The given dataset showed the past lending activity from a peer-to-peer lending service company.
- The dependant variable was the loan status which is whether a loan is healthy or high risk.
- The independent Variables were loan size, interest rate, lender income, debt to income ratio, and finally number of accounts and derogatory marks.
- First, the data was split into traning and test sets. 
- Second, the dependent and independent variables were defined. 
Third, a logistic regression model was created and the original data was fit into this model. The trained model was used to make predictions. 
- Finally, the model's performance was evaluated.
- Two diffeent Logistic Regression models were created by using the original data set and the over resampled data set. The results were compared at the end.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
 precision    recall  f1-score   support

           0       1.00      0.99      1.00     18750
           1       0.84      0.95      0.89       634

    accuracy                           0.99     19384
   macro avg       0.92      0.97      0.94     19384
weighted avg       0.99      0.99      0.99     19384



* Machine Learning Model 2:
  precision    recall  f1-score   support

           0       1.00      0.99      1.00     18750
           1       0.84      0.99      0.91       634

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The analysis showed that the collected data can be used to train and test the Machine Learning Classification Model. To have better preditions, the issue of imbalance between healthy and high risk should be resolved.
It seems that randomly oversampling gives higher balanced accuracy and higher recall scores. This means that this model performs better in predicting high risk loans. There are problems that can come up with predictions; false negatives and false positives. Both of these situations have a cost for the company, meaning it is important to predict the 0s and the 1s. This can lead to greater accuracy.