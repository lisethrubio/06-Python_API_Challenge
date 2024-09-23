# 06-Python_API_Challenge

## Overview: 
This project is divided into two main deliverables: WeatherPy and VacationPy, each of which involves the use of various Python libraries, APIs, and data visualization techniques to analyze weather data across cities and make travel recommendations based on specific weather conditions.

## Part 1: WeatherPy
In this section, the goal is to create a Python script that visualizes the weather of over 500 cities located at varying distances from the equator. The `OpenWeatherMap API` is used to retrieve current weather data for a generated list of cities, and the relationships between weather variables and latitude are analyzed. `Scatter plots` are created to analyze the relationship between *`"latitude"`* and various weather conditions, such as *`"temperature"`*, *`"humidity"`*, *`"cloudiness"`*, and *`"wind speed"`*. 

Also, a `linear regression` is computed separately for cities in the `Northern Hemisphere` (latitude ≥ 0°) and `Southern Hemisphere` (latitude < 0°) to analyze the relationship between latitude and the same various weather conditions.  
Each scatter plot displays the regression line, the linear regression formula, and the r² value to explain how well latitude explains the variance in these weather variables.

## Part 2: VacationPy

In this section, the goal is on using the previously gathered weather data to help plan future vacations. Using the `Geoapify API` and the *`geoViews`* library, the goal is to create interactive maps that display cities meeting ideal weather conditions and find hotels in those locations.

A map is therefore created to display a point for each city from the *`"city_data_df"`* DataFrame. The size of the point represents the humidity in that city. The data is then narrowed down based on ideal weather conditions. 
For each city that matches the ideal weather conditions, the `Geoapify API` is used to find the nearest hotel within a 10,000-meter radius of the city's coordinates.
A new DataFrame called *`"hotel_df"`* is created to store the *`"city"`*, *`"country"`*, *`"coordinates"`*, *`"humidity"`*, and the *`"hotel name"`*.

The map is enhanced to include additional information, such as the hotel name and the country, in the hover messages for each city. This allows users to easily identify which cities have favorable weather conditions and available hotels.


## References
- Xpert Learning Assistant
- AskBCS Learning Assistant
- Curriculum content
- Tutoring