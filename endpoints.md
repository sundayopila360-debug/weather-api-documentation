# API Endpoints

This guide explains the main endpoints available in the Weather API.

## Get Weather

Use this endpoint to retrieve weather information for a specific city.

### Request

GET /weather?city=Abuja&api_key=YOUR_API_KEY

### Parameters

- `city` — The name of the city.
- `api_key` — Your API authentication key.

### Example

GET /weather?city=Abuja&api_key=YOUR_API_KEY

### Example Response

{
  "city": "Abuja",
  "temperature": 28,
  "humidity": 65,
  "description": "Partly cloudy"
}

## Response Fields

| Field | Type | Description |
|---|---|---|
| city | string | Name of the city |
| temperature | number | Current temperature |
| humidity | number | Current humidity percentage |
| description | string | Brief weather description |

## Error Responses

The API may return an error when a request is invalid.

Common errors include:

- `400 Bad Request` — Invalid or missing parameters.
- `401 Unauthorized` — Invalid or missing API key.
- `404 Not Found` — City or endpoint not found.
- `500 Internal Server Error` — Server-side problem.

## Next Steps

Continue to the Troubleshooting guide for solutions to common API problems.
