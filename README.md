# AETHER Weather + Aether AI

A world weather, time, place, map and directions app with a multilingual Aether AI voice assistant.

## Included
- Worldwide place search with up to 100 matches and exact coordinates.
- Live weather and 7-day forecast from Open-Meteo.
- Celsius/Fahrenheit switch.
- Live local clock for the selected place and its IANA time zone.
- Place details: country, region, coordinates and time zone.
- AETHER map using Leaflet + OpenStreetMap tiles.
- Driving route using OSRM, with distance and estimated duration.
- Voice input and spoken answers through browser speech APIs.
- Multilingual UI/voice selection and script-aware fonts.
- Optional Aether AI backend using an environment variable for the API key.
- PWA files for website installation.
- Capacitor configuration for Android packaging.

## Run website locally
1. Install Node.js.
2. Open this folder in a terminal.
3. Run `npm install`.
4. Run `npm start`.
5. Open `http://localhost:3000`.

## Aether AI backend
Copy `.env.example` to `.env`, then set your server-side AI key. Never put the secret key in `www/app.js` or another public browser file.

## Android
This project is structured for Capacitor. After installing dependencies and the Android development environment, use:
- `npm run android:add`
- `npm run android:sync`
- `npm run android:open`

Then build/sign the Android App Bundle in Android Studio for Play publishing.

## Map/directions notes
The app uses OpenStreetMap/Leaflet for map display and OSRM for the example driving route service. Review the providers' usage policies and attribution requirements before a public commercial launch or high-traffic deployment.

## Data
Open-Meteo geocoding returns latitude, longitude, country, administrative regions and time zone. Weather is requested using the selected coordinates.
