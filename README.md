# World_Weather_Analysis

## Overview of the Analysis 
In this assignment, students were asked to complete an API pull from openweathermap.org to retrieve current data and description for various cities using randomly generated latitudes and longitudes. 

A database was created with the country, city name, coordinates, maximum temperature, humidity, cloudiness, wind speed, and weather description. The finalized database contains 706 cities. The cities from this database was used in the vacation search assignment and results from the vacation search was used later to develop a vacation itinerary based on user's temperature preferences. Next, users were asked to input their their max and minimum preferred temperature. Based on that list a preferred list of city was generated. Based on the coordinates and available values, users then use google direction api to get json data to query the nearest hotel within a 5000 meter radius. The finalized results include: a vacation map, a travel map with a heat layer, and a travel map with markers connecting locations on a csustomized itinerary. 

## Summary
The vacation search and itinerary maps contain markers that provide users with information regarding the hotel, city name, country, current weather and max temperature. Additionally, the vacation search contains a heat map layer that depicts the intensity of data at the hotel marker location. While, the itinerary file includes a hotel markers for four destinations and connect the different destinations based on the order in which they appear in the itinerary. Below you will find a travel map with markers.

<img src = 'https://github.com/osbornej-tech/World_Weather_Analysis/blob/main/Resources/WeatherPy_travel_map_markers.png'>

## Datafiles
OpenWeatherMap API

## Dependencies
import pandas as pd
import requests
import gmaps
import ipywidgets as widgets
widgets.IntSlider()
import numpy

# Import API key
from config import g_key
