# Project-1-Tip-Analysis-of-NYC-Taxi-Drivers

This project aims to predict the amount of tips for Yellow Taxis by the hour in New York City based on the weather of the day. The prediction models that we will be using will be the Linear Regression Model, and the Random Forest Regression Model. The data needed to train those two models will be sourced from the Taxi and Limousine Commision in New York City called - 2023 Yellow Taxi Trip Data, and the weather data which is sourced from an api using the Open-Meteo website.

This project is meant tot be ran in chronological order, starting from the file - RawTransformation, which will take all our landing data from the New York City TLC, and clean it, transforming it into the raw data in order to be preprocessed in the next step. The next step will be to have to run the Preprocessing file, which takes all of our data and preprocesses it. This filters everything that we would not need for analysis, including mistakes in the data, missing values, impossible records and etc. Following up on that, in the file FeatureEngineering, all the data that has been preprocessed will have to undergo feature engineering. One of this example would be to create a featuere counting the duration of the trip. Not only that, this file will also run our visualisations. The visualisations will be based on the Temporal and Geospatial data which we have obtained through the Trip Records and Open Meteo weather data.

However, before obtaining our weather data, we would need to download some modules that can allow us to retrieve the weather data:

pip install openmeteo-requests pip install requests-cache retry-requests numpy pandas

Making sure that these 2 modules are installed into our environment will allow us to use the api to read in the hourly data for 2023 in New York City. The data of New York City from Open Meteo is based on the longitude and latitude, and timing of the day. The data that were retrieved, were the depth of the snow, wind speed, the rain and the temperature of the hour based on day, month of the year.

Last but not least, we run the Modelling file, where we can train our Linear Regression and Random Forest Regression model. We then finish off our project by comparing the two models performance in predicting the average tip amounts by the hour in January of 2024 in New York City.
