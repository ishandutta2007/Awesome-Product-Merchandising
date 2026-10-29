# Awesome-Product-Merchandising

# Top Product Merchandising Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Searchandising, Product Discovery & Self-Hosted Merchandising Engines*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Product Merchandising**. These tools enable ecommerce teams to control product ranking, curate category pages, apply boost-and-bury rules, and personalize product discovery—turning the catalog into a strategic lever for conversion and margin.

**Examples** include Shopify Combined Listings, Searchspring, Algolia, Klevu, Bloomreach, Attraqt, Nosto, Constructor.io, Syte, and Fast Simon (the category leaders).

**Open-source emphasis**: Product Merchandising is a domain where open-source tooling is **emerging but still catching up to commercial searchandising suites**. The strongest active project is **ElasticSuite (Gally)**, an open-source searchandising engine for Magento, Shopware, Sylius, and OroCommerce with vector search, virtual categories, and boost-and-bury rules . **PragmaSearch** provides a local-first semantic search engine with synonym and ranking rule support, explicitly positioned as a low-cost Algolia alternative for small-to-mid catalogs . **Typesense** offers a fast, typo-tolerant search engine with vector search and merchandising-friendly features . However, no open-source project matches the full enterprise merchandising workflow (A/B testing, behavioral learning, automated campaigns) of Searchspring or Constructor.io out of the box.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Shopify Combined Listings](https://help.shopify.com/en/manual/products/combined-listings)**  
  Shopify's native product merchandising feature for grouping related product variants (e.g., same shirt in different colors) into a single listing; improves discovery and simplifies catalog management for merchants.

- **[Searchspring](https://searchspring.com/)**  
  Generative Discovery platform with ML-powered merchandising: specific sorting, boost/bury logic, pinning, triggered and scheduled banners, A/B testing, and personalized recommendations; praised by merchandising-heavy teams for category control and testing capabilities .

- **[Algolia](https://www.algolia.com/)**  
  AI-powered search and discovery platform with instant search, typo tolerance, and vector search; strong for developer-led merchandising with custom ranking rules, synonyms, and InstantSearch UI libraries .

- **[Klevu (Athos Commerce)](https://athoscommerce.com/klevu-search-platform/)**  
  AI search and discovery platform now integrated into Athos Commerce; provides NLP-based relevance, visual merchandising with pinning/boosting/exclusions, real-time personalization, and recommendations.

- **[Bloomreach](https://www.bloomreach.com/)**  
  Discovery platform with modular feature packages for Search, Categories, and merchandising; AI tools include conversational agents, Premium Search with optimized ranking, and visual search .

- **[Attraqt](https://www.attraqt.com/)**  
  Product discovery and merchandising platform with AI-powered search, personalization, and merchandising controls for enterprise retailers.

- **[Nosto](https://www.nosto.com/)**  
  AI-powered search and discovery with semantic search, predictive autocomplete, personalized search, synonym optimization, faceting, A/B testing, and analytics.

- **[Constructor.io](https://constructor.io/)**  
  AI-powered search and product discovery with Searchandising Campaigns for applying merchandising strategies across multiple search, category, and facet contexts; features bulk rule application and facet group curation.

- **[Syte](https://www.syte.ai/)**  
  Visual AI product discovery platform with visual search, automated product tagging, and personalized recommendations.

- **[Fast Simon](https://www.fastsimon.com/)**  
  Visual product discovery platform with SDK for visual search, discovery image galleries, and related product recommendations.

## Open-Source GitHub Projects

- **[ElasticSuite (Gally)](https://github.com/elasticsuite/elasticsuite)**  
  The most mature open-source **searchandising** platform available; designed for B2B and B2C ecommerce with advanced search, merchandising, and personalization . Gally, its searchandising engine, integrates natively with **Magento, Shopware, Sylius, and OroCommerce** to provide smart search with natural language understanding, typo tolerance, **virtual categories**, **boost-and-bury rules**, and merchandising analytics . Merchandisers can control product display order based on margins, stock, promotions, or seasonality without writing code . **The closest open-source equivalent to Searchspring or Klevu** for platform-native merchandising, though it requires one of the supported ecommerce platforms.

- **[PragmaSearch](https://www.npmjs.com/package/pragmasearch)**  
  Free, self-hosted semantic search engine positioned as an **open-source, local-first Algolia alternative** . Combines vector search and BM25 keyword search into hybrid ranking with **Reciprocal Rank Fusion**, typo tolerance, faceted filtering, and multilingual support. Includes **synonyms and ranking rules (boost/bury/pin)** and analytics (top/zero-result queries) with a bundled benchmark showing nDCG@10 of 0.941 for hybrid mode . **Explicitly designed for small-to-mid catalogs (≤ ~50k items)**; the author notes hosted platforms still win for million-SKU real-time catalogs with deep A/B testing . **The most accessible open-source merchandising engine** for teams migrating off hosted search.

- **[Typesense](https://github.com/typesense/typesense)**  
  Fast, typo-tolerant open-source search engine (GPL-3.0) written in C++; a single-binary alternative to Algolia . Serves a REST API with sub-50ms query latency, built-in typo correction, **faceting, filtering, sorting, synonym handling**, geo search, and **vector search (HNSW)** . While not a full merchandising suite, Typesense provides the search primitives (synonyms, ranking, filtering) needed to build merchandising workflows; it is drop-in for applications currently calling Algolia or Elasticsearch with no per-query fees .

- **[Marqo](https://github.com/marqo-ai/marqo)**  
  AI-native search and product discovery platform that is **self-hostable and maintained by the open-source community** . Leverages semantic search, LLMs, and behavioral learning for relevance, typo tolerance, multilingual queries, and **automated merchandising workflows** . Positioned for enterprise-scale retailers wanting self-hosted AI search with merchandising automation.

- **[OmniSearch](https://pypi.org/project/syeedalireza-omnisearch/)**  
  AI-powered ecommerce search engine using vector databases (Qdrant/Milvus) and HuggingFace Transformers (Sentence-BERT, CLIP) for **natural language and image search** . **Early-stage (v1.0.1, 28 weekly downloads) with technical implementation pending**—demonstrates the semantic/visual product discovery pattern but is not production-ready .

### Additional Strong Open-Source Options

- **searchrec** — Lightweight ecommerce recommendation engine based on item-item collaborative filtering; tracks click sessions and serves "you may also like" recommendations with an admin dashboard . **Recommendation-focused** rather than search merchandising, but useful for personalization.
- **VisualMatch** — AI-powered visual product search engine using OpenAI CLIP; matches user-uploaded photos against a catalog with <100ms latency and includes an Instagram DM bot . **Visual search niche** rather than general merchandising.

**Frameworks for building custom systems**: **ElasticSuite (Gally)** provides the most complete open-source searchandising platform for supported ecommerce platforms (Magento, Shopware, Sylius, OroCommerce) . **PragmaSearch** provides a lightweight, Algolia-like semantic search engine with merchandising rules for small-to-mid catalogs . **Typesense** provides the search infrastructure primitives (synonyms, faceting, vector search) for custom builds . **Marqo** offers self-hosted AI-native search with automated merchandising . No open-source project matches the full enterprise merchandising suite (A/B testing, behavioral learning at scale, automated campaigns) of Searchspring or Constructor.io.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Product merchandising platforms handling shopper behavior and catalog data must comply with applicable privacy regulations and ecommerce requirements; search analytics and personalization data require careful governance.
- **Open-source product merchandising is emerging but not turnkey**—ElasticSuite provides strong platform-native searchandising for supported ecommerce systems , PragmaSearch offers a compelling Algolia alternative for smaller catalogs , and Typesense/Marqo provide search infrastructure. However, no open-source project matches the full enterprise merchandising workflow (A/B testing, behavioral learning at scale, automated campaigns) of Searchspring or Constructor.io. Organizations requiring advanced merchandising automation should evaluate commercial platforms.
- Verify license terms for commercial use; ElasticSuite is open-source , PragmaSearch is an npm package , and Typesense uses GPL-3.0 .

---

**Made for ecommerce merchandisers, search managers, category managers, and product discovery engineers.**  
Let's make product merchandising more open, but with clear eyes about the enterprise automation gap that remains.
