---
name: Create a vault and generate a receiving address
description: Provision a Fordefi vault for a chain family and derive a receiving address, then read its assets.
api: openapi/fordefi-openapi-original.json
operations:
  - create_vault_api_v1_vaults_post
  - create_address_api_v1_vaults__id__addresses_post
  - list_vault_addresses_api_v1_vaults__id__addresses_get
  - get_vault_assets_api_v1_vaults__id__assets_get
---

# Create a vault and generate a receiving address

Use this to stand up custody for a new chain family in Fordefi.

## Auth
- Send `Authorization: Bearer {api_access_token}`.
- `create_vault` is state-changing: also send an ECDSA (NIST P-256) `x-signature`
  over `"${path}|${timestamp}|${body}"` plus `x-timestamp`, signed by your API Signer.
- Set a stable `x-idempotence-id` so retries do not create duplicate vaults.

## Steps
1. **create_vault_api_v1_vaults_post** — `POST /api/v1/vaults`. Choose the chain
   family (EVM, Bitcoin, Solana, Cosmos, ...). One vault serves a single family.
2. **create_address_api_v1_vaults__id__addresses_post** — `POST /api/v1/vaults/{id}/addresses`.
   Derive a receiving address in the new vault.
3. **list_vault_addresses_api_v1_vaults__id__addresses_get** — `GET /api/v1/vaults/{id}/addresses`
   to confirm the address.
4. **get_vault_assets_api_v1_vaults__id__assets_get** — `GET /api/v1/vaults/{id}/assets`
   to read balances once funded.

## Errors
See `errors/fordefi-problem-types.yml`. Handle `401` (token), `403` (policy),
`422` (validation); every error carries a `request_id` for support.
