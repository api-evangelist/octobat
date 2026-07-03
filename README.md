# Octobat (octobat)

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
