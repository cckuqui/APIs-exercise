# Python API Exercise - Weather

We all know that if we get closer to the equator the temperature gets higher, but can you prove it? This exercise focuses on it.

![Image retrived from OpenWeatherMap page](https://openweathermap.org/themes/openweathermap/assets/img/new-history-forecast-bulk.png)

## Data

For this example, I generated random latitudes and longitudes varing from +/-90 case of latitude and +/-180 for longitude. From it, using citypy, I detected the nearest city and generated a city list. This list was use to locate the weather information from the OpenWeatherMap API, to create a representative model of weather across world [cities](Resources/cities.csv).

![Preview of the latest file created](Images/prev_cities.png)

### Objective

Analize the information retrived with visual help from `matplotlib`.

* Temperature (C) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Divide by Hemispheres and review the same information as before, looking for correlation between the data.

Create a heatmap with the aid of `gmaps` with the humidity for the cities. Identifing an ideal weather, find the nearest hotel to the cities that have the ideal weather conditions.
Create an ideal weather and 

## Results

* General visualizations

  * Temperature (C) vs. Latitude

    ![Max Temperature vs. Latitude](Images/max_temp.png)

    In this plot we can see that as we get away from the Equator the max temperature decreses, but we see a more significant decrease in the north of the planet.

  * Humidity (%) vs. Latitude

    ![Humidity vs. Latitude](Images/humidity.png)

    As far as this chart shows, there is no relation between the latitude and the % humidity.

  * Cloudiness (%) vs. Latitude

    ![Cloudiness vs. Latitude](Images/clouds.png)

    Again, it appears as it there is no relation between the latitude and the % cloudiness.

  * Wind Speed (mph) vs. Latitude

    ![Wind Speed vs. Latitude](Images/wind_speed.png)

    In here also, there is no relation between the latitude and the wind speed.

* By Hemispher

  * Temperature (C) vs. Latitude

    ![Southern Hemispher Max Temperature vs. Latitude](Images/south-max_temp.png) ![Northen Hemispher Max Temperature vs. Latitude](Images/north-max_temp.png)

    As we stated before, the temperatures drop as we get away from the Equator more pronounce in the northern hemisphere, probably due earth oval shape.

  * Humidity (%) vs. Latitude

    ![Southern Hemispher Humidity vs. Latitude](Images/south-humidity.png) ![Northen Hemispher Humidity vs. Latitude](Images/north-humidity.png)

    The behaviour in both hemispheres are similar (mirroring), both with a +- 0.5 slope.

  * Cloudiness (%) vs. Latitude

    ![Southern Hemispher Cloudiness vs. Latitude](Images/south-clouds.png) ![Northen Hemispher Cloudiness vs. Latitude](Images/north-clouds.png)

    There seems to be a higher correlation between the southern hemisphere than in the northern hemisphere. And is notorious that both hemisphere behave similar instead of in a mirroring way as would be standard.

  * Wind Speed (mph) vs. Latitude

    ![Southern Hemispher Wind Speed vs. Latitude](Images/south-wind_speed.png) ![Northen Hemispher Wind Speed vs. Latitude](Images/north-wind_speed.png)

    There seems to be no significant correlation between the latitude and the wind speed.

* HeatMap with `gmaps`

  ![HeatMap with % humidity](Images/heatmap.png)

* Map with hotesl for the cities with ideal weather.

  ![Map with % humidity and hotels](Images/hotelmap.png)

### Copyright

Trilogy Education Services © 2019. All Rights Reserved. First image retrived from OpenWeatherMap site on 07/08/2020.
