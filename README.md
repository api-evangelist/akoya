# Akoya (akoya)

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
