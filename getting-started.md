Getting Started

This guide explains how to make your first request to the Weather API.

Prerequisites

Before using the API, make sure you have:

- An API key
- An internet connection
- A tool for sending HTTP requests

Base URL

All API requests are sent to:

https://api.example.com/v1

Make Your First Request

To retrieve weather information for a city, send a "GET" request to the "/weather" endpoint.

Example Request

GET /weather?city=Abuja&api_key=YOUR_API_KEY

Replace "YOUR_API_KEY" with your actual API key.

Example Response

A successful request returns weather information in JSON format:

{
  "city": "Abuja",
  "temperature": 28,
  "humidity": 65,
  "description": "Partly cloudy"
}

Understanding the Response

Field| Description
"city"| The name of the requested city.
"temperature"| The current temperature.
"humidity"| The current humidity percentage.
"description"| A short description of the current weather.

Common Issues

If your request does not work:

1. Check that your API key is correct.
2. Make sure the city name is spelled correctly.
3. Check your internet connection.
4. Confirm that the request URL is correct.

Next Steps

Now that you know how to make a basic request, continue to the "Authentication" (authentication.md) guide to learn more about API authentication.
