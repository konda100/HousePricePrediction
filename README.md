# SurpriseHousing
Suroise Housing Data Analysis

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free.

## Problem Statement
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:
- Which variables are significant in predicting the price of a house, and
- How well those variables describe the price of a house.

## Business Goal:
Model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.


## Steps followed:
* Load data
* Data inspection
* Handle Missing values
* Add or transform features
* Train/Test split
* Scaling
* Base line Modelling
* Tuning with regularisation (Ridge/Lasso)
* Model Evaluation:

## Result
#### Values for Lasso and Ridge
- Base RFE: Rain: 93.2 Test: 63.5
- Ridge:
    - With RFE:    Train: 93.1 Test: 66.7
    - Without RFE: Train: 90.3 Test: 80.6
- Lasso: Train: 91.8 Test: 77.3

#### Final Alpha values:
- Ridge: 10
- Lasso: 100

#### Top 5 most significant variables in Ridge with RFE are:
- OverallQual_Average
- OverallQual_Below Average
- OverallQual_Excellent
- OverallQual_Fair
- OverallQual_Good

#### Top 5 most significant variables in Ridge without RFE are:
- GarageType_Detchd
- GarageType_No Garage
- GarageFinish_No Garage
- GarageFinish_RFn
- GarageFinish_Unf

#### Top 5 most significant variables in Lasso are:
- GarageType_Detchd
- GarageType_No Garage
- GarageFinish_No Garage
- GarageFinish_RFn
- GarageFinish_Unf

### Contributed by:
* Konda Reddy Golamaru