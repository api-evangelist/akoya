# Akoya (akoya)

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

Akoya is a tokenized data-access network for US financial institutions. It implements the Financial Data Exchange (FDX) API standard, replacing screen-scraping with token-permissioned API access to consumer accounts.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/akoya/refs/heads/main/apis.yml)

## Type
- **x-type:** company

## Tags
- Fintech, Open Banking, Open Finance, Aggregator, Data Access Network, Tokenized, Consumer-Permissioned, FDX, Account Aggregation, United States

## APIs
Production base URL `https://api.akoya.com`; sandbox routes are data-provider-scoped under `ddp.akoya.com` (e.g. `https://sandbox-products.ddp.akoya.com`). All products are FDX-aligned and use OAuth 2.0 consumer-permissioned access.

Consumer data-access products:
- **Akoya Accounts API** - Accounts + Account Details (FDX)
- **Akoya Balances API** - real-time / available balances
- **Akoya Transactions API** - permissioned transaction history
- **Akoya Investments API** - holdings + tax lots
- **Akoya Statements API** - available account statements
- **Akoya Customers API** - customer/party identity + contact
- **Akoya Tax API** - 1099 tax form variants
- **Akoya Payments API** - tokenized ACH/RTP account credentials

Platform / service APIs:
- **Akoya Consent API** - consent grant lookup/management
- **Akoya Apps Management API** - recipient app registration/administration
- **Akoya Notifications API** - outage/availability webhooks

## Notes on OpenAPI
Akoya authors its docs as OpenAPI 3.1.0 but renders them client-side via the docs.akoya.com readme.io reference hub — there is **no publicly downloadable OpenAPI/Postman artifact** (guessable spec paths 404). The GitHub org `github.com/akoya-llc` publishes only Go code samples for the OAuth flow. Represented humanURL-only, honestly. The FDX standard at https://financialdataexchange.org/ is the canonical specification. Production access requires an Akoya network membership agreement (free self-service sandbox available).

## Timestamps
- **Created:** 2026-05-08
- **Modified:** 2026-07-23

## Common Properties
- [Portal](https://akoya.com/)
- [Documentation](https://docs.akoya.com/)
- [FDX Standard](https://financialdataexchange.org/)
- [Plans](plans/akoya-plans-pricing.yml) - reconciled (network membership)
- [RateLimits](rate-limits/akoya-rate-limits.yml) - partially reconciled
- [FinOps](finops/akoya-finops.yml) - reconciled FOCUS-aligned

## Maintainers
**FN:** Kin Lane

**Email:** kin@apievangelist.com
