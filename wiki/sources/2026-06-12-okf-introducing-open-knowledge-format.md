---
type: source
source_type: news
kind: reference
title: "Introducing the Open Knowledge Format"
authors: Sam McVeety, Amir Hormati (Google Cloud Data team)
url: https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing
resource: https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md
date: 2026-06-12
ingested: 2026-06-22
tags: [news, standard, knowledge-graph]
---

# Introducing the Open Knowledge Format

**Google Cloud Blog / SPEC.md** · 2026-06-12 · Sam McVeety & Amir Hormati

**Why it matters:** The reference announcement + spec for [[open-knowledge-format|OKF]] — the standard our radar is (almost) already built to.

## What it says
- OKF formalizes the [[llm-wiki|LLM-wiki pattern]] into a portable, vendor-neutral format: a **bundle** = a directory of markdown files with YAML frontmatter, cross-linked into a graph.
- **Only required field: `type`** (producer-defined). Recommended: `title`, `description`, `resource`, `tags`, `timestamp`. Consumers must tolerate unknown types/fields and broken links.
- **Edges are standard markdown links**; bundle-relative absolute form `[x](/path.md)` is recommended. Reserved files: `index.md` (progressive disclosure), `log.md` (history).
- Conventional body sections: `# Schema`, `# Examples`, `# Citations`. Conformance (v0.1) is just: parseable frontmatter + non-empty `type` + reserved-file structure when present.
- Ships with reference tooling: a BigQuery enrichment agent (Gemini/ADK), a self-contained HTML graph **visualizer**, and `kcmd` (CLI + MCP server) syncing to [[knowledge-catalog]].
- Positioned to **complement [[mcp]]**, not compete: MCP = access to tools/data; OKF = the knowledge itself.

## Caveats (from the spec + commentary)
- v0.1 draft, single-vendor; every launch producer/consumer was Google's — "an invitation, not yet a standard."
- The free format drives demand to the paid [[knowledge-catalog]] serving layer.

## Graph
- **Concepts:** [[llm-wiki|LLM wiki]]
- **Entities:** [[open-knowledge-format]] · [[knowledge-catalog]] · [[mcp]]
