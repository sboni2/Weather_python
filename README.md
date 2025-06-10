## ☁️ Weather App

A simple **command-line Python tool** that fetches and displays real-time weather information for a user-specified location—using the OpenWeatherMap API.

### 🌟 Features

* **API Request**: Retrieves current weather data via HTTP requests using Python's `requests` library
* **Real-time feedback**: Displays:

  * Main weather condition (e.g., Clear, Clouds, Rain)
  * Temperature in Celsius
  * Humidity percentage
* **User-friendly output**: Prints clean and informative messages based on API responses

### 🔑 Key Concepts & Learning Goals

1. **API Integration**
   Connect to OpenWeatherMap with an API key passed through environment variables (`os.getenv`).

2. **JSON Parsing**
   Extract JSON data (temperature, humidity, weather description) from API responses ([realpython.com][1], [medium.com][2], [beapython.dev][3]).

3. **Error & Status Handling**

   * Check `status_code == 200` to confirm valid cities
   * Inform user when a city is not found (404) or any request errors occur
     ([medium.com][2])

4. **Clean CLI Experience**
   Prompt the user for input, then present readable, well-formatted weather output.

---

### ✅ Why This Project Matters

* **Practical API use**: Demonstrates how to safely store and use API keys.
* **Robust programming practices**: Handles different HTTP responses and user scenarios gracefully.
* **Immediate utility**: A neat tool that delivers real-time, useful output for any location.
* **Ideal for beginners**: Builds familiarity with `requests`, `json`, and error handling in a useful, real-world context.

---

### ⚙️ Quick Start

1. Set your OpenWeatherMap API key:

   ```bash
   export weatherapp_api="YOUR_API_KEY"
   ```
2. Run the script:

   ```bash
   python weather_app.py
   ```
3. Input a city when prompted, and get instant weather details!

