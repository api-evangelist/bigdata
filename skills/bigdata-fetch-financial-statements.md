---
name: bigdata-fetch-financial-statements
description: Retrieve the main financial statements and key metrics for a company.
api: openapi/bigdata-structured_data.json
operations:
- query_balance_sheet_v1_balance_sheet_query_post
- query_income_statement_v1_income_statement_query_post
- query_cash_flow_statement_v1_cash_flow_statement_query_post
- query_company_ratios_ttm_v1_company_ratios_ttm_query_post
- query_key_metrics_TTM_v1_key_metrics_ttm_query_post
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bigdata-structured_data.json ; every operationId checked against the contract
---

# bigdata-fetch-financial-statements

Retrieve the main financial statements and key metrics for a company.

## Steps

1. 1. Call `query_balance_sheet_v1_balance_sheet_query_post` with the required request body and include the `X-API-KEY` header.
2. 2. Call `query_income_statement_v1_income_statement_query_post` with the required request body and include the `X-API-KEY` header.
3. 3. Call `query_cash_flow_statement_v1_cash_flow_statement_query_post` with the required request body and include the `X-API-KEY` header.
4. 4. Call `query_company_ratios_ttm_v1_company_ratios_ttm_query_post` with the required request body and include the `X-API-KEY` header.
5. 5. Call `query_key_metrics_TTM_v1_key_metrics_ttm_query_post` with the required request body and include the `X-API-KEY` header.

## Rules

- Auth: Provide the API key in the `X-API-KEY` request header (ApiKeyAuth).
- Rate limit: Maximum 500 requests per minute.
