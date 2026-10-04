---
name: broadcom-session-create-and-delete
description: Create a new Broadcom API session and then delete it when finished.
api: openapi/broadcom-session-api-openapi.yml
operations:
- createSession
- deleteSession
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/broadcom-session-api-openapi.yml ; every operationId checked against the contract
---

# broadcom-session-create-and-delete

Create a new Broadcom API session and then delete it when finished.

## Steps

1. 1. `createSession` – requires the `vmware-api-session-id` header (sessionAuth).
2. 2. `deleteSession` – requires the same `vmware-api-session-id` header to identify the session to delete.

## Rules

- Authentication: provide the session token in the `vmware-api-session-id` header using the `sessionAuth` scheme.
- No pagination parameters are needed for these operations.
