# Quarantined scaffold artifacts — Target

Moved here 2026-10-21 during a provenance review. **These files are not part of the live profile.**

The OpenAPI documents in `openapi/` are **not Target contracts**. They were written by the API
Evangelist 2026-05 profile sweep without any Target source, and every one declares
`x-provenance.method: scaffold` / `published-by-provider: false`:

- `openapi/target-{inventory,orders,products,search,status,stores}-api-openapi.yml` — the six
  `refine-openapis` splits of the sweep's single placeholder
- `openapi/_ae-authored/target-target-api-openapi.yml` — the same placeholder, also marked
  `method: scaffold`; its paths (`/products/v3`, `/stores/v3`, ...) are not evidenced in any public
  Target documentation, and every one probed 404 on `api.target.com` on 2026-08-27
  (see `openapi/PROVENANCE.md` for the probe table)

Everything else here was derived from those placeholders or written by the same sweep, and carries
no independent evidence:

- `collections/` — Postman and Open Collection files generated from the placeholder OpenAPIs
- `examples/`, `json-schema/`, `json-structure/`, `json-ld/`, `vocabulary/` — invented payloads,
  schemas (`$id` on api.target.com) and terms (`developer.target.com/vocab/`) for the same entities
- `agentic-access/` — classified from the placeholder OpenAPI
- `rules/` — Spectral rulesets written against the placeholder
- `plans/`, `rate-limits/`, `finops/` — bulk-sweep tiers, quotas and billing ("not harvested from
  the provider")

Target publishes **no** public API reference and **no** machine-readable specification. Its
developer program at developer.target.com is partner-gated: open to Target team members and third
parties with an existing Target relationship. Redsky, described in Target's engineering blog, is an
internal platform and is not licensed to third parties.

Per the network convention — record what a provider actually publishes and skip what is honestly
absent — the correct state for Target's contracts is **absent**, not scaffolded. Kept rather than
deleted so the pass that produced them can be traced. Do not restore without provider-published
evidence.
