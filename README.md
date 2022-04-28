# World Weather Analysis - Using APIs

## Overview of World Weather Analysis

The purpose of this assignment was to make some recommended improvements to the PlanMyTrip app by adding the Weather Description to weather data, which would allow beta testers to use specific input statements to filter the data toward their preferences.  To do this I first generated a set of 2,000 random latitudes and longitudes using the citipy module, which allowed me to retrieve the nearest city to those coordinates.  I then completed an API call with the OpenWeatherMap to determine what the current weather conditions were at those locations and added that to a new dataframe from which I could export to a WeatherPy_Database csv file. 

I was then able to leverage this csv file to determine which cities met the inputs that had been defined by the user.  The user was interested in cities that had a minimum temperature of 75 degrees, and a maximum temperature of 90 degrees.  This established a filtered dataset that I was able to use to create a second new dataframe that listed the cities that met the temperature criteria of the user, as well as a list of hotels within those cities that might make sense for the user to book their stay.  From there we created a map that had a marker for each hotel as well as the relevant information (Hotel Name, City, Country, Current Weather) for each hotel for the user to have a visual.  

Lastly, I created a travel itinerary to show the route between the four city stops that the user had selected for their vacation.  To do this I made a Google API call to illustrate a driving route on the map between and show the relevant hotel information at each marker on the map.
     

