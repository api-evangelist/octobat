# Octobat (octobat)

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

Octobat is a billing, invoicing, and tax-compliance platform for online businesses. It automates the creation, delivery, and storage of legally compliant invoices, credit notes, self-billing invoices, and tax receipts for every online transaction, and provides a real-time tax (VAT / GST / sales tax) determination engine for tax-exclusive and tax-inclusive billing models. Octobat integrates with Stripe, GoCardless, and other payment providers, and exposes a Stripe-style REST API at base URL `https://apiv2.octobat.com` authenticated with HTTP Basic (secret key as username, empty password). Octobat also ships Beanie (a hosted checkout) and Plaza (marketplace / platform tax and invoicing for connected accounts).

**Operating status:** Octobat was acquired by [Mirakl](https://www.mirakl.com/news/mirakl-acquires-invoice-compliance-startup-octobat) in November 2021. The standalone marketing site (octobat.com) now redirects to mirakl.com, and its invoice-compliance capability is largely delivered as part of the Mirakl marketplace platform. The developer documentation at [docs.octobat.com](https://docs.octobat.com) and the `apiv2.octobat.com` API remain available to existing integrators; public, reconciled pricing is no longer published.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/apis.yml)

## Tags

- Billing
- Invoicing
- Tax Compliance
- VAT
- E-Commerce
- Payments
- Fintech

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Octobat Invoices API

Create, list, retrieve, update, and delete compliant invoices, then add invoice items, confirm (finalize) them, set payment terms, send them by email, mark them uncollectible, cancel, cancel-and-replace, and export to PDF or CSV. Confirming an invoice assigns it a sequential legal number; listing supports filtering by customer and status (including due / unpaid invoices).

- **Human URL:** [https://docs.octobat.com/octobat/development/api](https://docs.octobat.com/octobat/development/api)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Invoices
- Billing
- Documents

#### Properties

- [Documentation](https://docs.octobat.com/octobat/development/api)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Credit Notes API

Create, list, and retrieve compliant credit notes issued against invoices for refunds, corrections, and cancellations, with the same numbering, tax, and document-generation guarantees as invoices.

- **Human URL:** [https://docs.octobat.com/octobat/development/api](https://docs.octobat.com/octobat/development/api)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Credit Notes
- Refunds
- Documents

#### Properties

- [Documentation](https://docs.octobat.com/octobat/development/api)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Transactions API

Register successful payments from any payment provider (Stripe, GoCardless, or a generic integration) so Octobat can reconcile them against invoices, drive tax reporting, and mark invoices as paid. Create, list, update transactions, list their items, and export to CSV.

- **Human URL:** [https://docs.octobat.com/octobat/integrations-docs/generic-integration/register-transactions-in-octobat](https://docs.octobat.com/octobat/integrations-docs/generic-integration/register-transactions-in-octobat)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Transactions
- Payments
- Reconciliation

#### Properties

- [Documentation](https://docs.octobat.com/octobat/integrations-docs/generic-integration/register-transactions-in-octobat)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Customers API

Create, list, retrieve, update, and delete customers, capturing the billing address, country, and tax number needed for compliant invoicing. List a customer's invoices, credit notes, payment sources, and balance transactions.

- **Human URL:** [https://docs.octobat.com/octobat/development/api](https://docs.octobat.com/octobat/development/api)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Customers
- Billing Details
- Tax

#### Properties

- [Documentation](https://docs.octobat.com/octobat/development/api)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Products API

Create, list, retrieve, and update products, including the product type used to drive tax categorization (for example digital goods versus services) so the tax engine applies the correct rate per jurisdiction.

- **Human URL:** [https://docs.octobat.com/octobat/development/api](https://docs.octobat.com/octobat/development/api)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Products
- Catalog
- Tax Categories

#### Properties

- [Documentation](https://docs.octobat.com/octobat/development/api)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Tax Evidence API

Real-time tax determination engine. Create a TaxEvidence for a registered customer, or a TaxEvidenceRequest for a not-yet-registered buyer at cart / checkout time (including B2B reverse-charge via a tax number), returning the applied rate, tax zone, and an evidence ID to store with the order for compliance and reconciliation.

- **Human URL:** [https://docs.octobat.com/octobat/integrations-docs/generic-integration/tax-calculation-for-a-cart-or-an-order](https://docs.octobat.com/octobat/integrations-docs/generic-integration/tax-calculation-for-a-cart-or-an-order)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Tax
- VAT
- Tax Determination

#### Properties

- [Documentation](https://docs.octobat.com/octobat/integrations-docs/generic-integration/tax-calculation-for-a-cart-or-an-order)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Coupons API

Create, list, retrieve, update, activate, deactivate, and delete coupons used to apply discounts to invoices and subscriptions.

- **Human URL:** [https://docs.octobat.com/octobat/development/api](https://docs.octobat.com/octobat/development/api)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Coupons
- Discounts
- Promotions

#### Properties

- [Documentation](https://docs.octobat.com/octobat/development/api)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Subscriptions API

Create and list subscriptions for recurring-billing models, and record usage items against a metered subscription so invoices reflect consumption for usage-based and tax-exclusive pricing.

- **Human URL:** [https://docs.octobat.com/octobat/development/api](https://docs.octobat.com/octobat/development/api)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Subscriptions
- Recurring Billing
- Usage

#### Properties

- [Documentation](https://docs.octobat.com/octobat/development/api)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Octobat Payouts API

List and retrieve payouts, drill into the balance transactions that make up each payout, and export payouts to CSV - the settlement side used by platforms and marketplaces (Octobat Plaza) to reconcile funds paid to connected accounts.

- **Human URL:** [https://docs.octobat.com/octobat/development/api](https://docs.octobat.com/octobat/development/api)
- **Base URL:** `https://apiv2.octobat.com`

#### Tags

- Payouts
- Balance
- Marketplace

#### Properties

- [Documentation](https://docs.octobat.com/octobat/development/api)
- [API Reference](https://v2apidoc.octobat.com)
- [OpenAPI](openapi/octobat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/octobat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/octobat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/0ctobat)
- [LinkedIn](https://www.linkedin.com/company/octobat)
- [Website](https://www.octobat.com)
- [Documentation](https://docs.octobat.com)
- [Plans](plans/octobat-plans-pricing.yml)
- [Rate Limits](rate-limits/octobat-rate-limits.yml)
- [Fin Ops](finops/octobat-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
