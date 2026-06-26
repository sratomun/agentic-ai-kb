# AI Tech Radar — Agentic-AI knowledge wiki

A self-maintaining knowledge graph on agentic AI, compiled from technical
literature, blog posts, and industry/consulting papers. Scanners pull sources in;
they're compiled into an interlinked wiki that compounds over time. It follows the
Karpathy "LLM-wiki" pattern and is an Obsidian vault, so wikilinks and graph view
work natively.

It serves a senior AI/tech exec persona — signal over textbook: what's genuinely
new, why it matters, and the "so what." Voice and node-quality rules live in
[`wiki/_templates/STYLE.md`](wiki/_templates/STYLE.md); architecture and operating
conventions live in [`CLAUDE.md`](CLAUDE.md).

## Layout

| Path | What it holds |
|------|----------------|
| `raw/` | Immutable source captures — `raw/arxiv/`, `raw/blogs/`, `raw/news/`, plus per-year censuses. Scanners only ever ADD here; never edited. Not part of the graph. |
| `wiki/` | The maintained graph: `concepts/`, `entities/`, `sources/`, `comparisons/`, `overview.md`, and `_templates/` (node structures + style guide). |
| `index.md` | Catalog of every wiki page — read first, then drill in. |
| `log.md` | Append-only timeline of every ingest / lint pass. |
| `CLAUDE.md` | The schema: architecture, ingest/query/lint operations, graph-density rules. |
| `scanners.md` | Source list + agents-centric focus filter the scanners read. |
| `skills/` | The automations — `arxiv-scanner/`, `blog-scanner/`, `kg-curator/` (see `skills/README.md`). |
| `briefings/` · `trackers/` · `radar-notes/` | On-demand exec deliverables, one doc type per folder (created on first use). |

## Three ingest tiers (coverage → depth)

1. **Census** — every matching paper as metadata in `raw/arxiv/<year>-census/`. Exhaustive, not in the graph.
2. **Browsable** — abstract-only auto-notes in `wiki/sources/<year>-census/`, keyword-linked, filtered out of the global graph view.
3. **Deep** — full-text reads with analysis (`depth: full-text`), first-class graph nodes.

## How it works

Three scanners feed the graph, each a different layer of truth: **arXiv** = *what's
true* (research), **news** = *what happened* (events), **blogs** = *what it means /
who thinks what* (attributed opinion + debates). After a scan, the **ingest**
operation writes/refreshes source notes, integrates findings into the relevant
concept/entity pages (no duplicates; contradictions flagged inline), promotes
node-worthy references to their own linked nodes, then updates `index.md` and
appends to `log.md`. The **kg-curator** skill periodically tends the graph — mining
new nodes, enriching citation-ranked sections, normalizing to templates, and linting
for orphans, broken links, and stale framing.

Two other operations: **query** (answer from the graph with citations to the pages
used; file durable answers back as new pages) and **lint** (health-check: contradictions,
stale claims, orphans, missing cross-references).

## Conventions

Kebab-case filename slugs; Obsidian `[[slug|Display]]` wikilinks (the links *are* the
graph). Every node has ≥1 inbound and ≥1 outbound link — no orphans — and every
relationship is reciprocal (back-link on both ends). Concept and entity pages are
synthesized, compounding articles grounded in full text, not abstracts; source notes
are one per ingested item. Full node structure and style are in `wiki/_templates/`.

## Current size

57 concepts · 157 entities · ~1,700 source notes · 2025 + 2026 agents-centric
censuses (~23k paper records). See `index.md` for the live catalog and `log.md` for
the running history.
