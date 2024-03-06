# UofD Data Analysis Bootcamp Module 20 Challenge

The primary files is: <credit_risk_classification.ipynb>, located in the directory labeled <Credit_Risk>. This directory also contains a directory that contains the <lending_data.csv> file used in the code.

I used the format provided by the Starter-Code files provided.

## Overview of the Analysis

* This analysis' purpose was to take a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* The financial information used were: loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status.

* The model was designed to accuratedly predict both healthy loans and high-risk loans.

* The stages of the machine learning process for this analysis:
    1. Cleaning and preparing data, including splitting the data into training and testing sets
    2. Training the model
    3. Validating/evaluating the model
    
* Logistic Regression was used for both models. The first method used only the original dataset, while the second method resampled the dataset for balance to obtain better accuracy.

## Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    Accuracy: 100% vs 88%
    Precision: 100% vs 99%
    Recall: 85% vs 91%

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    Accuracy: 99% vs 99%
    Precision: 99% vs 99%
    Recall: 99% vs 99%

## Summary

* Which one seems to perform best? How do you know it performs best?
    The second model, using resampling, seemed to perform best. The first model (linear regression with no resampling) was slightly more accurate for healthy loans, but significantly less so for high-risk loans. The difference in sample sizes was so great that the model was unable to accurately predict the high-risk loans to the same degree. By increasing the sample size of high-risk loans to match that of healthy loans, linear regression was able to provide predictions for high-risk loans with similar accuracy to healthy loans.
    
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
    Performance was dependent on ensuring similar sample sizes for both.

If you do not recommend any of the models, please justify your reasoning.
