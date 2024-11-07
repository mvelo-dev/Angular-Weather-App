# Angular Weather App

This Angular Weather App allows users to view real-time weather information for various cities around the world. The app is built using Angular for the frontend and leverages a Node.js backend to fetch weather data from an external weather API.

## Table of Contents

1. [Features](#features)
2. [Technologies](#technologies)
3. [Setup](#setup)
4. [Usage](#usage)
5. [API Endpoints](#api-endpoints)
6. [Contributing](#contributing)
7. [License](#license)

---

## Features

- **Real-Time Weather Data**: Displays current temperature, humidity, and weather conditions for selected locations.
- **Search Functionality**: Allows users to search for any city and view its weather details.
- **Responsive UI**: Adapts to both desktop and mobile screen sizes.
- **Error Handling**: Displays error messages for invalid city names or when the API fails to fetch data.

## Technologies

- **Frontend**: Angular
- **Backend**: Node.js with Express
- **API**: [OpenWeatherMap API](https://openweathermap.org/api) (or any similar weather API)

## Setup

### Prerequisites

- **Node.js** (version 14 or higher)
- **Angular CLI** (version 12 or higher)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/angular-weather-app.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd angular-weather-app
   ```

3. Install dependencies for the Angular frontend:
   ```bash
   cd client
   npm install
   ```

4. Install dependencies for the Node.js backend:
   ```bash
   cd ../server
   npm install
   ```

### Environment Variables

1. In the `server` directory, create a `.env` file to store your API key for the weather service:
   ```env
   WEATHER_API_KEY=your_weather_api_key
   PORT=5000
   ```

### Running the Application

1. Start the Node.js server:
   ```bash
   cd server
   npm start
   ```

2. In a separate terminal, start the Angular frontend:
   ```bash
   cd client
   ng serve
   ```

3. Open the app in your browser at `http://localhost:4200`.

## Usage

1. Open the application and enter the name of a city in the search bar.
2. View the real-time weather information for the selected location, including temperature, humidity, and weather description.

## API Endpoints

The Node.js backend is structured to provide weather data via a simple API endpoint:

- **GET `/api/weather?city={cityName}`**: Fetches weather information for a given city name.

Example response:
```json
{
  "city": "New York",
  "temperature": "15°C",
  "humidity": "80%",
  "description": "Clear sky"
}
```

## Contributing

Contributions are welcome! Please fork the repository and make changes as you'd like, or open an issue to discuss any ideas or bugs.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
