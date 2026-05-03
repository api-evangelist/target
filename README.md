# Target

Target Corporation is one of the largest retailers in the United States, offering a wide assortment of general merchandise and food through more than 1,900 stores and digital channels. Target's technology platform powers partner integrations, internal services, and open-source tooling across their retail operations.

**Website:** [https://www.target.com](https://www.target.com)
**Developer Portal:** [https://developer.target.com/](https://developer.target.com/)
**Tech Blog:** [https://tech.target.com](https://tech.target.com)
**GitHub:** [https://github.com/target](https://github.com/target)

## APIs

### Target API
Partner APIs for product catalog access, inventory availability, order management, and store information. Enables technology partners and affiliates to integrate with Target's retail platform.

- **Base URL:** https://api.target.com
- **Auth:** Bearer token
- **Docs:** [https://developer.target.com/](https://developer.target.com/)

### Target Redsky API
Target's internal aggregation API platform that converts GraphQL queries into client-managed REST APIs. Serves product data, pricing, promotions, and fulfillment information for Target.com and mobile applications, managing 200+ unique APIs across 30 clients.

- **Base URL:** https://redsky.target.com
- **Docs:** [https://tech.target.com/blog/empowering-clients-api](https://tech.target.com/blog/empowering-clients-api)

## Artifacts

### OpenAPI Specifications
| API | File |
|-----|------|
| Target API | [openapi/target-target-api-openapi.yml](openapi/target-target-api-openapi.yml) |

### JSON Schemas
| Schema | File |
|--------|------|
| Target Product | [json-schema/target-product-schema.json](json-schema/target-product-schema.json) |
| Target Store | [json-schema/target-store-schema.json](json-schema/target-store-schema.json) |

### JSON Structure
| Structure | File |
|-----------|------|
| Product Structure | [json-structure/target-product-structure.json](json-structure/target-product-structure.json) |

### JSON-LD Context
| Context | File |
|---------|------|
| Target Context | [json-ld/target-context.jsonld](json-ld/target-context.jsonld) |

### Spectral Rules
| Ruleset | File |
|---------|------|
| Target API Rules | [rules/target-spectral-rules.yml](rules/target-spectral-rules.yml) |

### Naftiko Capabilities
| Capability | File | Description |
|-----------|------|-------------|
| Retail Integration | [capabilities/retail-integration.yaml](capabilities/retail-integration.yaml) | Unified workflow for product search, inventory, stores, and orders |

**Shared definitions:**
| Definition | File |
|-----------|------|
| Target API | [capabilities/shared/target-api.yaml](capabilities/shared/target-api.yaml) |

### Examples
| Example | File |
|---------|------|
| Get Product | [examples/target-get-product-example.json](examples/target-get-product-example.json) |
| Search Products | [examples/target-search-products-example.json](examples/target-search-products-example.json) |
| List Stores | [examples/target-list-stores-example.json](examples/target-list-stores-example.json) |
| Get Product Fulfillment | [examples/target-get-product-fulfillment-example.json](examples/target-get-product-fulfillment-example.json) |

### Vocabulary
| Vocabulary | File |
|-----------|------|
| Target Vocabulary | [vocabulary/target-vocabulary.yml](vocabulary/target-vocabulary.yml) |

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
