# Adelaide Metro Bus Tracking Application

This is a real-time public bus tracking application for Adelaide Metro, developed using **Node-RED**. The application fetches real-time bus locations, weather data, and air quality information to display on an interactive dashboard.

## Features
- **Real-time Bus Tracking**: Displays live bus locations on a map.
- **Weather Information**: Shows current weather in Adelaide.
- **Air Quality Information**: Displays air quality data (AQI) for Adelaide.
- **Trip Planner**: Plan your bus trips and view estimated arrival times.

## Tech Stack
- **Node-RED**: Visual programming environment for wiring together devices, APIs, and online services.
- **Adelaide Metro API**: Provides real-time bus data for tracking vehicle positions.
- **OpenWeather API**: Fetches real-time weather data.
- **AirVisual API**: Fetches real-time air quality data.
- **Node-RED Dashboard**: Used for building the web-based UI to display bus data and information.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/YOUR_USERNAME/Adelaide-Metro-Bus-Tracking.git
    cd Adelaide-Metro-Bus-Tracking
    ```

2. **Install Node-RED**:
    - If you don’t have Node-RED installed, follow the official installation guide: [Node-RED Install](https://nodered.org/docs/getting-started/).

3. **Install Node-RED Dependencies**:
    - Install the necessary Node-RED nodes by running the following commands in your Node-RED installation folder:
      ```bash
      npm install node-red-dashboard
      npm install node-red-node-axios
      npm install node-red-contrib-leaflet
      ```

4. **Import the Flow**:
    - Open Node-RED’s editor (`http://localhost:1880`).
    - In the **Menu**, click **Import**, then paste the `Final_Code.json` contents into the import window.
    - Click **Import** and **Deploy** the flow.

5. **Set Up API Keys**:
    - Register for the Adelaide Metro API, OpenWeather API, and AirVisual API to get your **API keys**.
    - Replace the placeholder API keys in the flow:
      - Adelaide Metro API key: Replace in the **Get Adelaide Metro GTFS** node.
      - OpenWeather API key: Replace in the **Build Weather API URL** node.
      - AirVisual API key: Replace in the **Build AirVisual API URL** node.

## Usage
1. Start Node-RED and navigate to the **Dashboard** (`http://localhost:1880/ui`).
2. The dashboard will display:
    - A **map** with real-time bus locations.
    - **Weather information** such as temperature and weather conditions.
    - **Air quality information** such as AQI and pollution levels.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
