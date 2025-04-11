# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
*
*The purpose was to apply machine learning to loan data and figure out if a loan was high or low risk (1) or (0) respectively. Towards the goal of helping institutions decide the chance that someone will default on a loan or repay it.

* Explain what financial information the data was on, and what you needed to predict.
*
*The data included loan size, income, intrest rate, and debt to income ratio. These were made up of numbers related to information gathered about the borrowers.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
*
*loan_status was the variable we needed to predict.this was represented in a bianary values column.
(majority class - low risk) and (minority class- high risk)

* Describe the stages of the machine learning process you went through as part of this analysis.
-load and review data in pandas
-split into (x) and (y) using loan_status
-further split into testing and training  using train_test_split module
-train a classification model
-looked at model using recall,accuracy , and precision 

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
*
* a random_state= 1 was used with the LogisticRegression scikit-learn method.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.


                    precision    recall  f1-score   support

    *
    * Low Risk       1.00      0.99      1.00     18765
    *
    *High Risk       0.84      0.94      0.89       619

    *
    *accuracy                            0.99     19384
    *
    *macro avg       0.92      0.97      0.94     19384
    *
    *weighted avg    0.99      0.99      0.99     19384


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
*
*The logistic regression model had very high recal and accurracy, so would be the best choice.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
*
*to have less default the (1) is more important
*
*to have more approvals with no extra risk (0) is more important
If you do not recommend any of the models, please justify your reasoning.
*
*based on the results the model is working well. there could be improvements by testing more complicated models.