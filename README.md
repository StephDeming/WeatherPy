# WeatherPy

The Python code randomly selects a group of 500+ cities across the world. Then, the code collects data from the OpenWeatherMap API to create a representatitve model of weather across world cities. The API data is used to graph the following relationships:

- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

## Conclusion
- Temperature seems to have a clear correlation with latitude
- As expected, the weather becomes significantly warmer as one approaches the equator (0 Deg. Latitude). The southern hemisphere tends to be warmer this time of year than the northern hemisphere
- There is no strong relationship between latitude and cloudiness. However, it is interesting to see that a strong band of cities near 0, 80, and 90% cloudiness
- There is no strong relationship between latitude and wind speed. However, in northern hemispheres there is a flurry of cities with over 20 mph of wind
Wind speed tends to generally be betweeen 0 and 15 mph regardless of latitude
- There is no strong relationship between latitude and humidity. however there is a slightly larger cluster of northern hemisphere cities with high humidity (above 60% humidity)

## Files
- The analysis includes the following files:
- A "WeatherPy.ipynb" Jupyter Notebook that contains the Python code for the analysis
- A "api_keys.py" Python file that contains the OpenWeatherMap API key used in the analysis. If downloading this analysis, the user must put her or his OpenWeatherMap API key into this file in order for the "WeatherPy.ipynb" Jupyter Notebook to work properly
- A "weather_df.csv" CSV file in the "Output" folder that contains the CSV version of the DataFrame created in the Jupyter Notebook
- Four PNG files in the "Figures" folder. Each of the four files is a graph created in the analysis

