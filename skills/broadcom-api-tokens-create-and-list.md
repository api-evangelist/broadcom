---
name: broadcom-api-tokens-create-and-list
description: Create a new API token and then list all API tokens.
api: openapi/broadcom-api-tokens-api-openapi.yml
operations:
- createApiToken
- listApiTokens
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/broadcom-api-tokens-api-openapi.yml ; every operationId checked against the contract
---

# broadcom-api-tokens-create-and-list

Create a new API token and then list all API tokens.

## Steps

1. 1. Call `createApiToken` with the required request body fields as defined in the contract.
2. 2. Call `listApiToken` with optional query parameters `page` and `limit` as defined in the contract.

## Rules

- Authentication must be provided using one of the supported schemes: basicAuth (HTTP Basic), bearerAuth (Bearer token), or sessionAuth (API key in header `vmware-api-session-id`).
- Pagination parameters `page` and `limit` can be used with `listApiToken` to control result sets.
