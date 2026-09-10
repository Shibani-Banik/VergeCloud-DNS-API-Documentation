# VergeCloud DNS API

## What is the DNS API?

The VergeCloud DNS API enables programmatic management of DNS resources. Public VergeCloud documentation states that the DNS API supports creating, updating, deleting and retrieving DNS records, as well as managing DNS security and cloud status.

Use the API when DNS changes need to be integrated into automation, deployment workflows or infrastructure-management processes.

## Typical workflow

```text
Create API key
      |
      v
Authenticate request
      |
      v
Select domain
      |
      v
Create / update / delete / retrieve record
      |
      v
Verify DNS resolution
```

## Supported DNS record examples

VergeCloud's public DNS documentation covers:

- A
- AAAA
- CNAME
- ANAME
- TXT
- MX
- NS
- SRV
- PTR
- CAA
- TLSA

Each record type has different fields and validation requirements.

## Example use case

A DevOps team wants to automate DNS changes during an application deployment.

Instead of logging into the dashboard manually, the deployment process can call the DNS API to create or update a record and then verify the result with a DNS lookup.

## Source validation

Before production publication, confirm all endpoint paths, request schemas, response schemas, authentication requirements and status codes against the current VergeCloud OpenAPI specification.
