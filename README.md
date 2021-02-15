# Bankruptcy-Prediction 
<br>
## Introduction
This is my first ML project.
I downloaded the <a href="https://www.kaggle.com/fedesoriano/company-bankruptcy-prediction"> Company bankruptcy prediction </a> dataset from kaggle
The project is aimed at predicting whether a company will go bankrupt

## About the dataset
The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. 
Company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange.

## Technolgies used
I have used scikit-learn, XGBRegressor, CatboostClassifier for making predictions and matplotlib and seaborn for data visualisation

## About the project
After initial analysis of the data,I figured that the data was imbalanced with only 220 labels of companies going bankrupt as compared to 6600 of companies not going bankrupt.
I divided the data in train,validation and test sets.

### To solve the problem of imbalance I used undersampling and SMOTE for oversampling 
For each of the two techniques I used to XGBRegressor and Catboost Classifier for making predictions.

##### Undersampled data
For the undersampled data the catboost classifier worked better with a f1-score of 0.90 over XGBRegressors score of 0.78

##### SMOTE as Oversampling technique
After Oversampling, the overall results were better but the catboost classifier and XGBregressor had similar f1-scores of 0.99 and 0.98 respectively

## Conclusion
Finally, We run the best model i.e. the catboost classifier on the oversampled data on the test set and acquired an f1-score accuracy of 0.99
