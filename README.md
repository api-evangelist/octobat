# Octobat

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

Octobat is a billing, invoicing, and tax-compliance platform for online businesses. It automates the creation, delivery, and storage of legally compliant invoices, credit notes, self-billing invoices, and tax receipts for every online transaction, and provides a real-time tax (VAT / GST / sales tax) determination engine for tax-exclusive and tax-inclusive billing models. Octobat integrates with Stripe, GoCardless, and other payment providers, and exposes a Stripe-style REST API at base URL https://apiv2.octobat.com authenticated with HTTP Basic (secret key). Octobat also ships Beanie (a hosted checkout) and Plaza (marketplace / platform tax and invoicing for connected accounts). Operating status - Octobat was acquired by Mirakl in November 2021; the standalone marketing site (octobat.com) now redirects to mirakl.com, while the developer documentation at docs.octobat.com and the apiv2.octobat.com API remain available to existing integrators.

**Areas:** Billing · Invoicing · Tax Compliance · VAT · E-Commerce · Payments · Fintech

## Octobat on APIs.io

Everything profiled for Octobat is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/octobat/](https://apis.io/providers/octobat/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Octobat Coupons API](https://apis.io/apis/octobat/octobat-coupons-api/) — Discount coupons for invoices and subscriptions.
- [Octobat Credit Notes API](https://apis.io/apis/octobat/octobat-credit-notes-api/) — Compliant credit notes issued against invoices.
- [Octobat Customers API](https://apis.io/apis/octobat/octobat-customers-api/) — Customers and their billing / tax details.
- [Octobat Invoices API](https://apis.io/apis/octobat/octobat-invoices-api/) — Compliant invoices, their items, and lifecycle actions.
- [Octobat Payouts API](https://apis.io/apis/octobat/octobat-payouts-api/) — Settlement payouts and their balance transactions.
- [Octobat Products API](https://apis.io/apis/octobat/octobat-products-api/) — Products and their tax categorization.
- [Octobat Subscriptions API](https://apis.io/apis/octobat/octobat-subscriptions-api/) — Recurring-billing subscriptions and metered usage.
- [Octobat Tax Evidence API](https://apis.io/apis/octobat/octobat-tax-evidence-api/) — Real-time tax determination for customers and carts / checkouts.
- [Octobat Transactions API](https://apis.io/apis/octobat/octobat-transactions-api/) — Payments registered against invoices for reconciliation and tax reporting.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Octobat Agentic Access](https://apis.io/agentic-access/octobat/octobat-agentic-access/)

#### Collections (10)

Postman and Open Collection request collections.

- [Octobat API](https://apis.io/collections/octobat/open-octobat/)
- [Octobat Coupons API](https://apis.io/collections/octobat/open-octobat-coupons-api/)
- [Octobat Coupons Credit Notes API](https://apis.io/collections/octobat/open-octobat-credit-notes-api/)
- [Octobat Coupons Customers API](https://apis.io/collections/octobat/open-octobat-customers-api/)
- [Octobat Coupons Invoices API](https://apis.io/collections/octobat/open-octobat-invoices-api/)
- [Octobat Coupons Payouts API](https://apis.io/collections/octobat/open-octobat-payouts-api/)
- [Octobat Coupons Products API](https://apis.io/collections/octobat/open-octobat-products-api/)
- [Octobat Coupons Subscriptions API](https://apis.io/collections/octobat/open-octobat-subscriptions-api/)
- [Octobat Coupons Tax Evidence API](https://apis.io/collections/octobat/open-octobat-tax-evidence-api/)
- [Octobat Coupons Transactions API](https://apis.io/collections/octobat/open-octobat-transactions-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Octobat Authentication](https://apis.io/security/octobat/octobat-authentication/)
- [Octobat Domain Security](https://apis.io/security/octobat/octobat-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Octobat Plans Pricing](https://apis.io/plans/octobat/octobat-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Octobat Rate Limits](https://apis.io/rate-limits/octobat/octobat-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Octobat Finops](https://apis.io/finops/octobat/octobat-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.octobat.com)
- [Documentation](https://docs.octobat.com)
- [Blog](https://www.mirakl.com/blogs/)
- [GitHub](https://github.com/0ctobat)

## API Evangelist rating

**Kin Score 24.9** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 44.0 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 32.1 |
| Access clarity | 7.9 |

**Agent readiness 22.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 10.7** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/octobat/](https://apis.io/providers/octobat/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Octobat: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/octobat/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
