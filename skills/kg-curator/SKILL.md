---
name: kg-curator
description: Curate and maintain the exec's AI Tech Radar knowledge graph — the librarian for the wiki. Mines the census for new concept/entity nodes, promotes recurring references to nodes, enriches hubs with citation-ranked papers, normalizes nodes to the templates, and lints the graph for integrity. Use when the exec says "curate the wiki", "tidy the graph", "mine for concepts", "normalize the nodes", "lint the graph", "health-check the radar", or "fix orphans/broken links".
---

> Lives in `/Skills/kg-curator/`. Reads/writes the wiki under `../../`.
> The scanners (`arxiv-scanner`, `news-scanner`) *create* nodes; this skill *tends*
> them.

# KG Curator

The maintenance counterpart to the scanners. It keeps the graph consistent, dense,
and honest over time. Always conform to the **source of truth**:
`../../wiki/_templates/STYLE.md` (voice + rules) and the
`_templates/*.md` (structure). Read those first.

## Triggers
"curate the wiki", "tidy the graph", "mine for concepts/entities", "normalize the
nodes", "lint the graph", "health-check the radar", "fix orphans", "fix broken links".

## Operations (run the ones asked for; default = lint)

### mine — find missing concepts & entities
1. Frequency-scan the census (`raw/arxiv/<year>-census/census-<year>.jsonl`) for
   recurring sub-themes (concept candidates) and recurring named systems / models /
   benchmarks / methods / orgs (entity candidates).
2. Drop any that already exist (check `wiki/concepts/`, `wiki/entities/`, and aliases).
3. **Frequency-justify** (per STYLE): propose only candidates the corpus supports;
   prefer folding thin sub-themes into a parent's `## Includes` over a stub node.
4. On approval, create nodes from `_templates/concept-node.md` / `entity-node.md`,
   with reciprocal links on both ends and ≥1 inbound + ≥1 outbound each.

### promote — turn references into nodes
For node-worthy names that appear across multiple source notes but aren't yet nodes,
create the entity node and add reciprocal `## Cited by` ↔ source-note links.

### enrich — refresh citation-backed sections
1. Ensure citations exist (run `arxiv-scanner` citation mode if not).
2. Rebuild each node's `## Key papers (citation-ranked)` / `## Cited by` from the
   citation data (top-N by citations; model-reports excluded for concept hubs).
3. Where a hub's synthesis is thin or year-skewed, integrate findings from the **full
   text** of the anchor papers (`raw/arxiv/<id>.fulltext.md`) into
   `## What the evidence shows` — braid foundations + recent (per STYLE). Never from
   abstracts.

### normalize — conform a node to the standard
Bring a node (or a batch) to the current template + STYLE: add the `*one-liner*`,
`What it is` / `Why it matters` / evidence structure; retire year-stamped framing;
fix titles that name folded-out sub-hubs; preserve all links and existing sections.

### okf-export — emit a conformant Open Knowledge Format bundle
Produce a portable [[Open Knowledge Format]]-conformant copy of the wiki without
touching the Obsidian source (we author in wikilinks; OKF wants markdown-link edges).
1. Mirror `wiki/**` (minus `_templates/`) into a bundle dir / tarball.
2. Rewrite each `[[slug]]` / `[[slug|Display]]` → `[Display](/bundle/relative/path.md)`
   (bundle-relative absolute form; unresolved targets degrade to plain text, not broken
   edges). Guarantee `type` on every file; alias `url`→`resource`, `updated`/`date`→
   `timestamp`.
3. Generate OKF `index.md` per directory (no frontmatter except the bundle root, which
   declares `okf_version: "0.1"`) and a newest-first `log.md`.
4. **Verify conformance (OKF v0.1 §9):** every non-reserved `.md` has parseable
   frontmatter + non-empty `type`; reserved files structured; report markdown-edge and
   broken-link counts; confirm zero `[[wikilinks]]` remain.
Output is a build artifact (ship as a tarball) — keep it OUT of the vault/graph.

### lint — integrity pass (default)
Scan `wiki/**` + `index.md` (exclude `wiki/_templates/` and the graph-filtered
leaf folders). Report and fix:
- broken `[[links]]` (→ 0)
- orphans — nodes with 0 inbound or 0 outbound (→ 0; wire them in)
- duplicate sections (e.g. two `## Key papers`)
- stale year-stamped headers ("Threads (2026)", "2026 cohort additions")
- citation lists out of date
- mis-tag spot-check on the highest-cited papers
Append a one-line `## [YYYY-MM-DD] lint | <summary>` to `../../log.md`.

## Notes
- Drafts/notes only — never emails or posts.
- Don't silently rewrite history: report fixes, log them.
- Citation lists are machine-maintained; fix the data/curator, not by hand.
