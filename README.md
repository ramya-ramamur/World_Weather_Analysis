# World_Weather_Analysis

# Overview
An analysis and visualization of weather data across 500+ cities worldwide for a travel app called "PlanMyTrip" that will use the data to recommend ideal hotels based on clients' weather preferences to travellers so that they can plan their itinerary. 

### Resources
* Data Source: 
    1. Weather Database: WeatherPy_Database.csv
    2. Vacation Data : WeatherPy_vacation.csv
* Software: Python 3.8.8, Pandas Dataframe, Matplotlib, CitiPy, SciPy, Python Requests, APIs, JSON Traversals, Jupyter Notebook 6.3.0
* API's accessed:  OpenWeatherMap API, Google Maps and Places API, Google Maps Directions API

# Summary of Results

## Deliverable 1: Retrieve Weather Data
Generated a set of 2,000 random latitudes and longitudes, and retrieved the nearest cities. Performed an API call with the OpenWeatherMap and the following information was extracted from the API call:
* Latitude and longitude
* Maximum temperature
* Percent humidity
* Percent cloudiness
* Wind speed
* Weather description (for example, clouds, fog, light rain, clear sky)
The above data was captured in a Pandas Dataframe and exported to a "WeatherPy_Database.csv" file. An excerpt of the dataframe is as follows. 
<img width="926" alt="weather_database" src="https://user-images.githubusercontent.com/75961057/144698144-c15a395c-86dd-4e8c-8c67-37da2c5285c2.png">

## Deliverable 2: Create a Customer Travel Destinations Map
Using input statements from customer to get customer weather preferences, then used those preferences and data collected in "WeatherPy_Database.csv" file,  to identify potential travel destinations and nearby hotels, and exported the data to a 'WeatherPy_vacation.csv" file. The data is visualized on a world map that show those destinations on a marker layer map with pop-up markers.


<img width="734" alt="vacation_search" src="https://user-images.githubusercontent.com/75961057/144698291-b1532258-3fef-4166-ada4-b43e1bd7a823.png">


<img width="1072" alt="WeatherPy_vacation_map" src="https://user-images.githubusercontent.com/75961057/144698352-98ff6ddd-4768-4ed0-b82a-3b915cca4478.png">

## Deliverable 3: Create a Travel Itinerary Map
Using the Google Directions API and data from 'WeatherPy_vacation.csv", created a sample travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, created a marker layer map with a pop-up marker for each city on the itinerary.

Sample Travel Itinerary of four cities in USA starting and ending at North Myrtle Beach. 

<img width="828" alt="Sample Travel Itinerary" src="https://user-images.githubusercontent.com/75961057/144698597-e7451161-f951-4be3-977d-a39b4de2c4e4.png">

Vacation Travel Route

<img width="1427" alt="WeatherPy_travel_map" src="https://user-images.githubusercontent.com/75961057/144698661-785a746c-3355-4d1c-973d-5d7d9f645ddd.png">

Vacation Hotel and Weather Pop-up Marker Map

<img width="1440" alt="WeatherPy_travel_map_markers 6 53 19 PM" src="https://user-images.githubusercontent.com/75961057/144698735-2e19c0e8-91f7-4596-b3d9-169231939d2b.png">
