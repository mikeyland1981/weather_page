# Weather Station

Responsive local weather dashboard with barometric pressure trends and a seven-day forecast.

## Features
- Current temperature, feels-like, sky conditions, daily highs/lows, sunrise and sunset
- Barometric pressure (inHg or hPa), three-hour trend, and selectable 24-hour, 3-day, and 7-day historical pressure charts using modeled hourly estimates
- Humidity, wind, gusts, UV index, dew point, visibility, precipitation, cloud cover and surface pressure
- Next-24-hour temperature chart and seven-day forecast
- City search, location and unit preferences saved in the browser
- Responsive layout with no build tools, API keys or paid dependencies

The dashboard defaults to **Lancaster, Kentucky**, and uses the [Open-Meteo forecast API](https://open-meteo.com/en/docs) and [geocoding API](https://open-meteo.com/en/docs/geocoding-api).

**Important:** Forecast values and historical estimates are modeled weather data, not readings from a physical weather station. This is not a severe-weather warning system. Open-Meteo's free tier has [terms and noncommercial usage restrictions](https://open-meteo.com/en/terms).

## Run locally
Serve this repository using a simple HTTP server:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Publish free with GitHub Pages
After merging the pull request into `main`, open **Settings → Pages → Build and deployment**. Choose **Deploy from a branch**, branch **main**, folder **/(root)**, then save. The published address should be:

https://mikeyland1981.github.io/weather_page/

## Files
- `index.html`: Dashboard markup
- `styles.css`: Layout and visual design
- `app.js`: API calls, charts, unit conversion, rendering and city search

Weather data courtesy of [Open-Meteo](https://open-meteo.com/).