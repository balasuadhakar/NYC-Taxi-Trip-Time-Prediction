# **Project Name**    - NYC Taxi Trip Time Prediction Regression Project 

##### **Project Type**    - Regression
##### **Contribution**    - Individual
##### **Team Member 1 -** Arumugam Balasuadhakar

# **Project Summary -**



*   The duration of trip prediction is essential for all travel based business. The current project is based on the machine learning regression model used to predict the taxi trip duration in New York City. The main aim of this project is to provide more precise approximation of trip duration for the customers and drivers.

*   The past data of taxi trip in NYC have been used for developing the model. The data contained the information such as pickup datetime, dropoff datetime,  Passenger count, pickup longitude, pickup latitude, drop off longitude, drop off latitude, store_and_fwd_flag, and trip duration. The preprocessing was done for the data to handle missing values and transform categorical variables.The additional information such as distance between the location, day of the week  and time have been extracted by applied on future engineering techniques.
*   The regression algorithms such as linear regression, Lasso regression, ridge regression, elastic net regression classification tree,lightgbm and XG Boost have been adopted for developing the model. The optimization of the performance of the developed model was done by hyper parameter tuning. The MAE,MSE,RMSE,MAPE,R2 and Accuracy are the matrices used to evaluate the model. The LightGBM Regression model was performed well compared to other model. It was observed from the result the  model can able to predict the duration of drip with very less average error.

*  The important features to predict the duration are identified in this project; those are location for pickup and drop, time and the distance. Finally the machine learning regression algorithm has successfully established for predicting the duration of NYC taxi trip.

# **Problem Statement**
The one of the most crowded city in the word is New York. The crucial aspect of city infrastructure is transporting system. The more popular mode of transport in New York is taxis. The traffic; weather condition and time of the day are the some of the important factors for influencing trip duration. The estimation of trip duration is difficult for passengers and drivers.

The aim of this project is to develop a machine learning regression model for predicting the taxi trip duration in New York City. The prediction will be based on various input features such as the pickup and dropoff locations, the time of day, and the distance of the trip etc. The accuracy of the predictive model should be high level. The model also able to show the most important factors for predicting duration of trips. The efficiency and convenience of taxi service will be improved by the best optimized model.

### Variables Description 

* id - a unique identifier for each trip

* vendor_id - a code indicating the provider associated with the trip record

* pickup_datetime - date and time when the meter was engaged

* dropoff_datetime - date and time when the meter was disengaged

* passenger_count - the number of passengers in the vehicle (driver entered value)

* pickup_longitude - the longitude where the meter was engaged

* pickup_latitude - the latitude where the meter was engaged

* dropoff_longitude - the longitude where the meter was disengaged

* dropoff_latitude - the latitude where the meter was disengaged

* store_and_fwd_flag - This flag indicates whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server - Y=store and forward; N=not a store and forward trip.

* trip_duration - duration of the trip in seconds



