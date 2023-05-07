# Module-6---Python-APIs
Data analysis and manipulation utilizing python APIs

Part 1: WeatherPy
In this deliverable, I created a Python script to visualize the weather of over 500 cities of varying distances from the equator. I used the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and my own problem-solving skills to create a representative model of weather across cities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, I used the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, I created a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, I computed the linear regression for each relationship. Separated the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). I defined a function in order to create the linear regression plots.

Next, I created a series of scatter plots that include the linear regression line, the model's formula, and the r values.

Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots, I explained what the linear regression is modeling and described any relationships that I noticed.


Part 2: VacationPy
In this deliverable, I used my weather data skills to plan future vacations. I also used Jupyter notebooks, the geoViews Python library, and the Geoapify API.

My main task was to to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.


Created a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

Narrow down the city_data_df DataFrame to find your ideal weather condition. 

My ideal weather conditions:
A max temperature lower than 70 degrees.
Cloudiness less than 15%.
Humidity less than 40%.



Created a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, used the Geoapify API to find the first hotel located within 10,000 meters of my coordinates.

Added the hotel name and the country as additional information in the hover message for each city on the map.
