# World_Weather_Analysis

## Project Overview
Jack loves the PlanMyTrip app. Beta testers love it too. And, as with any new product, they’ve recommended a few changes to take the app to the next level. Specifically, they recommend adding the weather description to the weather data you’ve already retrieved in this module. Then, you'll have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, you will create a travel route between the four cities as well as a marker layer map. 

### Purpose
Purpose of this analysis is to have the beta testers input their weather preferences, which will be used to identify potential travel destinations and nearby hotels.

## Resources
- Data Source: Vacation_Itinerary.csv and Vacation_Search.csv
- Software: Python 3.8, Visual Studio Code, 1.46.1

## Results

### Weather Database
- The new Weather Database contains the following information from the API call with OpenWeatherMap:
    - Latitude and longitude
    - Maximum temperature
    - Percent humidity
    - Percent cloudiness
    - Wind speed
    - Weather description
    
![Weather_Database](https://github.com/grwon/World_Weather_Analysis/blob/master/Weather_Database/Weather_Database.png)   

### Vacation Search
- Beta testers were prompted to enter their minimum and maximum temperature criteria for their vacation. A new DataFram was created based on the minimum and maximum temperature and empty rows were dropped. We then retrieved the hotel names and added to the DataFrame, the rows with no hotel information were dropped. See the below picture of a marker layer map with pop-up markers for the cities in the vacation DataFrame. Each marker provides the following information:
    - Hotel name
    - City
    - Country
    - Current weather description with the maximum temperature
    
![WeatherPy_vacation_map](https://github.com/grwon/World_Weather_Analysis/blob/master/Vacation_Itinerary/WeatherPy_travel_map.png)

### Travel Itinerary Map
- A travel itinerary is created using the Google Directions API. It shows the route between four cities chosen from the customer's possible travel destinations. A marker layer map with a pop-up marker for each city on the itinerary is created.

![WeatherPy_travel_map](https://github.com/grwon/World_Weather_Analysis/blob/master/Vacation_Itinerary/WeatherPy_travel_map.png)
![WeatherPy_vacation_map_markers](https://github.com/grwon/World_Weather_Analysis/blob/master/Vacation_Itinerary/WeatherPy_travel_map_markers.png)


## Summary
- This analysis provided the beta user with a detination map that contains potential travel destinations based on their weather preferences. We then created travel itinerary map for the users based on four cities chosen from the potential travel destinations. A marker layer map with pop-up markers for the four cities in the vacation DataFrame is created to help users visualize their potential travel destinations and nearby hotels.
