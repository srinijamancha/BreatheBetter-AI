# BreatheBetter AI

A beginner-friendly air-quality intelligence dashboard built for the Let's Code Diwali Challenge 2026.

## Features
- Current US AQI and pollutant snapshot (PM2.5, PM10, NO2, SO2, CO, O3)
- City search using Open-Meteo Geocoding API
- Click-to-explore interactive map (Leaflet + OpenStreetMap)
- 48-hour model-history charts and 24-hour forecast chart
- Four-city comparison
- General health and activity guidance
- User-set AQI threshold alert while the page is open

## Run locally
1. Download or clone this repository.
2. Open `index.html` in Chrome or Firefox.
3. Keep an internet connection active (the app loads public APIs and libraries from CDNs).

For a local development server, open a terminal in this folder and run:
```bash
python -m http.server 8000
```
Then visit http://localhost:8000

## Data and transparency
- Air quality: Open-Meteo Air Quality API, based on Copernicus Atmosphere Monitoring Service (CAMS).
- Geocoding: Open-Meteo Geocoding API.
- Map tiles: OpenStreetMap contributors.
- The API returns gridded model output, not necessarily a nearby physical monitoring-station observation. Values may differ from official regulatory station readings.
- The dashboard labels hourly past data as model history and future values as forecasts.
- AQI categories use the US AQI scale returned by Open-Meteo.
- Health guidance is general information, not medical advice.

## API references
- https://open-meteo.com/en/docs/air-quality-api
- https://open-meteo.com/en/docs/geocoding-api
- https://www.openstreetmap.org/copyright

## Important
This is a front-end prototype. Threshold alerts are checked while the page is open; they are not background push notifications. Comparison locations are approximate model-grid comparisons, not official rankings of monitoring stations.
