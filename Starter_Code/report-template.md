# Module 12 Report Template

## Overview of the Analysis

* This project is using a dataset of historical lending activity from a lending service company to build a model that can identify the creditworthiness of borrowers.  The financial information we use for this exercise including loan size, interest rate of the loan, borrower income, debt to income ratio, number of accounts, derogatory marks, total debt and loan status.  With all the information from lending dataframe, we cluster them by loan status and use `value_counts` to see the result.  The model includes three stages of the machine learning process: 1, Instantiate the model  2, Fit the model 3, Use the model.  We run it twice with 1st model in standard logisticRegression and 2nd model in resampling method where we use the RandomOverSampler from the imbalanced-learn library to adjust the data to an equal number of data points.

## Results

* Machine Learning Model 1:
  * Standard logistic Regression Model - the prediction results for high risk loans is "good" with 
      accuracy score at 95.20
      Precision 85%
      Recall 91%
      Specificity 99%
      Harmonic Mean 88%
      Geometric Mean 95%

* Machine Learning Model 2:
  * Resampled logistic Regression Model - the prediction results for high risk loans is "very good" with
      accuracy score at 99.37
      Precision 84%
      Recall 99%
      Specificity 99%
      Harmonic Mean 91%
      Geometric Mean 99%

## Summary

* Model 2 provides better predictions because it is only 1% lower on precision versus Model 1.  But it has 8% higher recall value, 3% higher Harmonic mean and 4% higer Geometric mean for search for high risk loans.  
* In this exercise, it is far more important to be able to identify high risk loans.  
* Since resampled data is much more accurate predicting for loans, we recommend using resampled logistic Regression model.