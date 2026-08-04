# Coterie Insurance (coterie)

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

Coterie Insurance is a technology-first commercial insurance provider for small businesses, offering Business Owners Policy (BOP), General Liability (GL), Professional Liability (PL), and Workers' Compensation (WC). Its REST API lets appointed agents and digital partners build applications, generate bindable quotes, bind and issue policies, look up industry/NAICS classifications, retrieve policy documents, and subscribe to webhooks for an embedded small-business insurance experience.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/apis.yml)

## Tags

- Insurance
- Commercial Insurance
- Small Business
- Embedded Insurance
- Insurtech

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### Coterie Quotes API

Generates rated, bindable quotes for one or more lines of business (BOP, GL, PL, WC) and answers underwriting questions. Quotes are immutable and tied to an application; only "Ready to Bind" quotes guarantee pricing accuracy.

- **Human URL:** [https://docs.coterieinsurance.com/](https://docs.coterieinsurance.com/)
- **Base URL:** `https://api.coterieinsurance.com/v1`

#### Tags

- Quotes
- Bindable Quote
- Underwriting

#### Properties

- [Documentation](https://docs.coterieinsurance.com/)
- [OpenAPI](openapi/coterie-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coterie.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coterie.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Coterie Policies API

Binds an existing bindable quote into an active policy and issues coverage, including binding via Stripe payment token. Returns policy numbers and status for BOP, GL, PL, and WC lines of business.

- **Human URL:** [https://docs.coterieinsurance.com/](https://docs.coterieinsurance.com/)
- **Base URL:** `https://api.coterieinsurance.com/v1`

#### Tags

- Policies
- Bind
- Issue

#### Properties

- [Documentation](https://docs.coterieinsurance.com/)
- [OpenAPI](openapi/coterie-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coterie.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coterie.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Coterie Applications API

Creates and retrieves commercial applications describing the insured business. Applications hold a 1:Many relationship with quotes and policies and remain stable while quotes change over time.

- **Human URL:** [https://docs.coterieinsurance.com/](https://docs.coterieinsurance.com/)
- **Base URL:** `https://api.coterieinsurance.com/v1`

#### Tags

- Applications
- Account
- Insured

#### Properties

- [Documentation](https://docs.coterieinsurance.com/)
- [OpenAPI](openapi/coterie-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coterie.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coterie.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Coterie Industry / NAICS API

Resolves a business description to an industry classification, returning the IndustryId and AK Hash (NAICS combined with a description MD5 hash) required when submitting applications and quotes.

- **Human URL:** [https://docs.coterieinsurance.com/](https://docs.coterieinsurance.com/)
- **Base URL:** `https://api.coterieinsurance.com/v1`

#### Tags

- Industry
- NAICS
- Classification

#### Properties

- [Documentation](https://docs.coterieinsurance.com/)
- [OpenAPI](openapi/coterie-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coterie.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coterie.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Coterie Documents API

Retrieves policy documents and proposals generated for a quote or an issued policy, including the documentation delivered to the policyholder on successful policy issuance.

- **Human URL:** [https://docs.coterieinsurance.com/](https://docs.coterieinsurance.com/)
- **Base URL:** `https://api.coterieinsurance.com/v1`

#### Tags

- Documents
- Policy Documents
- PDF

#### Properties

- [Documentation](https://docs.coterieinsurance.com/)
- [OpenAPI](openapi/coterie-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coterie.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coterie.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Coterie Webhooks API

Manages webhook subscriptions that notify partner systems of policy lifecycle events, including issuance, cancelation, and updated premium information delivered via the policy webhook.

- **Human URL:** [https://docs.coterieinsurance.com/](https://docs.coterieinsurance.com/)
- **Base URL:** `https://api.coterieinsurance.com/v1`

#### Tags

- Webhooks
- Notifications
- Events

#### Properties

- [Documentation](https://docs.coterieinsurance.com/)
- [OpenAPI](openapi/coterie-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coterie.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coterie.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/CoterieInsure)
- [LinkedIn](https://www.linkedin.com/company/coterie-insurance)
- [Website](https://coterieinsurance.com/)
- [Documentation](https://docs.coterieinsurance.com/)
- [Plans](plans/coterie-plans-pricing.yml)
- [Rate Limits](rate-limits/coterie-rate-limits.yml)
- [Fin Ops](finops/coterie-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
