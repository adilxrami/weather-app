# Weather App

This is a simple weather app that fetches current weather and 5-day forecast data from the OpenWeatherMap API and displays it in an easy-to-read format. The app provides real-time weather information based on a city input by the user, including temperature, weather description, and a weather icon. Additionally, the background image dynamically changes based on the current weather conditions to enhance the visual experience.

## Features
- **Current Weather**: Displays the current temperature, weather description, and an icon representing the current weather condition.
- **5-Day Forecast**: Shows a 5-day weather forecast, with temperature and weather icons for each day.
- **Dynamic Background**: The app changes the background image depending on the weather condition (e.g., clear, cloudy, rainy, snowy) to provide a more immersive experience.
- **City Search**: Users can input the name of any city to get the weather details for that location.

## How It Works
- The app makes API requests to OpenWeatherMap for both the current weather and 5-day forecast using the city name entered by the user.
- The current weather data includes temperature, weather description, and an icon, which is displayed on the app's interface.
- A dynamic background is set based on the main weather condition (clear, clouds, rain, snow).
- The 5-day forecast is presented by displaying temperature and weather icons for each day, using 3-hour intervals from the API response.
- The user can interactively update the weather information by entering a new city.

## Installation & Usage
1. Get your own API key from [OpenWeatherMap](https://openweathermap.org/api).
2. Replace the placeholder API key (`'YOUR-API-KEY-HERE'`) in the script with your actual API key.
3. Open the `index.html` file in your browser.
4. Enter a city name and click the search button to view the current weather and forecast for that city.

## Example API Call
- Current weather: `https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY}&units=metric`
- 5-Day forecast: `https://api.openweathermap.org/data/2.5/forecast?q={city}&appid={API_KEY}&units=metric`

## Notes
- The app uses async/await syntax to handle API requests.
- The background image URLs are sourced from external image repositories.
