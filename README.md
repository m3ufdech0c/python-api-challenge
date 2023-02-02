# python-api-challenge
Module 6 API challenge

Part 1: WeatherPy
In this challenge, we are using Python to write a script to visualize the weather of over 500 cities of varying distances from the equator. Using citipy Python library Links to an external site., the OpenWeatherMap API Links to an external site., to create a representative model of weather across cities.

First, we'll be generating random geographic coordinates and the nearest city to each latitude and longitude combination that is provided, please refer to the comments in the script for step by step instructions and how this is done.

From there, we'll create Plots to showcase the Relationship Between Weather Variables and Latitude, by using the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Then we'll create scatter plots to illustrate the following relationships:

Latitude vs. Temperature

Latitude vs. Humidity

Latitude vs. Cloudiness

Latitude vs. Wind Speed

Next the correlation coefficient and Linear Regression will be computed for the relationships listed above, only this time in each hemisphere. This is fullfilled by creating 2 dataframes;
first one for the Northern Hemisphere (where latitude > 0) 
second one for the Souththern Hemisphere (where latitude < 0)
(please refer to the comments in the script) 

Part 2: VacationPy
In this portion we will be planning for future vacations using Jupyter notebooks, the geoViews Python library, and the Geoapify API.

First we will load the CSV file with the weather and coordinates data for each city created in Part 1.

We will then use the Geoapify API and the geoViews Python library to create map visualizations of those cities. The size of the point is the humidity in each city. (please refer to the comments in the script for more details on the steps)

Second, we will narrow down the city_data_df DataFrame to find our ideal weather condition. i.e:

Max temperature lower than 31 degrees but higher than 18 degrees

Wind speed less than 5 m/s

Zero cloudiness

Then we will create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity. 

For each city, we will use the Geoapify API to find the first hotel located within 10,000 meters of the coordinates.

Finally we will map each city and add the hotel name and the country as additional information in the hover message.