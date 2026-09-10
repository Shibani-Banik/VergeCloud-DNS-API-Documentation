# Troubleshooting

## DNS change is not visible

DNS propagation can take time. Verify the authoritative response and check the record with `dig`.

```bash
dig A example.com
```

## API authentication fails

Check:

- The `X-API-Key` header is present.
- The key has not been revoked.
- The key has the required role.
- The request is sent to the correct API endpoint.

## Cloud option does not behave as expected

Confirm:

- The DNS record exists.
- The Cloud setting was updated successfully.
- The record points to the expected VergeCloud configuration.
- The DNS response is correct.
- CDN/security behavior is being tested after DNS changes have propagated.

## Documentation escalation

If API behavior differs from the published specification, capture:

- endpoint
- request
- response
- timestamp
- error/status code
- environment

Then validate the behavior with Engineering/API owners before changing the documentation.
