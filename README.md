README

GOAL: We aim to develop an AI model for estimating the price of used cars based on various features such
as age, mileage, brand, model, and other relevant features. This involves collecting and
preprocessing data, selecting or filtering important features, and applying ML algorithms to them
and evaluate and compare their accuracy. The overall goal is to uncover patterns and relationships
within the data that influence car prices, enabling more informed pricing strategies and decision-
making.

PROCESS: 
Scatterplots and barplots were used to visaulize the correlation between price and other factors involved in the sale of a used car. A basic linear regression model was initially trained and tested. 
The model was then compared to RIDGE, LASSO, and Decision tree. 
The linear regression model gets us to a RMSE of $6545 for the price prediction, with an R2 score of 0.73
The basic model can predict the price of used cars with an error which would typically be in the range of a few thousand dollars.
While this can be a good starting point, it would definitely not be ideal for a car dealership using our model for their pricing strategy and marketing decisions.
We would like to improve the basic linear regression. In the next step, we try a few different regression models to see if we can improve over the initial result.italicized text

FINDINGS: 
While columns like odometer reading, condition, manufacturer, and drive are highly relevant for the price of used cars, other columns such as VIN, id, and region do not typically affect the price as much. 
It is important to filter out these columns as part of the data clean up and pre-processing stage
The price of a used car has high correlation with the year, odometer reading, condition, transmission and cylinders. 
The correlations are weaker for the other features in the processed dataset.
We see that the Lasso and Ridge regression models do not improve over Linear regression. 
However, using a Decision Tree (DT) based regression model leads to a significant improvement. 
The R2 score jumps to 0.86 and the test RMSE goes down to $4682. 
The use of polynomial features with order of 3 leads to a slight improvement in the RMSE and R2 score of the Decision Tree regression model.
