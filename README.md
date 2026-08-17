Authentication

The Weather API uses an API key to authenticate requests. An API key allows the API to identify and authorize your application.

API Key

You must include a valid API key when making requests to the Weather API.

For security reasons, keep your API key private and never share it publicly.

Adding Your API Key

Include your API key as a query parameter in your request.

Example Request

GET /weather?city=Abuja&api_key=YOUR_API_KEY

Replace "YOUR_API_KEY" with your actual API key.

Authentication Errors

If your request is not properly authenticated, the API may return an error.

Common causes include:

- Missing API key
- Invalid API key
- Expired API key
- Incorrect API key format

How to Resolve Authentication Errors

1. Confirm that your API key is correct.
2. Make sure the API key is included in the request.
3. Check that the key has not expired.
4. Make sure there are no unnecessary spaces or characters in the key.

Security Best Practices

Follow these practices to protect your API key:

- Never publish your API key on GitHub.
- Do not share your API key with other people.
- Never include a real API key in screenshots or examples.
- Store API keys securely.
- Replace your key immediately if you believe it has been exposed.

Example of a Safe Request

Use a placeholder instead of a real API key when sharing documentation:

GET /weather?city=Abuja&api_key=YOUR_API_KEY

Next Steps

Continue to the "API Endpoints" (endpoints.md) guide to learn how to retrieve weather information.
