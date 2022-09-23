# Bike_sharing_demand_prediction_Capstone-_project_Regression

# Conclusion :

# Data Exploration Conclusions :

In this project, we explored several types of informations that influence bike rental count. Below is a quick summary of exploratory data analysis

# Working Day:

for a Working Day where the rental count high at peak hours (Most demand for bike is in between 7 to 9 AM and 5 to 8 PM .)

# *Non-working day *:

where rental count is more or less uniform across the day with a peak at around noon.

# Hour of the day:

Bike rental count is mostly correlated with the time of the day. As indicated above, the count reaches a high point during peak hours on a working day and is mostly uniform during the day on a non-working day

# Season:

We see highest number bike rentals in Fall (July to September) and Summer (April to June) Seasons and the lowest in Spring (January to March) season

# Weather:

As one would expect, we see highest number of bike rentals on a clear day and the lowest on a snowy or rainy day

# Humidity:

With increasing humidity, we see decrease in the number of bike rental count.

# Model performance observations :

During the time of our analysis, we initially did EDA on all the features of our datset. We first analysed our dependent variable, 'Rented Bike Count' and also transformed it. Next we analysed categorical variable and dropped some variables which were not optimum for model building. We also analysed numerical variable, found out the correlation, distribution and their relationship with the dependent variable. We also removed some numerical features which had high collinearity and hot encoded the categorical variables.

Next we implemented some machine learning algorithms Linear Regression, lasso,ridge, elasticnet, decission tree, Random Forest and XGB Regressor. We did hyperparameter tuning(Gridsearch CV) to improve our model performance.

Now that we are finished implementing all the models, its time to evaluate them and conclude our findings and learnings over them.

Lets start by looking at the training scores for all the model



Also below are the testing scores for all the models.


No overfitting is seen, as we can see the models are performing well with the test data with good results.

• Random forest Regressor, Random forest Regressor with gridsearchCV and XGB Regressor gives the highest R2 score of 92%, 91% and 86% recpectively for test dataset.

• Feature Importance value for Random Forest and Gradient Boost are different.

However, this is not the ultimate end. As this data is time dependent, the values for variables like temperature, windspeed, solar radiation etc., will not always be consistent. Therefore, there will be scenarios where the model might not perform well. As Machine learning is an exponentially evolving field, we will have to be prepared for all contingencies and also keep checking our model from time to time. Therefore, having a quality knowledge and keeping pace with the ever evolving ML field would surely help one to stay a step ahead in future.
