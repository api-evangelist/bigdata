---
name: bigdata-company-profile-and-events
description: Retrieve a company's profile and then fetch related events from the calendar.
api: openapi/bigdata-structured_data.json
operations:
- query_company_profile_v1_company_profile_query_post
- query_events_calendar_v1_events_calendar_query_post
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bigdata-structured_data.json ; every operationId checked against the contract
---

# bigdata-company-profile-and-events

Retrieve a company's profile and then fetch related events from the calendar.

## Steps

1. 1. Call `query_company_profile_v1_company_profile_query_post` with the required request body fields and include the `X-API-KEY` header.
2. 2. Call `query_events_calendar_v1_events_calendar_query_post` with the appropriate request body fields (e.g., company identifier) and include the `X-API-KEY` header.

## Rules

- Auth: Provide the API key in the `X-API-KEY` header (ApiKeyAuth).
- Rate limit: 500 requests per minute; exceeding returns no specific HTTP error code.
- Both endpoints require a JSON request body; the exact fields are defined in the API contract.
