# Add a DNS Record

## Purpose

Use this workflow when you need to add a DNS record to a VergeCloud-managed domain.

## Before you begin

You need:

- Access to the VergeCloud account
- A domain managed through VergeCloud DNS
- The record type and required values
- Appropriate API permissions

## Workflow

1. Select the DNS record type.
2. Identify the root domain or subdomain.
3. Enter the fields required for that record type.
4. Set the TTL where supported.
5. Save the record.
6. Verify DNS resolution.

## Example: A record

```text
Type: A
Name: @
IP address: 192.0.2.1
TTL: 120
```

The IP address above is an example documentation value.

## Verify

```bash
dig A example.com
```

Check the answer section to confirm the expected record is returned.

## Production API note

The exact `POST` endpoint, request schema and response schema must be taken from the current VergeCloud OpenAPI specification before publishing an API reference example.
