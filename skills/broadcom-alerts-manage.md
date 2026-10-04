---
name: broadcom-alerts-manage
description: Manage Broadcom alerts by listing, creating, retrieving, updating, and deleting them.
api: openapi/broadcom-alerts-api-openapi.yml
operations:
- listAlerts
- createAlert
- getAlert
- updateAlert
- deleteAlert
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/broadcom-alerts-api-openapi.yml ; every operationId checked against the contract
---

# broadcom-alerts-manage

Manage Broadcom alerts by listing, creating, retrieving, updating, and deleting them.

## Steps

1. 1. Use `listAlerts` with query parameters `page` and `limit` for pagination.
2. 2. Use `createAlert` with the request body containing the alert fields.
3. 3. Use `getAlert` with path parameter `id` to retrieve a specific alert.
4. 4. Use `updateAlert` with path parameter `id` and request body containing updated alert fields.
5. 5. Use `deleteAlert` with path parameter `id` to remove an alert.

## Rules

- Authentication: Provide one of the supported auth schemes – basicAuth (HTTP), bearerAuth (HTTP), or sessionAuth (API key in header `vmware-api-session-id`).
- Pagination: Use `page` and `limit` query parameters on `listAlerts` to control result sets.
