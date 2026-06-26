---
type: entity
entity_type: standard
aliases: [OKF, Open Knowledge Format]
tags: [agents, standard, knowledge-graph, interoperability]
created: 2026-06-22
updated: 2026-06-22
resource: https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf
---

# Open Knowledge Format (OKF)

*Google Cloud's open spec (v0.1, Jun 2026) for representing curated knowledge as a directory of Markdown files with YAML frontmatter — the [[llm-wiki|LLM-wiki pattern]] turned into a standard.*

## What it is
An Apache-2.0 specification that pins down the *minimal* conventions needed to make a markdown knowledge base portable and agent-readable: a **bundle** is a directory of markdown "concept" files; the only required frontmatter field is `type`; relationships are standard markdown links; `index.md` (progressive disclosure) and `log.md` (history) are reserved. It is a **format, not a platform** — no SDK, no runtime, no account. It *complements* [[mcp]] (MCP governs access to tools/data; OKF describes the knowledge itself).

## Why it matters
This is the standardized version of exactly how this radar is built — and its arrival means our wiki can become consumable by any OKF-speaking agent or viewer with no bespoke integration. Concretely: our nodes already meet OKF's only hard requirements (frontmatter + non-empty `type`); the one gap is that we use Obsidian wikilinks where OKF wants markdown-link edges, which we bridge with an export rather than disrupting authoring (see [[2026-06-22-okf-adoption-assessment]]). Caveat: v0.1 is single-vendor (every launch producer/consumer was Google's) — "an invitation, not yet a standard," with a paid serving layer ([[knowledge-catalog]]) behind the free format.

## Relationships
- formalizes [[llm-wiki]] (the Karpathy pattern)
- complements [[mcp]]; sits in the [[agent-protocols]] interoperability family
- describes structures for [[knowledge-graph]]
- served by [[knowledge-catalog]] (Google Cloud's paid layer)
- a capability standard for [[agentic-ai]]

## Cited by
- [[2026-06-12-okf-introducing-open-knowledge-format]]
- [[2026-06-22-okf-adoption-assessment]]
