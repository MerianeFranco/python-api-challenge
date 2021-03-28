# Python API Homework - Meriane Franco


## Part I - WeatherPy

A Python script was created to visualize the weather of 500+ cities across the world of varying distance from the equator. 
In a random search in [simple Python library](https://pypi.python.org/pypi/citipy), 615 cities where found,
but the weather data of some of them where not available on the [OpenWeatherMap API](https://openweathermap.org/api).
A file called "weather.csv" lists the weather of 565 cities and a file called "summary.csv" gives a summary statistic of those cities.

Looking at the data, I could observe the trending below:
1 - Cities with latitude -40 to -60 in the Southern Hemisphere are way warmer than cities with Latitude 40 to 60 in the Northern Hemisphere.
2 - In both Hemispheres, the linear regression did not show an influence of Latitude and Cloudiness. Both r-values are low (0.11 and 0.04)
3 - The relationship between maximum temperature and latitude is closer in the Northern than in Southern Hemisphere. The higher r-value (0.77) in the North, compared to the r-value in the South (0.40) indicates this condition.



### Part II - VacationPy

The weather information from the cities in Part I was used to create a heatmap that displays the humidity for every city using Jupyter-gmaps and the Google Places API.

The conditions below were used to select cities for vacation.
 * A max temperature lower than 100 degrees but higher than 80.
 * Wind speeds up to 15 mph.
 * Humidity from 40% to 65%


The cordinates of each city were used to get the first hotel name result in Google Places API in a radius of 5000 meters.

A mark was added to each city in a heat map with a hotel.

