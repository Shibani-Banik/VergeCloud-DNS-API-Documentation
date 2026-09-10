# Quick Start

## 1. Create an API key

Create an API key in the VergeCloud dashboard and assign the minimum required permissions.

The key is shown during creation and should be stored securely.

## 2. Set the API key

Example:

```bash
export VERGECLOUD_API_KEY="YOUR_API_KEY"
```

Do not place a real key in source code or commit it to Git.

## 3. Make an authenticated request

The authentication header documented by VergeCloud is:

```http
X-API-Key: <your-api-key>
```

A production request should use the exact endpoint and base URL provided by the current VergeCloud API specification.

## 4. Verify the result

For DNS changes, use a DNS lookup such as:

```bash
dig A example.com
```

or the appropriate record type.

VergeCloud's public DNS documentation uses `dig` examples to verify DNS resolution after record changes.
