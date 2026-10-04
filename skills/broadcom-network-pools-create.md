---
name: broadcom-network-pools-create
description: Create a new network pool after optionally listing existing pools.
api: openapi/broadcom-network-pools-api-openapi.yml
operations:
- listNetworkPools
- createNetworkPool
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/broadcom-network-pools-api-openapi.yml ; every operationId checked against the contract
---

# broadcom-network-pools-create

Create a new network pool after optionally listing existing pools.

## Steps

1. 1. Call `listNetworkPools` – supports query parameters `page` and `limit` for pagination.
2. 2. Call `createNetworkPool` – send the required request body fields as defined in the contract.

## Rules

- Authentication: include either a `Authorization: Basic <credentials>` header, a `Authorization: Bearer <token>` header, or a `vmware-api-session-id` header for sessionAuth.
- Pagination: use `page` and `limit` query parameters when listing network pools.
- Errors: the API returns standard HTTP error codes; no specific rate‑limit headers are defined.
