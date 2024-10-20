
# Real-Time Weather Monitoring Application

## Project Overview

This project is a real-time weather monitoring application that retrieves weather data for any city using the OpenWeatherMap API. The application allows users to search for weather information by entering a city name and provides real-time weather conditions, such as temperature, perceived temperature, and weather description.

[Live Project Link](https://weather-app-resu.vercel.app/)  
[GitHub Repository](https://github.com/DHANUNJAY965/weather-Application.git)

## Features

- Search for real-time weather data for any city globally
- Displays key weather data, including:
  - Main weather condition (e.g., Rain, Clear, Snow)
  - Temperature in Celsius
  - Feels like temperature in Celsius
  - Weather description
  - Time of data retrieval (Unix timestamp)
- Simple and user-friendly interface

---

## Project Setup

### Option 1: Using Docker (Recommended)

1. Install Docker and Docker Compose on your system.

2. Clone the repository:
   ```bash
   git clone https://github.com/DHANUNJAY965/weather-Application.git
   cd weather-Application
   ```

3. Build and run the Docker containers:
   ```bash
   docker-compose up --build
   ```

4. The application will be available at [http://localhost:3000](http://localhost:3000).

---

### Option 2: Manual Setup

1. Install Node.js (v14 or later) on your system.

2. Clone the repository:
   ```bash
   git clone https://github.com/DHANUNJAY965/weather-Application.git
   cd weather-Application
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Run the development server:
   ```bash
   npm run dev
   ```

5. The application will be available at [http://localhost:3000](http://localhost:3000).

---

## Using the Application

1. Open your browser and navigate to [http://localhost:3000](http://localhost:3000).

2. In the search bar, enter the name of any city to retrieve real-time weather data for that location.

3. The application will display:
   - Main weather condition (e.g., Rain, Clear, Snow)
   - Current temperature (in Celsius)
   - Feels like temperature (in Celsius)
   - Weather description
   - Time of the data retrieval

---

## OpenWeatherMap API

The application uses the OpenWeatherMap API to retrieve real-time weather data. To run the project, you'll need to:

1. Sign up for a free API key from OpenWeatherMap [here](https://openweathermap.org/).
2. Add the API key to the environment variables as follows:
   ```bash
   NEXT_PUBLIC_OPENWEATHER_API_KEY=your_api_key
   ```

---

## Docker Setup

A `Dockerfile` and `docker-compose.yml` are included to run the application in a containerized environment.

1. **Dockerfile**: Defines the Node.js environment and serves the Next.js application.

2. **docker-compose.yml**: Builds the application container and starts the service.

### Running Docker

To build and run the application using Docker, follow these steps:

```bash
docker-compose up --build
```

The application will be available at [http://localhost:3000](http://localhost:3000).

---

## Troubleshooting

1. **Search not returning results**: 
   - Ensure the OpenWeatherMap API key is valid.
   - Verify internet connectivity.
   - Ensure the city name is spelled correctly.

2. **Docker containers not starting**: 
   - Ensure Docker is installed and running.
   - Check the `docker-compose.yml` configuration for errors.

---

For any further issues or questions, please feel free to open an issue on the [GitHub repository](https://github.com/DHANUNJAY965/weather-Application.git).
