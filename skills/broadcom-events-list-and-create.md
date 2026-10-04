---
name: broadcom-events-list-and-create
description: Retrieve a paginated list of events and then create a new event.
api: openapi/broadcom-events-api-openapi.yml
operations:
- listEvents
- createEvent
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/broadcom-events-api-openapi.yml ; every operationId checked against the contract
---

# broadcom-events-list-and-create

Retrieve a paginated list of events and then create a new event.

## Steps

1. 1. Call `listEvents` with optional query parameters `page` and `limit` to retrieve events.
2. 2. Call `createEvent` with the required request body fields for the new event.

## Rules

- Authentication: include one of the supported auth schemes – Basic (`Authorization: Basic …`), Bearer (`Authorization: Bearer …`), or Session (`vmware-api-session-id: <token>`).
- Pagination: `listEvents` supports `page` and `limit` query parameters.
- Idempotency: not defined for these operations; callers should ensure they do not unintentionally duplicate events.
