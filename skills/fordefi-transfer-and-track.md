---
name: Transfer assets and track to completion
description: Move assets out of a Fordefi vault with the transfer helper and track the result.
api: openapi/fordefi-openapi-original.json
operations:
  - create_transfer_api_v1_transactions_transfer_post
  - create_transaction_and_wait_api_v1_transactions_create_and_wait_post
  - get_transaction_api_v1_transactions__id__get
  - list_transactions_api_v1_transactions_get
---

# Transfer assets and track to completion

## Auth
- `Authorization: Bearer {api_access_token}` plus ECDSA P-256 `x-signature` /
  `x-timestamp` (state-changing). Use `x-idempotence-id` to make retries safe.

## Steps
1. **create_transfer_api_v1_transactions_transfer_post** — `POST /api/v1/transactions/transfer`.
   Simplified helper for a straight asset transfer from a vault to a destination.
2. Or **create_transaction_and_wait_api_v1_transactions_create_and_wait_post** —
   `POST /api/v1/transactions/create-and-wait` to submit and block until a terminal
   state in one call.
3. **get_transaction_api_v1_transactions__id__get** — `GET /api/v1/transactions/{id}`
   to read final state, gas and effects.
4. **list_transactions_api_v1_transactions_get** — `GET /api/v1/transactions`
   with `created_after`/`limit`/`page` to reconcile activity.

## Errors
See `errors/fordefi-problem-types.yml`; retry-safe on `429` with backoff.
