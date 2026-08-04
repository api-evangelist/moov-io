# Moov (moov-io)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Moov is a money-movement platform that lets software teams accept, store, send, and spend money through a single REST API. The Moov API covers accounts and onboarding, representatives, capabilities and underwriting, funding sources (bank accounts, cards, Apple Pay, Google Pay, wallets), and money movement across ACH, RTP, push-to-card, and card acquiring - plus transfers, refunds, disputes, sweeps, and card issuing.

Moov also maintains a well-known open-source GitHub organization ([github.com/moov-io](https://github.com/moov-io)) of Go libraries and Dockerized HTTP servers for banking file formats - ACH, wire, IAT, and more. Those OSS projects are self-hostable and carry their own OpenAPI specs; they are **distinct** from the commercial hosted money-movement API documented here. This catalog entry focuses on the commercial Moov API at `https://api.moov.io`. The commercial platform SDKs are published under the [github.com/moovfinancial](https://github.com/moovfinancial) organization and are generated from Moov's OpenAPI spec.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/apis.yml)

## Tags

- Payments
- Money Movement
- Fintech
- ACH
- RTP
- Cards
- Wallets
- Embedded Finance

## Timestamps

- **Created:** 2026-07-02
- **Modified:** 2026-07-02

## APIs

### Moov Accounts API

Create and manage Moov accounts for businesses and individuals - the core identity onto which funding sources, capabilities, and money movement are attached. Supports creating, listing, retrieving, updating, and disconnecting accounts, plus account connections and a terms-of-service token.

- **Human URL:** [https://docs.moov.io/api/moov-accounts/accounts/](https://docs.moov.io/api/moov-accounts/accounts/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Accounts
- Onboarding
- KYC

#### Properties

- [API Reference](https://docs.moov.io/api/moov-accounts/accounts/)
- [Documentation](https://docs.moov.io/guides/accounts/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/moov-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moov-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moov Representatives API

Add, list, retrieve, update, and remove the beneficial owners and controllers (representatives) attached to a business account for KYC / KYB verification.

- **Human URL:** [https://docs.moov.io/api/moov-accounts/representatives/](https://docs.moov.io/api/moov-accounts/representatives/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Representatives
- KYC
- Ownership

#### Properties

- [API Reference](https://docs.moov.io/api/moov-accounts/representatives/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/moov-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Moov Capabilities API

Request, list, retrieve, and disable the capabilities (transfers, send-funds, collect-funds, wallet, card-issuing, etc.) that determine what money movement an account is enabled to perform.

- **Human URL:** [https://docs.moov.io/api/moov-accounts/capabilities/](https://docs.moov.io/api/moov-accounts/capabilities/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Capabilities
- Onboarding
- Compliance

#### Properties

- [API Reference](https://docs.moov.io/api/moov-accounts/capabilities/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Underwriting API

Retrieve and update the underwriting details (expected activity, volume, and business model) Moov uses to enable card acquiring and higher-risk money-movement capabilities on an account.

- **Human URL:** [https://docs.moov.io/api/moov-accounts/underwriting/](https://docs.moov.io/api/moov-accounts/underwriting/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Underwriting
- Risk
- Compliance

#### Properties

- [API Reference](https://docs.moov.io/api/moov-accounts/underwriting/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Bank Accounts API

Link, list, retrieve, and delete bank accounts as funding sources, and verify them via instant verification or micro-deposits for ACH and RTP money movement.

- **Human URL:** [https://docs.moov.io/api/sources/bank-accounts/](https://docs.moov.io/api/sources/bank-accounts/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Bank Accounts
- ACH
- Verification

#### Properties

- [API Reference](https://docs.moov.io/api/sources/bank-accounts/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/moov-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Moov Cards API

Link, list, retrieve, update, and disable payment cards as funding sources, with verification (CVV / address) for card acquiring, pull-from-card, and push-to-card money movement.

- **Human URL:** [https://docs.moov.io/api/sources/cards/](https://docs.moov.io/api/sources/cards/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Cards
- Funding Source
- PCI

#### Properties

- [API Reference](https://docs.moov.io/api/sources/cards/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/moov-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Moov Wallets API

Create and manage Moov wallets (stored-balance accounts), inspect wallet balances and their ledgered transactions, and review balance adjustments.

- **Human URL:** [https://docs.moov.io/api/sources/wallets/](https://docs.moov.io/api/sources/wallets/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Wallets
- Balances
- Ledger

#### Properties

- [API Reference](https://docs.moov.io/api/sources/wallets/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Payment Methods API

List and retrieve the payment methods available on an account - the concrete combinations of a funding source (bank account, card, or wallet) and a rail (ACH, RTP, card, wallet) that can be used as the source or destination of a transfer.

- **Human URL:** [https://docs.moov.io/api/sources/payment-methods/](https://docs.moov.io/api/sources/payment-methods/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Payment Methods
- Rails
- Funding Source

#### Properties

- [API Reference](https://docs.moov.io/api/sources/payment-methods/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Transfers API

Move money between funding sources across ACH, RTP, push-to-card, and card acquiring. Create, list, retrieve, and patch transfers; look up transfer options and per-account transfer configuration; and cancel transfers.

- **Human URL:** [https://docs.moov.io/api/money-movement/transfers/](https://docs.moov.io/api/money-movement/transfers/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Transfers
- Money Movement
- ACH
- RTP

#### Properties

- [API Reference](https://docs.moov.io/api/money-movement/transfers/)
- [Documentation](https://docs.moov.io/guides/money-movement/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/moov-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Moov Refunds API

Refund and reverse card transfers - create a refund on a completed card transfer, cancel or reverse a still-authorized card transfer, and list or retrieve the refunds on a transfer.

- **Human URL:** [https://docs.moov.io/api/money-movement/refunds/](https://docs.moov.io/api/money-movement/refunds/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Refunds
- Reversals
- Cards

#### Properties

- [API Reference](https://docs.moov.io/api/money-movement/refunds/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Sweeps API

Configure automated sweeps that move accumulated wallet balances to a designated bank account on a schedule. Create, list, retrieve, and update sweep configurations, and inspect the individual sweeps they produce.

- **Human URL:** [https://docs.moov.io/api/money-movement/sweeps/](https://docs.moov.io/api/money-movement/sweeps/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Sweeps
- Wallets
- Automation

#### Properties

- [API Reference](https://docs.moov.io/api/money-movement/sweeps/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Disputes API

Manage card disputes and chargebacks - list and retrieve disputes, accept a dispute, and upload, submit, list, retrieve, and delete the evidence (files and text) used to respond to a dispute.

- **Human URL:** [https://docs.moov.io/api/money-movement/disputes/](https://docs.moov.io/api/money-movement/disputes/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Disputes
- Chargebacks
- Evidence

#### Properties

- [API Reference](https://docs.moov.io/api/money-movement/disputes/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Card Issuing API

Issue virtual spending cards backed by a Moov wallet, retrieve full PCI card details, and review the authorizations, authorization events, and settled card transactions those issued cards generate.

- **Human URL:** [https://docs.moov.io/guides/money-movement/spend/card-issuing/](https://docs.moov.io/guides/money-movement/spend/card-issuing/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Card Issuing
- Virtual Cards
- Spend

#### Properties

- [Documentation](https://docs.moov.io/guides/money-movement/spend/card-issuing/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moov Institutions API

Validate a financial institution by routing number before initiating payment activity, and check which payment rails (ACH, RTP, wire) are available for a given routing number.

- **Human URL:** [https://docs.moov.io/api/enrichment/institutions/](https://docs.moov.io/api/enrichment/institutions/)
- **Base URL:** `https://api.moov.io`

#### Tags

- Institutions
- Routing Numbers
- Enrichment

#### Properties

- [API Reference](https://docs.moov.io/api/enrichment/institutions/)
- [OpenAPI](openapi/moov-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/moov-io)
- [LinkedIn](https://www.linkedin.com/company/moov-financial)
- [Website](https://moov.io)
- [Documentation](https://docs.moov.io)
- [Plans](plans/moov-io-plans-pricing.yml)
- [Rate Limits](rate-limits/moov-io-rate-limits.yml)
- [Fin Ops](finops/moov-io-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
