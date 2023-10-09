# Loan-Prediction
This is an ML project to assist a bank that has received loan applications than it typically receives to predict applicants who are eligible for the loan and those that are not.

## Problem Statement 
SYL bank is one of Australia�s largest banks. Currently, the loan applications which come in to their various branches are processed manually. The decision whether to grant a loan or not is subjective and due to a lot of applications coming in, it is getting harder for them to decide the loan grant status. Thus, they want to build an automated machine learning solution which will look at different factors and decide whether to grant loan or not to the respective individual.

## Goal 
The goal of this project is to build a classification model to predict if an applicant is elibile for a loan or not. The project also aims to look into various factors that influences the applicants elibility for the loan, per the model. 

## Solutions steps 
### Table of Content
1) Data Importation
   - Imported the raw data files (111107 rows, 19 columns)
    
2) Exploratory data analysis, data cleaning, and Feature engineering
   - The data was validated and cleaned, data types, and missing values were fixed appropriatly.
   - Each variable was explored to understand its distribution
   - Bivariate analysis was done to assess the relationships between varibales

3) Data preprocessing for modelling
   - Categorical variables were converted to numerical varibales through One-Hot Encoding
   - Data was separated into predictors(input varibales), and target vaiable
   - Data was split into Train/Test set
   - 
4) Building different Classification models
   - Different models were built using different algorithms, in order to get the best model
   - The models built include the following:
      * Decision Tree Classifier
      * Logistic Regression
      * XGboost
      * Random Forest Classifier
      * Gradient Boosting
      * Ada Boosting
      * Votting Classifier - combined Logistic regression, Support Vector Classifier, Decision Tree Classifier to form the stronger model
        
5) Model Evaluation
  - Different metrics are considered for evaluating and comparing the models.Since the classes in the target variable (Loans status) is not balanced, 
    accuracy is definetly not a good metric to rely on in this case hence will be used to only check for overfitting and underfitting. Confusion
    matrix,F1 score,and Receiver Operation Curve will employed in evaluating and comparing the models.
    
6) Model Selection
   - Considering the ROC curve,confusion matrix and F1 score - the Gradient boost appears to be the best model. Since management is concerned about
     feature imortantce, the importance features were extracted by the model.
  -  ROC curve, confusion Matrix, and F1 Score were used to evaluate he model performance because the target varibale was imbalanced and accurancy was not
    best metric to use.
   
7) Feature importance
   - The first six important features include:
     * Credit Score
     * Annual Income
     * Term(Short term in particular)
     * Maximum Open Creit
     * Current Loan Amount
     * Current Credit Balance 
    
8) Summary
   - The following features also have an influenctial impact on whether or not a customer was able to attain a loan: 
     * Term (short term in particular)/ 
     * Maximum Open Credit/
     * Current Loan Amount/
     * Current Credit Balance 




