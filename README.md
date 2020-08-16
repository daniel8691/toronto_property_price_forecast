# toronto_property_price_forecast

Data used for this analysis were webscrapped from [a toronto listings website](https://toronto.listing.ca/condo-price-history.htm). 

### Data Cleaning
* Edited recorded data to meet the requirements of float datatypes (ie. remove dollar signs or commas)
* Make sure features in the study have to correct datatypes


### LSTM Models
First used Python's statsmodels library to uncover any trends and seasonalities within the dataset
![trends_seasonality](https://github.com/daniel8691/toronto_property_price_forecast/blob/master/project_images/seasonal_trends.png)

Developed a prediction model using the Keras library. Only monthly average sold price were used to make the prediction
![LSTM_prediction](https://github.com/daniel8691/toronto_property_price_forecast/blob/master/project_images/test_prediction_lstm.png)


### Facebook Prophet Models
We can see that the model predicted with similar results as the LSTM model
![prophet_forecast](https://github.com/daniel8691/toronto_property_price_forecast/blob/master/project_images/fb_prophet_forecast.png)

![prophet_trend](https://github.com/daniel8691/toronto_property_price_forecast/blob/master/project_images/fb_prophet_trend.png)

![prophet_prediction](https://github.com/daniel8691/toronto_property_price_forecast/blob/master/project_images/fb_prophet_prediction.png)


This is my first project using LSTM with keras and the Facebook Prophet open-source library. 
**Future considerations** can be mortgage interest rates from the big 5 Canadian Banks
* Immigration Levels (Population Growth)
* GDP Growth
* Unemployment Rate
* Consumer Confidence Index
* Manufacturing PMI



