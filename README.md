# Weather-Now
Weather Now is a simple React application designed for outdoor enthusiasts like Jamie who want to quickly check current weather conditions for any city. This application uses the Open-Meteo API to provide real-time weather updates.

# Features
Enter a city name to fetch current weather conditions.
Displays:
Temperature (in °C)
Windspeed (in km/h)
Weather code (to describe weather conditions).
Simple and clean user interface.

# Technologies Used
React: For building the user interface.
Axios: For making API requests.
Open-Meteo API: To fetch real-time weather data.
CSS: For styling the application.

# Prerequisites
Before running the application, ensure you have the following installed:
Node.js (v14 or higher)
npm or yarn (comes with Node.js)

# Installation
1. Clone the repository:
    git clone https://github.com/your-repo/weather-now.git
2. Navigate to the project directory:
    cd weather-now
3. Install dependencies:
    npm install
   
# Usage
1. Start the development server:
    npm start
2. Open your browser and navigate to http://localhost:3000.
3. Enter a city name in the input field and click Get Weather to see the current weather conditions.

# Customization
Modify API Integration:
1. Dynamic City Coordinates: Update the application to fetch latitude and longitude for the entered city using a geocoding API (e.g., OpenCage Geocoder or Mapbox).
2. Replace the static coordinates in the Open-Meteo API URL with dynamic ones.
Example:
Replace this line:
  javascript
  `https://api.open-meteo.com/v1/forecast?latitude=52.52&longitude=13.405&current_weather=true`
With:
  javascript
  `https://api.open-meteo.com/v1/forecast?latitude=${latitude}&longitude=${longitude}&current_weather=true`

# File Structure
weather-now/
├── src/
│   ├── App.js         # Main React Component
│   ├── App.css        # Styling for the application
│   ├── index.js       # React DOM entry point
│   └── index.css      # Global styles
├── public/
│   ├── index.html     # Main HTML template
│   └── favicon.ico    # Application favicon
├── package.json       # Project metadata and dependencies
└── README.md          # Documentation

# Future Improvements
1. Integrate a geocoding API for dynamic city-based weather fetching.
2. Display user-friendly weather descriptions (e.g., "Clear Sky" instead of a weather code).
3. Add icons representing weather conditions.
4. Implement autocomplete for city input.
5. Add support for additional weather details like humidity, pressure, etc.

# Contributing
Contributions are welcome! If you have ideas or bug fixes, feel free to open a pull request or an issue in this repository.

# Acknowledgments
1. Open-Meteo API for real-time weather data.
2. Jamie, the outdoor enthusiast, for inspiring the idea!
