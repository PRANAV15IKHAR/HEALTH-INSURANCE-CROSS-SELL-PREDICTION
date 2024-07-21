# Capstone-project-6
# Health-insurance-cross-sell-prediction

This is a note book of  cross selling of health insurance customers on vehicle insurance product and using machine learning to predict whether a customer is interested or not in vehicle insurancen

## Background Information :
an Insurance company that provide Health Insurance to its customers, usually they offer other insurance product to the customers through diffirent kind of marketing channel. In this case we will build a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.
## Problem Statement:
Un optimize customer reachout process, many insurance worker spend a lot of their time having meeting with prospective client without knowing the probablity of that customer to buy the insurance product
## Business Goals:
Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue
## Business Question:
How does age of a vehicle determing the response of vehicle insurance advertisment
How to attract customers from different generation
what's the major factor that make a health insurance customer not intersted with vehicle insurance
What's the best machine Learning modeling for this Cross Sell case


## Feature Engineering & Selection For Machine Learning Process

Encoding all the categorical features
Checking correlation between dependent and independent variable
Feature Selection
## Model Building :

Splitting data into Training and Testing
Apllying the SMOTE (Synthetic Minority Oversampling Technique) to the minority target since the data is imbalance
Creating base model of classification algorithm ( Logistic Regression, Random Forest Clasifier)
Check The Evaluation matrix for all the base model
HyperParameter tuning
Checking Evaluation Matrix for tuned Model
Choose which model has the best recall score for this case

## Conclusion:
Through Exploratory Data Analysis, I observed that customers belonging to young Age are more interested in vehicle response. While young people below 30 are not interested in vehicle insurance. I also noticed that customers with vehicles older than 2 years are more likely to be interested in vehicle insurance. Similarly, customers with damaged vehicles are more likely to be interested in vehicle insurance.
Variables such as Age, Previously_insured, and Annual_premium seem to have a significant impact on the target variable.
I found that the target variable was highly imbalanced, which I addressed by using the Random Over Sample resampling technique. Additionally, I applied feature scaling techniques to normalize our data, bringing all features to the same scale, which makes it easier for ML algorithms to process.
I then applied Machine Learning Algorithms to predict whether a customer would be interested in Vehicle Insurance. For logistic regression, I achieved an accuracy of 78%, and for the XGBoost Classifier, I obtained an accuracy of 79%. However, I achieved the highest accuracy of about 91% and an ROC_AUC score of 92% with the random forest model. Therefore, I conclude that random forest is the best model compared to the others.

