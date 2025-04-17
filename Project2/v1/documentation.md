# API Test Documentation

This is a comprehensive test file to demonstrate how markdown renders in our documentation system.

## Introduction

Welcome to our API documentation. This markdown file showcases various features that you can use when writing your documentation.

### Key Features

Our API offers the following features:

* **Authentication** - Secure access to resources
* **Rate Limiting** - Protection against abuse
* **JSON Responses** - Standardized data format
* **Comprehensive Documentation** - What you're reading now!

## Getting Started

To get started with our API, follow these steps:

1. [Register for an API key](authentication)
2. Set up authentication in your client
3. Make your first request
4. Handle the response

## Code Examples

Here's how to make a request using cURL:

```bash
curl -X GET "https://api.example.com/v1/resources" \
     -H "Authorization: Bearer YOUR_API_KEY" \
     -H "Content-Type: application/json"
```

And here's an example response:

```json
{
  "data": [
    {
      "id": 1,
      "name": "Example Resource",
      "status": "active"
    },
    {
      "id": 2,
      "name": "Another Resource",
      "status": "pending"
    }
  ],
  "meta": {
    "total": 2,
    "page": 1,
    "per_page": 10
  }
}
```

## API References

You can find detailed information about our endpoints here:

- [API:openapi] - Main API specification
- [API:users] - User management endpoints
- [API:billing] - Billing and subscription endpoints

> **Note**: Replace "openapi", "users", and "billing" with the actual names of your JSON files (without the .json extension).

## Error Handling

| HTTP Status | Error Code | Description |
|-------------|------------|-------------|
| 400 | BAD_REQUEST | The request was malformed |
| 401 | UNAUTHORIZED | Authentication failed |
| 403 | FORBIDDEN | Insufficient permissions |
| 404 | NOT_FOUND | Resource not found |
| 429 | TOO_MANY_REQUESTS | Rate limit exceeded |
| 500 | SERVER_ERROR | Internal server error |

## Advanced Topics

For more detailed information, check out these additional resources:

- [Authentication Guide](authentication)
- [Pagination and Filtering](examples#pagination)
- [Webhook Integration](webhooks)

---

## FAQ

### How do I reset my API key?

Contact support to have your API key reset.

### Is there a rate limit?

Yes, the default rate limit is 100 requests per minute.

### Can I use the API in a mobile app?

Yes, but never embed your API key directly in the app. Use a server-side component to make API calls.

---

*Last updated: April 2025*