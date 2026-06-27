# Coterie Insurance (coterie)

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
