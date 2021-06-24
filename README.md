# Google Weather Forecast Scraper

A simple BeautifulSoup scraper for Google/(weather.com) weather forecast data.

## Features

+ Automatic units detection and conversion.
+ Extracts current weather data, containing "Weather Condition", "Temperature", "Humidity", "Precipitation Probability" and "Wind Speed".
+ Extracts the summary of the next 8 days *(including the current day)*, containing "Weather Condition", "Day Name", "Minimum Temperature" and "Maximum Temperature" for each day.
+ Extracts the wind data for the next 15 days with 3 hour intervals, containing "Wind Speed", "Wind Direction", and "Wind Bearing".
+ Extracts a hourly forecast for the next 15 days, containing "Temperature", "Humidity", "Precipitation Probability", "Weather Condition" and "Wind Speed".

## Units

The main function `get_forecast()` accepts an optional `output_units` parameter which has to be a dictionary with the following structure:

+ `temp:`
  + `c` for Celsius
  + `f` for Farenheit
+ `speed:`
  + `mph` for Miles per Hour
  + `km/h` for Kilometers per Hour
