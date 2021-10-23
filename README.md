# python-api-challenge

Unit 6: APIs HOMEWORK 

Included in this repository is my solution for the Unit 6: APIs Homework for the Georgia Tech Analytics Bootcamp.

In this assignment, we were asked to analyze weather data from 500+ cities around the world and make some simple observations and help plan a possible vacation, using the OpenWeatherMapAPI and the Google Places API to generate the needed data. This task was broken up into two parts WeatherPy and VacationPy.

For WeatherPy, we were given some code to generate random cities that had varying distances from the equator, so that we could see how a city's latitude effected certain aspects of the weather. In order to get the weather for each city, we had to run the city's name through the OpenWeatherMapAPI, which gave us Latitude, Longitude, Max Temperature, Humidity, Cloudiness, Wind Speed, etc. Some of the cities in the initial list were left out here because they weren't in the API. We saved that dataframe into a csv to use for VacationPy. Then, we graphed scatter plots for Latitude vs Max Temperature, Humidity, Cloudiness, and Wind Speed. There are some comments on each of these graphs to give a feel for what is happening. Finally, we split the data into Northern and Southern Hemispheres, and did a line regression for each of the catagories to see closer how the data acts relational to the equator. There are three observations at the bottom of the script.

For VacationPy, we use the data that was generated from WeatherPy, and create a heat map using the humidity value as the weight. then, we were asked to to narrow down the data within certain perameters to find the ideal vacation spot. Once we had the locations for the vacation spot, we were tasked with finding the nearest hotel, and ploting it onto the previous heat map.

The biggest road block that I ran into in this assignment was trying to clean the data from starting the columns as empty. It caused problems for the original for plot and made the linear regression impossible. I had to go through and change all the empty values to NaN values and then dropping them entirely from the dataframe. It should run fine now, but it caused a major headache.

Includes:
1. WeatherPy Folder
    a. the script named WeatherMain.py
    b. the csv file (cities.csv) that hold the weather data for the list of cities
    c. Images folder that holds all the png images of graphs
2. VacationPy Folder
    a. the script named VacationMain.py
    b. Images folder that hold the screen shots of the maps