# Authentication

The Weather API uses an API key to authenticate requests.

## API Key

An API key is a unique identifier that allows the API to verify your request.

Keep your API key private and do not share it publicly.

## Including Your API Key

Add your API key to the request header:

    Authorization: Bearer YOUR_API_KEY

Replace `YOUR_API_KEY` with your actual API key.

## Example

    GET /weather?city=Abuja

    Authorization: Bearer YOUR_API_KEY

## Security Best Practices

- Never share your API key publicly.
- Do not commit API keys to GitHub.
- Store API keys securely.
- If your key is exposed, replace it immediately.

## Common Authentication Error

If the API returns an authentication error, check that:

1. Your API key is correct.
2. Your API key has not expired.
3. The authorization header is included correctly.

Once you've entered it, **commit the file**.

Then send me the screenshot like you did with `getting-started.md`, and we'll move to **`endpoints.md`**.
