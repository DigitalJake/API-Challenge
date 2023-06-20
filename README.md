# Python-API-Challenge

## WeatherPy

![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/55210b46-5dca-4d46-a879-71580dd9365d)

In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

###  Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/6213ae20-ed79-4546-a0ad-ed1e925fa678)

Latitude vs. Humidity
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/fc906772-ace2-4695-9f15-9cf6816eef41)

Latitude vs. Cloudiness
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/3bad6a82-c19b-44a5-8807-f00d3ef6585e)

Latitude vs. Wind Speed
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/19eb4d53-ce76-4ad6-b29b-100487de8ded)

### Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values as you can see in the following image

You should create the following plots:

- Northern Hemisphere: Temperature vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/a6ffa43d-4089-47b6-89f3-d1bc3267de76)

- Southern Hemisphere: Temperature vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/9c21b263-aca1-4508-87b0-6a8e01d0fa1f)

- Northern Hemisphere: Humidity vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/3b846b54-7df5-4be9-a603-55bb82308034)

- Southern Hemisphere: Humidity vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/27469bb3-490a-43a2-abd0-eb532b4065bf)

- Northern Hemisphere: Cloudiness vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/42e8e863-0e74-4b93-aa0f-9e33080f5343)

- Southern Hemisphere: Cloudiness vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/c22a0230-9652-44cc-91bb-031718d868da)

- Northern Hemisphere: Wind Speed vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/959f7f08-84b0-468c-85f2-1f42d7143e42)

- Southern Hemisphere: Wind Speed vs. Latitude
![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/8dfd2d4a-7a94-49aa-b5d6-bd1b549ad6f0)

After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

## VacationPy

![image](https://github.com/DigitalJake/API-Challenge/assets/120591725/25bfd188-323f-4c89-ad4c-45ebbea38cd9)

In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

- Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

- Narrow down the city_data_df DataFrame to find your ideal weather condition. 
For example:
  - A max temperature lower than 27 degrees but higher than 21
  - Wind speed less than 4.5 m/s
  - Zero cloudiness

- Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

- For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

- Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:
