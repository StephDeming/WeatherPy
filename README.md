# WeatherPy

Data analysis of world weather data to better understand and explain what the weather is like close to the equator. Used Python, Matplotlib, Citipy, the OpenWeatherMapAPI, the Google Places API, and other technologies to help create a representative model of weather across world cities.

## Analysis
For the first part of this project (WeatherPy), I created a Python script to visualize the weather of 500+ cities across the world of varying distances from the equator. Using the numpy package, I generated a random set of at least 500 latitude and longitude coordinates and used a package called Citipy to identify the nearest city for each latitude and longitude pair. I then made API calls to the OpenWeatherMap API to get weather data for each of the cities. After the API calls were complete, I saved the retrieved data to a csv file, which can be found here.

Using the data I received from the OpenWeatherMap API, I built a series of scatter plots to visualize the following relationships:

- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

For the second part of this project (VacationPy), I used the weather data gathered from part one to help plan for future vacations. Specifically, I used jupyter-gmaps and the Google Places API to create a heatmap that displays the humidity for every city from part one. I then narrowed down the list of cities to find the ideal weather conditions, including:

- A max temperature lower than 80 degrees but higher than 70.
- Wind speed less than 10 mph.
- Zero cloudiness.
- Dropped anr rows that didn't conatin all three conditions.

I then used the Google Places API to find the first hotel for each city located within 5000 meters of the coordinates. Finally, I plotted the hotels on top of the humidity heatmap with each pin containing the hotel name, city, and country.

## Conclusion
- Temperature seems to have a clear correlation with latitude
- As expected, the weather becomes significantly warmer as one approaches the equator (0 Deg. Latitude). The southern hemisphere tends to be warmer this time of year than the northern hemisphere
- There is no strong relationship between latitude and cloudiness. However, it is interesting to see that a strong band of cities near 0, 80, and 90% cloudiness
- There is no strong relationship between latitude and wind speed. However, in northern hemispheres there is a flurry of cities with over 20 mph of wind
- Wind speed tends to generally be betweeen 0 and 15 mph regardless of latitude
- There is no strong relationship between latitude and humidity. however there is a slightly larger cluster of northern hemisphere cities with high humidity (above 60% humidity)
- The same analysis is also used in a mockup website for another project. 

## Technologies
- Python
- Pandas library
- Jupyter Notebook
- Matplotlib library
- Citipy (will need to be installed in your anaconda environment)
- OpenWeatherMap API
- Google Places API
- jupyter-gmaps


