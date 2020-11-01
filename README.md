# python-api-challenge
tracking weather using Python API
Hello Again, World.
This repository contains my work on a project investigating weather around the world.
There are two jupyter notebooks: TM_WeatherPy and TM_VacationPy.

In TM_WeatherPy, I take a look at 500+ randomly selected cities around the world and 
using an OpenWeather API, retrieve weather related information about that location.  
Pandas is used to gather all of this weather information and make comparisons while
MatPlotLib is used to create several plots showing any relationships I was able to find.
My code includes a significant time delay to keep from exceeding OpenWeather's maximum 
calls per minute, so be warned.
Observations: 
1. In looking at this data, I found a strong correlation between Latitude
and Maximum Temperate, which is, of course, to be expected.
2. I did not find statistically significant correlations between Latitude and Humidity,
Latitude and Cloudiness or between Latitude and Windspeed. 
3. Also, the correlation between Latitude and Maximum Temperature was stronger in the 
Northern Hemisphere than in the Southern Hemiphere.  This raises questions as to why
this is the case?  Does it have something to do with the cities that were randomly selected?
Were there more Northern Hemisphere cities selected than Southern Hemisphere cities?

In TM_VacationPy, I take those same randomly selected cities and whittle them down to two 
handfuls using certain favorable weather conditions, namely low Windspeed, high Temperature
and little Cloudiness.  I use Google API to find and plot hotels in these favorable weather
conditioned cities and display them on markers on the world map.
