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

### Aout the Dataset
This dataset contains 14,58,644 rows and 11 columns.There is no null values and duplicate values in the dataset. The data types of the pickup_datetime and dropoff_datetime are object type.It need to be converted in to datetime data type. 

### Manipulations done in the dataset

The following manipulations were done in the datawrangling process


*   The pickup and drop datetime columns were converted to datetime data type from object type.
*   Assigning new columns to the dataframe for weekday number, month,hour and weekday,period for both pickup and dropoff.
*   Distance was calculated for each trip and added as a new column.
*   Speed of the trip was calculated and added as a new column.

###  Manipulations have done in dataset and insights found

The following manipulations were done in the datawrangling process


*   The pickup and drop datetime columns were converted to datetime data type from object type.
*   Assigning new columns to the dataframe for weekday number, month,hour and weekday,period for both pickup and dropoff.
*   Distance was calculated for each trip and added as a new column.
*   Speed of the trip was calculated and added as a new column.

### Evaluation metrics considered for a positive business impact 

The following evaluation metrics have been considered for positive business impact.

*   Mean Absolute Error (MAE):It is a metric for evaluating prediction accuracy by calculating the average magnitude of errors in predictions, regardless of direction. The goal in regression model is to minimize the MAE, leading to improved accuracy and positive business impact.
* italicized text Mean Squared Error (MSE): It measures the average squared difference between the actual and predicted values and provides a numerical representation of the average error in the model's predictions. The MSE is often used as a loss function in the training process of machine learning models and the goal is to minimize this value, resulting in a more accurate model. 
*   Root Mean Squared Error (RMSE): It  is a popular evaluation metric for regression models, calculated as the square root of the Mean Squared Error. This  making it easier to understand the magnitude of prediction errors.
*   Mean Absolute Percentage Error (MAPE): It  is a metric  to evaluate the accuracy of predictions. It is calculated as the average of the absolute percentage differences between the actual and predicted values. With the help of MAPE an analyst can easily explain the percentage error. This metric is considered as one of the most important regression metric in time series data for a positive business impact.
*   R2 Score: The R2 Score is a commonly used metric in regression analysis, measuring the proportion of the dependent variable's variance explained by the independent variables in the model. It provides insight on model fit and comparison, helping in decisions about model selection and analysis.
*   Accuracy: It is calculated as the average of the absolute percentage differences between the actual and predicted values. A lower value of 100-MAPE indicates a more accurate model, with a higher degree of similarity between the actual and predicted values.


###  ML model  choosed from the created models 
LightGBM model has been choosen from the above models.It performs well in all metric scores such as Accuracy,R2 Score,MAE,MSE,RMSE and MAPE.


### The model which  have been used and the feature importance using model explainability tool
LightGBM is an effective gradient boosting framework for both linear and tree-based regression models. It uses gradient boosting to optimize the parameters and due to that loss will be reduced. Initially It trains a series of simple models, such as decision trees, after that it combines their predictions to form a stronger model. Regularization and parallel processing are salient features of this algorithm. The interpretability of the model further improved by LIME and SHAP. 

# **Conclusion**

**From the EDA**

Exploratory Data Analysis (EDA) is a fundamental part of data analysis that facilitates a primary research of the dataset to identify patterns, anomalies, and relationships, detect potential issues, and inform advanced analytical methods.The thorough understanding of the data and leads further study were provided by the EDA.. The following conclusions are found from EDA.

*   	Most of the trips are with single passenger
*   Most of the trip duration are within 15 minutes and 30 minutes
*   Vendor 2 has slightly more trips than vendor 1
*   Most of the trips distances are within 100km
*   The trip details stored in vehicle memory is 0.6% only
*   Most of the trips are between 10 to 20 km/h.Very few trips are 50 to 60km/h
*   	More busiest hours in pickup and dropoff is between 6pm to 7pm.
*   March, April and May months are more demand for the vehicles compared to other months.
*   Pickup and dropoff are more in evening period and morning period.
*   Friday and Saturday the vehicle usage is more.
*   During 7pm to 8pm the trips are more for both vendors.Vendore 2 is more compared to vendore 1 during that period.
*   Vendore 2 has the more duration of trips.
*   pickup hour and drop hour highly correlated.trip duration nd distance highly correlated.
*   During 4 passanger traveling the trip duration are more.


**From the ML Model Implementation**

*   Effective implementation of an ML model requires proper data selection and preprocessing, regular evaluation and tuning, use of appropriate evaluation metrics, integration for easy maintenance, consideration of ethical and legal factors, appropriate algorithm choice, efficient hyperparameter tuning, and transparency in results.
*   Initially simple Linear Regression model was tried after that Lasso Regression, Ridge Regression and Elasticnet Regression have been tried with hyper parameter tuning but significant result was not received
*   The advanced linear algorithms such as .DecisionTree, LightGBM and XGBoost have been checked. Finally LightGBM with gradient boosting technique performed well.
*   In the LightGBM with RandomizedSearchCV the maximum accuracy  87.29% in test has been achieved.
*   By analyzing 7 machine learning models, LightGBM has been selected as the optimal model for predicting NYC taxi trip duration. The performance of the model can be further improved by incorporating PCA technique for features selection.
