## Attrition-Prediction

 

![image](https://user-images.githubusercontent.com/116499989/197399058-deba9587-2760-4fc8-9590-28a793c7e668.png)


# Overview

Employee attrition is when an employee leaves the company through any method, including voluntary resignations, layoffs, failure to return from a leave of absence, or even illness or death. Whenever an employee stops working for the company due to any reason and is not replaced immediately, it is called employee attrition.

# Business Problem

Latest survey by global professional services firm Aon Plc has revealed that the first half of 2022 saw an attrition rate of 20.3% in India, a significant increase after the two year Covid pandemic induced lockdown. The recruitment agency Michael Page predicted that India is likely to witness an 86% employee attrition for 2022. Reports have suggested that the Great Resignation occurred owing to career progression, change career role or industry, unhappy with salary, unhappy with strategy or direction of company.
Being able to determine factors that lead to attrition, and correspondingly being able to predict which employee will leave the company can help companies formulate strategies that can help them retain talent.


# Data

The data contains attributes such as Age, Attrition, Business Travel, Department, Education Field, Gender, Environment Satisfaction, Over Time, Martial Status, Monthly Income, Years of Work experience, Years at company, Job Satisfaction etc.
The dataset suffers from class imbalance where, where approximately 16% of the target variable observations have been classified as ‘1’ and approximately 84% are classified as ‘0’.
There are no missing values in our dataset.

# Workflow

•	EDA

  1.	Univariate analysis 
  2.	Bivariate analysis
  3.	Multivariate analysis
  
•	Feature Engineering

  1.	Label encoding
  2.	One hot encoding on nominal variables
  3.	Train-Validation-Test split
  4.	Handling Imbalance data using SMOTE(done only on training data)
  5.	Standardization of train, validation and test data.
  
•	Model fitting on training data

•	Model evaluation on validation data

•	Model testing on test data


# Results

I fitted 3 classification models – Logistic Regression, KNN and Decision Tree Classifier- on the training dataset and evaluated the performance of all models on validation dataset.
Since this is an attrition problem I used recall or sensitivity as the evaluation metric because we are interested in knowing how our model is predicting the employees who are leaving.
Decsion Tree Classifier gave the best recall (55%) on validation dataset and reported to be the best model to predict whether an employee will leave or not.
