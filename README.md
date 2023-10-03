# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
Do create a model that attempts to predict trends of bike availability at bike stations accross a city based on API data on specific business categories within a 1km radius of each bike station.

With Toronto as my city, the business categories as "restaurants", "bars", and "performance art venues", the APIs of Foursquare, citybikes, and Yelp, I created a linear regression model in the attempt to find correlated data.

## Process
### step 1
Obtain CityBike Data and use the latitude and longitude for each bike station as a parameter for my requests to the Foursquare and Yelp APIs

### step 2
Determine which of the API data sets yielded better measures for a linear regression model. Then I joined the yelp data with the city bike data to associate the independent variable of my model "free_bikes".

### step 3
EDA of model variables, checking especially for correlation and cleaning the data from outliers.


## Results
The Yelp Data was much more detailed in quantitative data and provided more places of interest than the Foursquare API.  

The R-Squared Value 0.005 shows this model being completely useless.  The distance is the only independent variable with a P-value below a benchmark 5%, making it statistically significant relative to this model.  However, the correlation found between distance and free_bikes during EDA shows a very low positive correlation. Additionally, the linear relationship assumption was not met for any variables, so this model does not have practical use.

## Challenges 
Yelp API limited the amount of data I could retrieve for my model.  The API request formats (list/JSON/Dictionary) proved difficult where work arounds were needed initially, but ultimately discarded.

## Future Goals
More Yelp API requests, though I do believe the model would still be useless.
