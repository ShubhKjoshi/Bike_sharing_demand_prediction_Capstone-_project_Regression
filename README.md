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
  
Model	                                     MAE	 MSE  	  RMSE	 R2_score   Adjusted R2
Linear regression	                        4.474	 35.078  	5.923 	0.772	   0.77
Lasso regression	                        7.255	 91.594	  9.570 	0.405	   0.39
Ridge regression	                        4.474	 35.078	  5.923 	0.772	   0.77
Elastic net regression	                  5.792 	57.574  7.588	0.626	     0.62
Lasso regression with Cross-validation    4.474	 35.079	  5.923	  0.772	   0.77
Ridge regression with Cross-validation	  4.474	 35.078	  5.923  	0.772	   0.77
Decision tree regression	                3.562	 23.342	  4.831	  0.848	   0.85
Random forest regression	                 0.803 1.613	  1.270	  0.990	   0.99
Random forest regression with gridSearchCV 1.419 4.989	  2.234	  0.968	   0.97
XGBoost Regression	                       3.288 18.940	  4.352   0.877	   0.87


Also below are the testing scores for all the models.

Model	                                        MAE	    MSE	   RMSE	    R2_score Adjusted R2
Linear regression	                            4.474	  33.275	5.768  	0.772	   0.77
Lasso regression	                            7.456	  96.775	9.837	  0.387	   0.37
Ridge regression	                            4.410	  33.277	5.769	  0.789	   0.78	
Elastic net regression Test	                  5.874	  59.451	7.710	  0.624	   0.62
Lasso regression Test with cross-validation  	4.410	  33.276	5.769	  0.789	   0.78	
Ridge regression Test with cross-validation	  4.413	  33.291	5.770  	0.789	   0.78
Decision tree regression	                    4.031	  32.245	5.678  	0.796	   0.79
Random forest regression	                    2.203	  12.576	3.546	  0.920	   0.92
Random forest regression with gridSearchCV	  2.401	  14.174	3.765	  0.910	   0.91
XGBoost regression	                          3.508	  21.640	4.652	  0.863	   0.86

No overfitting is seen, as we can see the models are performing well with the test data with good results.

• Random forest Regressor, Random forest Regressor with gridsearchCV and XGB Regressor gives the highest R2 score of 92%, 91% and 86% recpectively for test dataset.

• Feature Importance value for Random Forest and Gradient Boost are different.

However, this is not the ultimate end. As this data is time dependent, the values for variables like temperature, windspeed, solar radiation etc., will not always be consistent. Therefore, there will be scenarios where the model might not perform well. As Machine learning is an exponentially evolving field, we will have to be prepared for all contingencies and also keep checking our model from time to time. Therefore, having a quality knowledge and keeping pace with the ever evolving ML field would surely help one to stay a step ahead in future.
