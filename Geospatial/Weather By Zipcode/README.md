Weather by Zip Code

A simple Python script that retrieves the current weather for a given U.S. ZIP code using the OpenWeatherMap API.

Features

Fetches current weather conditions (temperature, humidity, description) for a ZIP code.

Gracefully handles API key activation wait times.

Minimal dependencies: requests and python-dotenv.

Prerequisites

Python 3.8 or higher

A free API key from OpenWeatherMap (https://openweathermap.org/)

Installation

Clone the repository:

git clone https://github.com/Aeronique/weather-by-zip.git
cd weather-by-zip

Create and activate a virtual environment:

python3 -m venv venv
source venv/bin/activate    # macOS/Linux
# .\venv\Scripts\Activate.ps1  # Windows PowerShell

Install dependencies:

pip install requests python-dotenv

Configure your API key:

Create a file named .env in the project root.

Add the following line, replacing YOUR_API_KEY with your actual key:

OPENWEATHER_API_KEY=YOUR_API_KEY

Usage

Run the script:

python3 weather_by_zip.py

When prompted, enter a U.S. ZIP code (e.g., 10001).

Example output:

Enter ZIP code (e.g. 10001): 90210

Current weather in Beverly Hills:
  Conditions: Clear Sky
  Temperature: 75.2°F (feels like 74.5°F)
  Humidity: 45%

Troubleshooting

401 Unauthorized: If you see a message about the API key not being active, wait a few hours for OpenWeatherMap to propagate the key.

Environment variable issue: Ensure .env is in the project root and contains the correct key. Activate your virtual environment before running the script.

Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

License

This project is licensed under the MIT License.

