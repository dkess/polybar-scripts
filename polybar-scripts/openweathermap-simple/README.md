# Script: openweathermap-simple

A weather script that displays some weather information.

It shows icons and temperatures for the current weather. The script can be easily modified to display a forecast. Look at the commented out line.

Change these values:
```
KEY=""
CITY=""
UNITS="metric"
SYMBOL="°"
```


## Dependencies

* [OpenWeatherMap-Key](https://openweathermap.org/appid)
* [weather-icons](https://github.com/erikflowers/weather-icons)
* `jq`


## Module

```
[bar/polybar]
...
font-2 = Weather Icons:size=12;1
...


[module/openweathermap-simple]
type = custom/script
exec = ~/polybar-scripts/openweathermap-simple.sh
interval = 600
label-font = 3
```
