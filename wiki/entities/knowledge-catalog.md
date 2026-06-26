---
type: entity
entity_type: product
aliases: [Google Cloud Knowledge Catalog]
tags: [agents, product, knowledge-graph, google]
created: 2026-06-22
updated: 2026-06-22
resource: https://cloud.google.com/blog/products/data-analytics/introducing-the-google-cloud-knowledge-catalog
---

# Google Cloud Knowledge Catalog

*Google Cloud's managed catalog that ingests and serves [[open-knowledge-format|OKF]] bundles to its agents — the paid serving layer behind the free format.*

## What it is
A Google Cloud product (updated Jun 2026) that can ingest OKF bundles and serve the curated knowledge to AI agents, with a `kcmd` CLI + MCP server for bidirectional sync between local OKF files and the catalog.

## Why it matters
It's the commercial shape of OKF worth noting: Google gives away the cheap part (a markdown file any editor can open) and points the demand it creates toward the part it sells. Not a knock — open formats with a paid serving layer have a long track record — but a reason OKF's neutrality is "trust but verify."

## Relationships
- serves [[open-knowledge-format]]
- exposes bundles via [[mcp]]
- made by [[google]]
