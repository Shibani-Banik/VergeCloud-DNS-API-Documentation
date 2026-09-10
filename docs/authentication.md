# API Authentication

## API keys

VergeCloud's public support documentation describes API keys as the credentials used to authenticate API requests.

The documented request header is:

```http
X-API-Key: <your-api-key>
```

Treat the API key like a password.

## Security guidance

- Do not commit API keys to Git repositories.
- Store keys in environment variables or a secure secret manager.
- Use the least-privilege role required for the automation.
- Revoke a key immediately if it is exposed.
- Generate a new key when access requirements change.

## Roles

VergeCloud's public documentation describes roles including:

- Admin
- Read-Only Admin
- Billing Manager
- Cache Purger
- DNS Manager
- Security Manager
- Traffic Manager
- Insights Analyst

For DNS automation, use the minimum role/scope required for the operation.

> Production note: confirm the exact permission model and role-to-endpoint mapping against the current API documentation.
