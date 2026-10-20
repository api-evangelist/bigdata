---
name: bigdata-fetch-market-data
description: Retrieve market data such as daily prices, intraday prices, and a company quote.
api: openapi/bigdata-structured_data.json
operations:
- query_daily_prices_v1_price_daily_query_post
- query_intraday_prices_v1_price_intraday_query_post
- query_company_quote_v1_quote_query_post
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bigdata-structured_data.json ; every operationId checked against the contract
---

# bigdata-fetch-market-data

Retrieve market data such as daily prices, intraday prices, and a company quote.

## Steps

1. 1. Call `query_daily_prices_v1_price_daily_query_post` with the required request body fields and include the `X-API-KEY` header.
2. 2. Call `query_intraday_prices_v1_price_intraday_query_post` with the required request body fields and include the `X-API-KEY` header.
3. 3. Call `query_company_quote_v1_quote_query_post` with the required request body fields and include the `X-API-KEY` header.

## Rules

- Auth: Provide the API key in the `X-API-KEY` header (ApiKeyAuth).
- Rate limit: 500 requests per minute; on exhaustion the response has no specific HTTP status code defined.
