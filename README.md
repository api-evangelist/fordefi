# Fordefi

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Fordefi is an institutional MPC (multi-party computation) wallet and digital-asset security platform for DeFi, trading, and on-chain payments. Its developer API lets teams programmatically create vaults across 10+ blockchain families (EVM, Bitcoin, Solana, Cosmos and more), manage addresses and assets, and build, approve, sign, and broadcast transactions under a policy engine with built-in AML screening and audit logging. Authentication combines a Bearer JWT access token with ECDSA (NIST P-256) request signing by a registered API Signer; state-changing calls support idempotency and a signed webhook event surface for real-time monitoring. Fordefi is SOC 2 Type II certified. This profile was enriched by the API Evangelist pipeline from Fordefi's public OpenAPI and developer documentation.

**Areas:** Company · Security · Cryptocurrency · Digital Assets · Wallets · Custody · Blockchain · DeFi · MPC · Payments

## Fordefi on APIs.io

Everything profiled for Fordefi is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/fordefi/](https://apis.io/providers/fordefi/)** — or go straight to one of the APIs or properties below.

### APIs (17)

- [Fordefi Address Book API](https://apis.io/apis/fordefi/fordefi-address-book-api/) — These endpoints allow you to list the contacts in your address book.<br><br>To add/remove contacts, visit the Fordefi web console. See the <a…
- [Fordefi Assets API](https://apis.io/apis/fordefi/fordefi-assets-api/) — These endpoints allow you to get information about the assets in your organization, including metadata, balances, and prices. <br><br> Fordefi supports…
- [Fordefi Audit Log API](https://apis.io/apis/fordefi/fordefi-audit-log-api/) — These endpoints allow you to manage audit logs. <br><br> Audit logs are used to track the actions of users in your organization.
- [Fordefi Authorization Tokens API](https://apis.io/apis/fordefi/fordefi-authorization-tokens-api/) — These endpoints allow you to manage end-user authorization tokens used for Fordefi's WaaS solution.<br><br>Authorization tokens allow end users to…
- [Fordefi Batch Transactions API](https://apis.io/apis/fordefi/fordefi-batch-transactions-api/) — These endpoints allow you to manage batch transactions on the Fordefi platform. <br><br> Batch transactions are currently supported only on Solana, for the…
- [Fordefi Blockchains API](https://apis.io/apis/fordefi/fordefi-blockchains-api/) — These endpoints allow you to get information about blockchains supported by Fordefi.
- [Fordefi Enclave Keys API](https://apis.io/apis/fordefi/fordefi-enclave-keys-api/) — The Enclave Keys API from Fordefi — 1 operation(s) for enclave keys.
- [Fordefi End Users API](https://apis.io/apis/fordefi/fordefi-end-users-api/) — These endpoints allow you to manage WaaS end-users. <br><br> End users correspond to users of the platform who has integrated the Fordefi WaaS solution. For…
- [Fordefi Exports API](https://apis.io/apis/fordefi/fordefi-exports-api/) — These endpoints allow you to manage asynchronous actions such as data exports.
- [Fordefi Organizations API](https://apis.io/apis/fordefi/fordefi-organizations-api/) — The Organizations API from Fordefi — 4 operation(s) for organizations.
- [Fordefi Swaps API](https://apis.io/apis/fordefi/fordefi-swaps-api/) — These endpoints allow you to manage swaps.
- [Fordefi Transactions API](https://apis.io/apis/fordefi/fordefi-transactions-api/) — These endpoints allow you to manage transactions on the Fordefi platform. <br><br> A transaction represents an operation that can be one of the following:…
- [Fordefi User Groups API](https://apis.io/apis/fordefi/fordefi-user-groups-api/) — These endpoints allow you to view your user groups. <br><br> User Groups are used to collectively manage policies and view permissions for a group of users.…
- [Fordefi Users API](https://apis.io/apis/fordefi/fordefi-users-api/) — These endpoints allow you to get information about users in your Fordefi organization. There are several types of users in the Fordefi platform: -…
- [Fordefi Vault Groups API](https://apis.io/apis/fordefi/fordefi-vault-groups-api/) — These endpoints allow you to view your vault groups. <br><br> Vault Groups are used to collectively manage policies and view permissions for a group of…
- [Fordefi Vaults API](https://apis.io/apis/fordefi/fordefi-vaults-api/) — These endpoints allow you to manage vaults. <br><br> A vault is the basic unit to manage funds. Each vault supports a single "chain family", such as EVM,…
- [Fordefi Webhooks API](https://apis.io/apis/fordefi/fordefi-webhooks-api/) — These endpoints allow you to manually trigger your pre-configured webhooks.<br><br><a href='https://docs.fordefi.com/reference/webhooks'>Use Webhooks</a>…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Fordefi Webhooks](https://apis.io/asyncapis/fordefi/fordefi-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [fordefi](https://apis.io/servers/fordefi/fordefi/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Fordefi Agentic Access](https://apis.io/agentic-access/fordefi/fordefi-agentic-access/)

#### Collections (17)

Postman and Open Collection request collections.

- [Fordefi Address Book API](https://apis.io/collections/fordefi/open-fordefi-address-book-api/)
- [Fordefi Address Book Assets API](https://apis.io/collections/fordefi/open-fordefi-assets-api/)
- [Fordefi Address Book Audit Log API](https://apis.io/collections/fordefi/open-fordefi-audit-log-api/)
- [Fordefi Address Book Authorization Tokens API](https://apis.io/collections/fordefi/open-fordefi-authorization-tokens-api/)
- [Fordefi Address Book Batch Transactions API](https://apis.io/collections/fordefi/open-fordefi-batch-transactions-api/)
- [Fordefi Address Book Blockchains API](https://apis.io/collections/fordefi/open-fordefi-blockchains-api/)
- [Fordefi Address Book Enclave Keys API](https://apis.io/collections/fordefi/open-fordefi-enclave-keys-api/)
- [Fordefi Address Book End Users API](https://apis.io/collections/fordefi/open-fordefi-end-users-api/)
- [Fordefi Address Book Exports API](https://apis.io/collections/fordefi/open-fordefi-exports-api/)
- [Fordefi Address Book Organizations API](https://apis.io/collections/fordefi/open-fordefi-organizations-api/)
- [Fordefi Address Book Swaps API](https://apis.io/collections/fordefi/open-fordefi-swaps-api/)
- [Fordefi Address Book Transactions API](https://apis.io/collections/fordefi/open-fordefi-transactions-api/)
- [Fordefi Address Book User Groups API](https://apis.io/collections/fordefi/open-fordefi-user-groups-api/)
- [Fordefi Address Book Users API](https://apis.io/collections/fordefi/open-fordefi-users-api/)
- [Fordefi Address Book Vault Groups API](https://apis.io/collections/fordefi/open-fordefi-vault-groups-api/)
- [Fordefi Address Book Vaults API](https://apis.io/collections/fordefi/open-fordefi-vaults-api/)
- [Fordefi Address Book Webhooks API](https://apis.io/collections/fordefi/open-fordefi-webhooks-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Fordefi Openapi Overlay](https://apis.io/overlays/fordefi/fordefi-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Fordefi Authentication](https://apis.io/security/fordefi/fordefi-authentication/)
- [Fordefi Domain Security](https://apis.io/security/fordefi/fordefi-domain-security/)
- [Fordefi Trust Center](https://apis.io/security/fordefi/fordefi-trust-center/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://fordefi.com/)
- [Documentation](https://docs.fordefi.com/developers/api-overview)
- [Getting started](https://docs.fordefi.com/developers/getting-started/create-an-api-user)
- [API reference](https://docs.fordefi.com/api/openapi)
- [Sign up](https://app.fordefi.com/)
- [Blog](https://medium.com/fordefi)
- [Compliance](https://fordefi.com/solutions/mpc-security)
- [Terms of service](https://fordefi.com/terms-and-conditions)
- [Privacy policy](https://fordefi.com/privacy-policy)
- [GitHub](https://github.com/FordefiHQ)
- [Status](https://status.fordefi.com/)

## API Evangelist rating

**Kin Score 53.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 58.3 |
| Contract governance | 18.2 |
| Operational transparency | 50.0 |
| Developer ergonomics | 62.5 |
| Access clarity | 36.8 |

**Agent readiness 37.8** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 26.8** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/fordefi/](https://apis.io/providers/fordefi/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Fordefi: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/fordefi/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
