# Module-6---Python-APIs   
Data analysis and manipulation utilizing python APIs     

## Part 1: WeatherPy  
In this deliverable, I created a Python script to visualize the weather of over 500 cities of varying distances from the equator. I used the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and my own problem-solving skills to create a representative model of weather across cities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, I used the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, I created a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature <br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/52c8f828-ff83-4f04-8904-1caa228777c0)

Latitude vs. Humidity<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/60fd75d4-7666-4359-9a1a-de89fcbf32d6)

Latitude vs. Cloudiness<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/663e29ea-fca7-47ed-9226-ccd78bd0827b)

Latitude vs. Wind Speed<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/33421780-3a0d-4006-bd80-4a2f4a70cced)


### Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, I computed the linear regression for each relationship. Separated the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). I defined a function in order to create the linear regression plots.

Next, I created a series of scatter plots that include the linear regression line, the model's formula, and the r values.<br />

Northern Hemisphere: Temperature vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/3f2543a5-ff1e-46e5-8909-5734aa464e7c)

Southern Hemisphere: Temperature vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/76f80924-47f7-4428-8367-626209d35ce4)

Northern Hemisphere: Humidity vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/05a68f6d-b324-423c-9a4a-51c358e1ce73)

Southern Hemisphere: Humidity vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/58325482-7d72-4d98-a5e0-49af76ce63c9)

Northern Hemisphere: Cloudiness vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/469d683b-beda-48cb-90fe-030dfecbaaa9)

Southern Hemisphere: Cloudiness vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/d9d8c0d6-2bca-46a3-bcc4-8718fba5bd31)

Northern Hemisphere: Wind Speed vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/bfbc066d-9d89-4996-ab15-048503ebf742)

Southern Hemisphere: Wind Speed vs. Latitude<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/6d07d1f0-63c7-4b0a-9d90-e70f7f01eb97)


After each pair of plots, I explained what the linear regression is modeling and described any relationships that I noticed.


## Part 2: VacationPy
In this deliverable, I used my weather data skills to plan future vacations. I also used Jupyter notebooks, the geoViews Python library, and the Geoapify API.

### My main task was to to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.


Created a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/fb609613-ecaf-4d92-b6be-6a2c6b7d5bd5)

Narrow down the city_data_df DataFrame to find your ideal weather condition. <br />

My ideal weather conditions:<br />
A max temperature lower than 70 degrees.<br />
Cloudiness less than 15%.<br />
Humidity less than 40%.<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/fda5c123-65de-41cf-8046-fa3d33756538)



Created a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/28989b02-0a9e-410d-92d4-81e9b28cb90a)

For each city, used the Geoapify API to find the first hotel located within 10,000 meters of my coordinates.<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/1a82b531-c2e3-4092-a178-a5d7be5a540c)

Added the hotel name and the country as additional information in the hover message for each city on the map.<br />
![image](https://github.com/dclaxto1/Python-API-Challenge/assets/128431134/931dac2b-aa35-4d46-bf91-8aa929d2c4a1)
