# Google Weather Forecast Scraper

Simple BeautifulSoup scraper for Google weather forecast data, including hourly precipitation probability and wind forecast for a week (hourly temperatures are planed to be implemented).

It also has automatic units detection and conversion (hourly forecasts still don't have this feature)

## Units

The main function `get_google_forecast()` accepts an optional `output_units` parameter which has to be a dictionary with the following structure:

+ `temp:`
    + `c` for Celsius
    + `f` for Farenheit
+ `speed:`
    + `mph` for Miles per Hour
    + `kph` for Kilometers per Hour

### Note

Depending on your locale/language, you might need to change the regex at the end of the main function, currently it works for English and Portuguese, other languages may also work, but it has not been tested.
