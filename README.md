# Smartwatch - Gif Weather App

Project completed together with [Joey Scott](https://github.com/joeylouise), [Lucy Sabin](https://github.com/lucyrose93) and [Zooey Miller](https://github.com/ZooeyMiller)

## Introduction

- The location is based on user's IP address.
- Weather is based on user's location.
- Gif is based on weather description.

### APIs used

- [Nekudo](http://geoip.nekudo.com/) (geolocation)

  *This API gets location information for IP addresses.*

  We get the user's __latitude__ and __longitude__ from this API.

- [OpenWeather](https://openweathermap.org/api)

  *This API gets current weather data for one location.*

  We use __latitude__ and __longitude__ from the Nekudo API to call the OpenWeatherMap API, to get weather information for the user's location (based on IP address).

  We get __city__, __temperature__, __weather description__ and __weather summary__ from this API.

  We use __city__, __summary__ and __temperature__ to update the DOM, in order to show the user the this information.

- [Giphy](https://api.giphy.com/)

  *This API gets gifs.*

  We use __weather description__ from the OpenWeatherMap API to call the Giphy API, in order to return gifs that relate to the description of the weather.


### Architecture

![Waterfall graph](demo/waterfall-graph.png)
