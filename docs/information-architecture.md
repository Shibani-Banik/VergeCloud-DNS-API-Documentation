# Information Architecture

## User-intent model

The documentation is intentionally organized around the developer journey.

```text
UNDERSTAND
   |
   +--> What is the DNS API?
   |
AUTHENTICATE
   |
   +--> How do I create and use an API key?
   |
DO
   |
   +--> How do I add/update/delete a DNS record?
   |
REFERENCE
   |
   +--> What parameters and responses are available?
   |
VERIFY
   |
   +--> How do I confirm the DNS change?
   |
TROUBLESHOOT
   |
   +--> What should I check when something fails?
```

## Content model

- Concept: explains what/why.
- Task: explains how.
- Reference: provides precise technical facts.
- Map: assembles the topics into a coherent deliverable.

## Content-quality checks

Before release:

1. Validate technical facts against the API specification.
2. Test examples in a safe test environment.
3. Check terminology.
4. Check authentication/security guidance.
5. Check links and code samples.
6. Review with Engineering/SME.
7. Check accessibility and readability.
