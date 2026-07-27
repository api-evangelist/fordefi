---
name: Create, sign and monitor a transaction
description: Submit a Fordefi transaction, move it through approval/signing, and poll to completion.
api: openapi/fordefi-openapi-original.json
operations:
  - create_transaction_api_v1_transactions_post
  - approve_transaction_api_v1_transactions__id__approve_post
  - trigger_transaction_signing_api_v1_transactions__id__trigger_signing_post
  - get_transaction_api_v1_transactions__id__get
---

# Create, sign and monitor a transaction

## Auth
- `Authorization: Bearer {api_access_token}`.
- Transaction creation and approval are state-changing: send the ECDSA P-256
  `x-signature` + `x-timestamp` from your API Signer.
- Pass a stable `x-idempotence-id` on `create_transaction` to make retries safe.

## Steps
1. **create_transaction_api_v1_transactions_post** — `POST /api/v1/transactions`.
   Build the transaction against a vault; capture the returned transaction `id`.
2. **approve_transaction_api_v1_transactions__id__approve_post** — `POST /api/v1/transactions/{id}/approve`.
   Satisfy the vault's policy quorum. (Use `.../abort` to cancel.)
3. **trigger_transaction_signing_api_v1_transactions__id__trigger_signing_post** —
   `POST /api/v1/transactions/{id}/trigger-signing` when signing must be prompted.
4. **get_transaction_api_v1_transactions__id__get** — `GET /api/v1/transactions/{id}`;
   poll until state reaches MINED/COMPLETED, or subscribe to the
   `enriched_transaction_state_update` webhook (see `asyncapi/fordefi-webhooks.yml`).

## Errors
`errors/fordefi-problem-types.yml` — `403` usually means a policy blocked the move.
