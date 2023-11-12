# Module 12 Report Template

## Overview of the Analysis

In this task, our objective was to develop a machine learning model for predicting the overall risk of loans using a dataset of 77,536 loans with eight features, including loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and loan_status. We followed these steps:

Segregated the data into labels and features, with loan_status as the label and the remaining columns as features.
Split the data into training and testing sets.
Utilized a logistic regression model to classify loans into 'healthy' or 'high-risk.'
Fitted the model with the training data.
Made predictions using the test data.
Evaluated the model by comparing predictions with test labels.
Conducted an additional logistic regression prediction using resampled data and generated a confusion matrix and classification report.


## Results

Machine Learning Model 1:

Accuracy: 95.20%
Precision:
Healthy: 100%
High-Risk: 85%
Recall:
Healthy: 99%
High-Risk: 91%

Machine Learning Model 2 (Resampled Data):

Accuracy: 99.45%
Precision:
Healthy: 99%
High-Risk: 99%
Recall:
Healthy: 99%
High-Risk: 99%


## Summary

According to the classification report, Model 1 achieved 95% overall accuracy but demonstrated room for improvement in precision, especially for high-risk loans. Model 2, trained on resampled data, exhibited remarkable across-the-board accuracy of 99%, showcasing its superior performance in distinguishing between 'healthy' and 'high-risk' loans.

In conclusion, resampling proved advantageous, enabling the model to achieve optimal performance by repeatedly drawing small samples from the same population. This approach saves time and resources by recycling the dataset without the need for new data.