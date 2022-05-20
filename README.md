# Swen Fereira / NYC-Taxi-Trip-Time-Prediction---Capstone-Project

In this Capstone project , the main aim is to build a model that predicts the total ride duration of taxi trips in New York City. 

The primary dataset is one released by the NYC Taxi and Limousine Commission, which includes pickup time, geo-coordinates, number of passengers, and several other variables.

The dataset consists of 1458644 rows and 11 columns, containing features such as trip longitude and latitude values, day, month, year of the trip, etc.

The project is executed in 6 main steps:
1.	Data Overview 
2.	Feature Creation 
3.	Exploratory Data Analysis 
4.	Feature Engineering 
5.	Model Creation & Tuning 
6.	Model Evaluation
Features such as speed and distance are engineered, to create useful variables. 
Also we created four parts of time, ie  Morning , Afternoon , Evening , Late Night.

Exploratory data analysis (EDA) was performed, both univariate and bivariate analysis were done to gain better understanding about the data. Some understanding from the data was received such as, single passenger trips are the highest, evenings are the busiest, Mostly trips are done at a speed range of 10-20 km/h, We see the busiest hours are 6:00 pm to 7:00 pm which makes sense as this is the time for people to return home from work, We see Fridays are the busiest days followed by Saturdays. 
Models experimented with:
1.	Linear Regression
2.	Lasso Regression
3.	Ridge Regression
4.	Decision Tree
5.	XGBoost
Conclusion: 
For Linear regression model, MSE and RMSE for training and testing are similar but has very poor R2 for training and testing data.
Lasso regression and Ridge regression R2 increases , but not with significant amount.
We can see that MSE and RMSE of Decision Tree model are not varying much during training and testing time. Also the R2 is almost same for training and testing time.
MSE and RMSE of XGBoost model are very similar and their R2 is 80. 
From above table, we can conclude XGBoost is best model for our dataset.
