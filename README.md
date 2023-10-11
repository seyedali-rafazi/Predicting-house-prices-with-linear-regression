# Predicting House Prices with Linear Regression and Random Forest
This repository builds a linear regression model and random forest model to predict house prices in California based on housing features like median income, median house age, rooms per household etc.

## Data
The data used is the California Housing Prices dataset from Kaggle. It contains the following features:

longitude
latitude
housing_median_age
total_rooms
total_bedrooms
population
households
median_income
median_house_value
Data Cleaning
The data is cleaned before modeling:

## Missing values are imputed
Categorical variables converted to dummies
Outliers removed from target column 'median_house_value'
Exploratory Data Analysis
Some insights from EDA:

## Median house value is higher in coastal regions
House price increases with median income
Higher median rooms per household correlates with higher prices
House value distribution is right-skewed
Models
### Linear Regression
A linear regression model is built using 'median_income' as the main predictor. Additional predictors like 'rooms_per_household', 'bedrooms_per_room' etc. are added.

The model is evaluated using MAE between predicted and actual prices.

### Random Forest
A random forest model is tuned using grid search on hyperparameters like number of trees, max depth etc.
The random forest model outperforms the linear regression model.

