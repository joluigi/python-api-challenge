# python-api-challenge

## WeatherPY task 
Description:

This task aims to get weather data from a number of random cities auto-generated with the aid of Citipy library.
The weather data will be extracted from <a href="https://openweathermap.org/api">OpenWeather API</a>

Data variables to extract:
<ul>
  <li>City latitude</li>
  <li>City longitude</li>
  <li>Max Temperature</li>
  <li>Humidity</li>
  <li>Cloudiness</li>
  <li>Wind speed</li>
  <li>Country</li>
  <li>Date</li>
</ul>

Special considerations
<ul>
  <li>The data extracted is displayed in metric system</li>
  <li>WeatherPy folder includes the generated CSV to use in VacationPy</li>
</ul>

## VacationPY task

Description:

From the dataframe extracted in CSV format from WeatherPY there is an analysis that plots with a heatmap the humidity of all cities.
The used map was obtained from <a href="https://jupyter-gmaps.readthedocs.io/en/latest/index.html">gmaps library</a> and helped to display the results.
Also, there was a filtering of cities based on ideal weather conditions that were selected arbitrarily. This was the criteria:

<ul>
  <li>Humidity between 45% - 60%</li>
  <li>Temperature between 25° and 32° celsius</li>
  <li>Cloudiness between 0% and 40%</li>
</ul>

After selecting the weather conditions, using API of <a href="https://developers.google.com/places/web-service/search">Google places</a> nearby hotels from coordinates of cities with ideal weather conditions were extracted and plotted in the heatmap mentioned before.

Special considerations
<ul>
  <li>The data extracted is displayed in metric system as in WeatherPy</li>
  <li>Some responses from the Google API were different from each one. As a result a Try/except function was applied to continue with the search and to ignore if there were no hotels found </li>
</ul>
