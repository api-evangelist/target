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
- **Modified:** 2026-10-21

## APIs

### Target Redsky API

Redsky is Target's internal aggregation API platform, described by Target's engineering team on tech.target.com, that turns GraphQL queries into client-managed REST APIs serving product, price, promotion and fulfillment data to Target.com and Target's mobile apps. It is internal infrastructure: Target does not license it to third parties.

- **Human URL:** [https://tech.target.com/blog/empowering-clients-api](https://tech.target.com/blog/empowering-clients-api)
- [GraphQL notes](graphql/target-graphql.md)

### Target Partner API

Target runs a partner-gated developer program at developer.target.com, open to Target team members and third parties with an existing Target relationship. Access is by partner onboarding.

- **Human URL:** [https://developer.target.com/](https://developer.target.com/)

## Not published by Target

Honestly absent — recorded here so their absence is not mistaken for an oversight:

- No public API reference, base URL, or machine-readable OpenAPI for the partner program
- No public contract for Redsky, which is internal and not licensed to third parties
- No public API pricing or plan tiers
- No published rate limits

Earlier scaffold OpenAPIs (written by an API Evangelist sweep without a Target source; every path returned 404 on api.target.com) and every artifact derived from them were moved to [`_scaffold/`](_scaffold/README.md) on 2026-10-21. They are not Target's and are not part of this profile.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/target)
- [Website](https://www.target.com)
- [Developer Portal](https://developer.target.com/)
- [Blog](https://tech.target.com)
- [GitHub Org](https://github.com/target)
- [Open Source](https://tech.target.com/open-source)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
