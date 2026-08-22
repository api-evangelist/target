# target (target)

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

Target Corporation is one of the largest retailers in the United States, offering a wide assortment of general merchandise and food through more than 1,900 stores and digital channels. Target's technology platform powers partner integrations, internal services, and open-source tooling across their retail operations.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/apis.yml)

## Tags

- E-Commerce
- Retail
- Products
- Inventory
- Fortune 100
- Stores
- Orders

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-05-19

## APIs

### Target API

Target provides partner APIs for product catalog access, inventory availability, order management, and store information. These APIs enable technology partners and affiliates to integrate with Target's retail platform. The Redsky aggregation platform powers client-managed REST APIs built on GraphQL queries covering product, price, promotion, and fulfillment data.

- **Human URL:** [https://developer.target.com/](https://developer.target.com/)
- **Base URL:** `https://api.target.com`

#### Tags

- E-Commerce
- Inventory
- Orders
- Products
- Retail
- Stores

#### Properties

- [Documentation](https://developer.target.com/)
- [OpenAPI](openapi/target-target-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/target-target-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/target-target-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/target-spectral-rules.yml)

### Target Redsky API

Redsky is Target's internal aggregation API platform that converts GraphQL queries into client-managed REST APIs. It serves product data, pricing, promotions, and fulfillment information for Target.com and mobile applications. The platform manages 200+ unique APIs across 30 clients backed by 50+ integrations.

- **Human URL:** [https://tech.target.com/blog/empowering-clients-api](https://tech.target.com/blog/empowering-clients-api)
- **Base URL:** `https://redsky.target.com`

#### Tags

- E-Commerce
- GraphQL
- Products
- Retail

#### Properties

- [Documentation](https://tech.target.com/blog/empowering-clients-api)
- [Postman Collection](collections/target-target-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/target-target-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Target Partner API

Target's partner API program enables technology vendors, affiliates, and supply chain partners to integrate with Target's retail operations including product catalog, inventory management, order fulfillment, and store data.

- **Human URL:** [https://developer.target.com/](https://developer.target.com/)
- **Base URL:** `https://api.target.com`

#### Tags

- E-Commerce
- Inventory
- Partners
- Retail
- Suppliers

#### Properties

- [Documentation](https://developer.target.com/)
- [Postman Collection](collections/target-target-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/target-target-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/target)
- [Website](https://www.target.com)
- [Developer  Portal](https://developer.target.com/)
- [Blog](https://tech.target.com)
- [Git Hub  Org](https://github.com/target)
- [Open  Source](https://tech.target.com/open-source)
- [Status Page](https://status.target.com)
- [JSON Schema](json-schema/target-product-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/target-store-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/target-product-structure.json)
- [JSON-LD](json-ld/target-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/target-vocabulary.yml)
- [L L Ms Txt](https://developer.target.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
