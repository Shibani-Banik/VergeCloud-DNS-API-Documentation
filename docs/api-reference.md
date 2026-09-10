# DNS API Reference

> **Important:** The operation below is the one for which the public VergeCloud support content exposes the endpoint path. Other endpoint paths in the public support material are described functionally but are not reproduced here without verification against the current OpenAPI specification.

## Update the Cloud setting for a DNS record

### Endpoint

```http
PUT /v1/dns/{domain}/records/{id}/cloud
```

This path is derived from the endpoint linked in VergeCloud's public Cloud-option documentation.

### Purpose

Updates the Cloud setting for a specific DNS record. The Cloud option controls whether CDN/security features are enabled for the record.

### Path parameters

| Parameter | Type | Required | Description |
|---|---|---|---|
| `domain` | string | Yes | VergeCloud-managed domain |
| `id` | string | Yes | DNS record identifier |

### Authentication

```http
X-API-Key: <your-api-key>
```

### Request body

The exact production request schema should be taken from the current OpenAPI specification.

Illustrative example only:

```json
{
  "cloud": true
}
```

### Verification

After enabling the Cloud option, verify DNS behavior with a DNS lookup and confirm that the record points to the expected VergeCloud CDN configuration.

### Related workflow

```text
DNS record exists
      |
      v
Update Cloud setting
      |
      v
Verify DNS resolution
      |
      v
Verify CDN/security behavior
```

## Production documentation checklist

Before publishing this reference page, validate:

- HTTP method
- Base URL
- Authentication requirements
- Path parameters
- Request schema
- Response schema
- Success status code
- Error status codes
- Rate limits
- Idempotency behavior
- Permissions/roles
- Example response
- Error examples
