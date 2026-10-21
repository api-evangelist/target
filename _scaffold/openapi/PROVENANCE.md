# Provenance — the OpenAPI documents in this directory are API Evangelist scaffolds

**Verified 2026-08-27 by the enrichment pipeline (local-v1). Not published by Target Corporation.**

Every `.yml` in this directory (and in `_original/`) now carries an `x-provenance` block saying the
same thing in machine-readable form. This file is the human-readable version and the evidence table.

## What they are

`openapi/_original/target-target-api-openapi.yml` was written by the API Evangelist **2026-05 profile
sweep** — the same bulk pass that stamped `plans/` and `rate-limits/` in this repo with *"written by
the API Evangelist bulk sweep dated 2026-05-04, not harvested from the provider"*. The six per-tag
documents beside it are the `refine-openapis` split of that one file, so they inherit its provenance
exactly.

They were never harvested from Target, because there is nothing to harvest: `developer.target.com` is
open only to Target team members and third parties with an existing Target relationship, and its
catalog API returns `401 {"message":"Invalid Key"}` to anonymous callers.

## The evidence

Every operation these documents declare was probed against `https://api.target.com` — the host their
own `servers[]` block names — on 2026-08-27:

| Probed URL | Status |
|---|---|
| `https://api.target.com/products/v3` | **404** |
| `https://api.target.com/products/v3/12345` | **404** |
| `https://api.target.com/products/v3/search` | **404** |
| `https://api.target.com/stores/v3` | **404** |
| `https://api.target.com/orders/v1` | **404** |
| `https://api.target.com/status` | **404** |

The 404s are route-absence, not a blanket edge denial. Two control probes against paths Target really
operates prove the gateway distinguishes present from absent:

| Control URL | Status | Meaning |
|---|---|---|
| `https://redsky.target.com/redsky_aggregations/v1/web/pdp_client_v1` | **403** | Real route, exists, gated behind PerimeterX |
| `https://redsky.target.com/v3/pdp/tcin/12345` | **410** | Real route, existed, permanently retired |

Target's live product surface is `redsky.target.com/redsky_aggregations/v1/...`. The
`api.target.com/products/v3/...` shape in these documents does not exist and, on this evidence, never did.

## What this means for the rest of the repo

Per the pipeline's ownership rule, **everything derived from a spec inherits that spec's provenance**.
So the 2026-08-27 enrichment pass deliberately did NOT write:

- `errors/` — an RFC 9457 catalog derived from invented `4xx`/`5xx` responses
- `data-model/` — an entity graph derived from invented `$ref`s
- `skills/` — Agent Skills grounded in `operationId`s that do not resolve
- `overlays/` — an Overlay extending a document that is not Target's
- `mcp/` tool candidates and `mcp/target-tool-crosswalk.yml` — an agent surface built from invented operations

`authentication/target-authentication.yml` previously carried an `http`/`bearer` scheme derived from
these documents. It has been rewritten from Target's two live OpenID Connect discovery documents, and
the old bearer claim is recorded under `unverified_prior_claims` rather than carried forward.

`agentic-access/target-agentic-access.yml` (2026-07-15) is still derived from the scaffold and should
be regarded as describing nothing real.

## What Target actually publishes

| Surface | URL | Status |
|---|---|---|
| llms.txt | `https://www.target.com/llms.txt` | 200, `text/plain`, well formed |
| OIDC discovery (corporate) | `https://oauth.iam.target.com/.well-known/openid-configuration` | 200 |
| OIDC discovery (suppliers) | `https://oauth.iam.partnersonline.com/.well-known/openid-configuration` | 200 |
| JWKS | `https://oauth.iam.target.com/openid/connect/jwks.json` | 200 |
| Vulnerability disclosure policy | `https://security.target.com/vdp/` | 200, with safe harbour |
| OAuth service Swagger (advertised by Target's own discovery doc) | `https://oauth.iam.target.com/apidocs/auth/oauth/v2/swagger` | **404** |

That last row is the finding worth taking back to Target: their own discovery document points at a
machine-readable OAuth contract that they do not serve. Restoring it would give Target a real,
first-party, fetchable API contract with no other work.

## Recommended remediation

Follow the worked example in `all/meditech/`: quarantine these files to `openapi/_scaffold/` with this
README, and correct `accessModel` to `pricing: unknown` / `onboarding: request`. That is a
network-wide pass and a human decision, so this round stopped at stamping and evidencing rather than
moving files.
