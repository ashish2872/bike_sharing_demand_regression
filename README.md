# Bike sharing (Demand Regression)
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


## General Information
On the given dataset of the Bike Sharing, I have conducted the Exploratory Data Analysis and Linear Regression to determine and predict the demand of shared bikes.

## Technologies Used
- Numpy
- Pandas
- Matplolib
- Seaborn
- ScikitLearn
- Statsmodel

## Conclusions 
1. Understanding the data - My first step was to understand what kind of data has been provided. 

2. Data Preparation and EDA  - Next I converted the categorical variables into their respective categories and performing the EDA on the numerial and categorical variables.

3. Dummy Variables creation - Next I created the dummy variables for the categorical variables, so the model efficiency increases.

4. Train-Test Split and Rescaling - In this particular step I split the dataset into 70:30 ratio and rescale the train dataset for all variables to be in the same interval.  

5. Training the model - In this particular step, I used the RFE method to get the top 25 features and then run the model to check the stats of the features, when I did this I found many insignificant variables and repeated the process till I got the top 10 features then I ran the model again and check the p-values to determine the significant variables. Then I calculated the VIF to check for the multicollinearity. After I got the top 10 features, I still had to remove the humidity column as the VIF was more than the acceptable level

6. Prediction of the Model - After training the model, I performed the predictions on the test dataset.

7. Model Evaluation - After completing the prediction of the testing dataset, I did the model evaluation and performed Residual analysis, durbin-watson test and the test for homoscedasticity. I found that verified all the assumptions with an R-squared value of 0.825 (82.5%) 
