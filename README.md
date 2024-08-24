# credit-risk-classification

# Module 12 Report

  

## Overview of the Analysis

* **Purpose of the analysis**
The goal of this analysis is to determine if the Logistic Regression machine learning model can more accurately predict healthy loans versus high-risk loans using the original dataset or a dataset that is resampled to increase the size of the minority class.

* **The Dataset** 
Consisting of information on 77,536 loans, the dataset used to preform the analysis includes columns for loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. **Loan status** is the category that we focused on attempting to predict with our analysis. The data provided in the remaining columns will be used as features to train the data and inform the predictions. 

* **Stages of the Machine Learning Process**
If followed in order, the stages of the machine learning process provide an accurate assessment of the model's ability to make predictions. The stages of the machine learning process are as follows:

	1. Data Preparation: Import the file, establish the DataFrame, and evaluate the columns and features.
	2. Separate the Data into Features and Labels: The labels are that you are attempting to predict are the status of the loan, healthy(0) or high-risk(1).  The features are all of the remaining data you will use to train and test the model.
	3. Use the train_test_split function to separate the features and labels into training and testing datasets. 
	4. Import the Machine Learning Model from the Library: In this instance, we imported LogisticRegression from SKLearn.
	5. Instantiate the model.
	6. Fit the model using the training data.
	7. Use the model to make predictions using the features tests data.
	8. Evaluate the Predictions: Evaluation are done by calculating and comparing metrics like accuracy score, a confusion matrix, and a classification report.

* **Machine Learning Methods Utilized**

	Primary model used in this analysis:
	* LogisticRegression model from SKLearn

	Supporting functions used in this analysis:
	* train_test_split from SKLearn
	
	Model are evaluated using the following functions:
	* confusion_matrix from SKLearn
	* classification_report from SKLearn
	

## Results

* Machine Learning Model- Logistic Regression:
	* **Accuracy Score** 99%
	* **Precision Scores**
		Class 0 (Healthy Loans): 100%
		Class 1 (High-Risk Loans):  85%
	* **Recall Scores**
		Class 0 (Healthy Loans): 99%
		Class 1 (High-Risk Loans):  91%

  

## Summary

  
The model, using the original data, performed well, predicting values of the healthy loans with precision at 100% and recall at 99%.

The model, using the original data, displayed decreased performance, predicting the values of the high risk loans with precision at 85% and recall at 91%

After reviewing the results, it can be said that the Logistic Regression model does a great job at predicting both healthy and high-risk loans, given the features that are used to train the data.

  



> Written with [StackEdit](https://stackedit.io/).
