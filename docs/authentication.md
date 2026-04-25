# Authentication

Namazu API v1 should use a simple managed authentication model.

## Recommended approach

Use a bearer token in the request header:

```http
Authorization: Bearer YOUR_API_KEY
