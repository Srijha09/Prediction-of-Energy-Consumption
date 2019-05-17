# Prediction-of-Energy-Consumption
Prediction of Energy Consumption using Machine Learning


About the dataset
Time Series Datasets can be slightly tricky for using and coming up with the right predictions using Machine Learning algorithms and neural networks.
I have used 3 datasets for the prediction of Solar energy consumption
1.	HISTORICAL DATA:  When historical data are given by steps of 15 minutes, forecasts are required by steps of 15 minutes. When historical data are given by steps of 1 hour, forecasts are required by steps of 1 hour. When historical data are given by steps of 1 day, forecasts are required by steps of 1 day.
•	Timestamp - The time of the measurement
•	Value - A measure of consumption for that building
2.	WEATHER FORECAST: It can be obtained for the OpenWeatherStation Website for the weather forecast of the place where the building is located.
•	Timestamp - The time of the measurement
•	Temperature - The temperature as measured at the weather station
3.	BUILDING DATA:
•	DAY_OF_WEEK]IsDayOff - True if DAY_OF_WEEK is not a working  day
•	Number of employees everyday

FEATURE EXTRACTION:
Feature Extraction: In this phase we need to validate the predictive power of new features as well as existing features. There are many techniques applied to validate the feature importance such as correlation analysis, ensemble and tree based model based feature importance.
Feature Transformation/Derivation: during the validation with a baseline model some of the feature may require transformation. These transformations include log transformation, Standard Scaling (SS) and Min Max Scaling (MMS).  After literature survey and consultation with subject matter expert, a set of most desirable features for electricity load/consumption forecasting were listed.  :
a) Past consumption pattern: electrical consumption pattern cannot change abruptly until unless some major changes happen at the place. So past consumption pattern carries information for future consumption pattern.  
b) Calendar:  month, day of week, 
c) Demography: The population of building can affect the consumption pattern
d) Geography:, temperature, etc. If temperature is high, people will use more electrical appliance and similarly when temperature is low.


ALGORITHMS AND MODELS TO BE USED FOR THE PREDICTION ANALYSIS:

LINEAR REGRESSION
 We'll train a Linear Regression model for predicting building energy consumption based on historical enregy data, several weather variables, hour of the day, day of the week, weekends and holidays.
The accuracy obtained is 63.74%
USING NEURAL NETWORKS:
LSTMs (or long-short term memory networks) allow for analysis of sequential or ordered data with long-term dependencies present. Traditional neural networks fall short when it comes to this task, and in this regard an LSTM will be used to predict electricity consumption patterns in this instance.
The accuracy obtained for this model is 97.12%

So we can conclude that deep neural networks such as LSTMs are more useful for prediction of energy consumption.



