# RAW — Introducing the Open Knowledge Format (Google Cloud Blog)

Source: https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing
Authors: Sam McVeety, Amir Hormati (Google Cloud Data Cloud team) · 2026-06-12
Spec: https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md (Apache-2.0)

Key points (captured 2026-06-22):

- OKF is an open specification that formalizes the Karpathy LLM-wiki pattern into a
  portable, vendor-neutral, agent- and human-friendly format for the metadata,
  context, and curated knowledge AI systems need.
- OKF v0.1 = a directory ("bundle") of markdown files with YAML frontmatter, with a
  small set of agreed conventions so wikis written by different producers can be
  consumed by different agents without translation. "Just markdown, just files, just
  YAML frontmatter."
- Structured frontmatter fields that need to be queryable: type, title, description,
  resource, tags, timestamp. Only `type` is required.
- Concepts link to each other with normal markdown links → the directory is a graph.
  Optional reserved files: index.md (progressive disclosure) and log.md (history).
- Full v0.1 spec fits on one page (~451 lines). Three design principles: minimally
  opinionated (only `type` required), producer/consumer independence, format-not-platform.
- Reference implementations: a BigQuery enrichment agent (Gemini + ADK), a static
  self-contained HTML visualizer (Cytoscape.js + marked.js), `kcmd` CLI + MCP server,
  and three sample bundles (GA4 e-commerce, Stack Overflow, Bitcoin).
- Complements MCP (MCP = access to tools/data; OKF = the knowledge itself). Google
  Cloud Knowledge Catalog updated to ingest OKF and serve it to its agents.
- Repo: github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf
- Caveat: at launch every producer/consumer was Google's; "a starting point, not a
  finished standard."
