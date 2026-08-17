API Endpoints

This guide explains how to use the Weather API endpoint to retrieve weather information for a specific city.

Get Current Weather

Use the "/weather" endpoint to retrieve the current weather conditions for a city.

Request

Method: "GET"

Endpoint:

/weather

Example Request

GET /weather?city=Abuja&api_key=YOUR_API_KEY

Request Parameters

Parameter| Type| Required| Description
"city"| string| Yes| The name of the city.
"api_key"| string| Yes| Your API authentication key.

Example

To retrieve the weather for Abuja:

GET /weather?city=Abuja&api_key=YOUR_API_KEY

Example Response

A successful request returns a JSON response:

{
  "city": "Abuja",
  "temperature": 28,
  "humidity": 65,
  "description": "Partly cloudy"
}

Response Fields

Field| Type| Description
"city"| string| Name of the requested city.
"temperature"| number| Current temperature.
"humidity"| number| Current humidity percentage.
"description"| string| Description of the current weather conditions.

Error Responses

The API may return an error when a request cannot be completed.

Status Code| Meaning| Possible Cause
"400"| Bad Request| Missing or invalid parameter.
"401"| Unauthorized| Missing or invalid API key.
"404"| Not Found| Requested city or resource was not found.
"500"| Server Error| Temporary problem with the API server.

Next Steps

If you encounter an error while using the endpoint, see the "Troubleshooting" (troubleshooting.md) guide for possible solutions.
