---
type: source
source_type: analysis
kind: decision-note
title: "OKF adoption assessment for the AI Tech Radar"
authors: Sage
date: 2026-06-22
ingested: 2026-06-22
tags: [analysis, standard, knowledge-graph, decision]
---

# OKF adoption assessment

**Decision note** · 2026-06-22 · re: adopting [[open-knowledge-format|OKF]] for this wiki

**Decision:** adopt via **export**, not in-place rewrite. Keep authoring in Obsidian; emit a conformant OKF bundle on demand.

## How conformant we already are
The radar is ~90% an OKF bundle by design. Against OKF v0.1's hard conformance rules:

| OKF requirement | This wiki | Status |
|---|---|---|
| Directory of `.md` + YAML frontmatter | yes | ✅ |
| Non-empty `type` on every concept file | `type: concept\|entity\|source` everywhere | ✅ |
| Reserved `index.md` + `log.md` present & structured | both present (formatting differs) | ◑ |
| Edges = standard markdown links | Obsidian wikilinks | ❌ gap |
| `resource`, `timestamp` (recommended) | `url`, `updated`/`date` | ◑ aliasable |

## The one real gap
OKF edges are markdown links (`[x](/path.md)`); ours are Obsidian wikilinks. Converting in place would degrade Obsidian's native graph/backlinks and authoring ergonomics, so we **bridge with an export** instead.

## What we did
1. **Imported** OKF + the [[llm-wiki]] pattern as first-class nodes (self-documenting the methodology).
2. **Aligned in place** where safe — confirmed `type` on every node (the only hard requirement we don't get for free is links).
3. **Built `okf-export`** in the kg-curator skill (`/Skills/kg-curator/`): wikilinks→bundle-relative markdown links, `url`→`resource`, `updated`→`timestamp`, OKF-shaped `index.md` per directory + root (`okf_version: "0.1"`), newest-first `log.md`. Output is a verifiably conformant bundle; the Obsidian source is untouched.

## Why not full in-place conformance now
v0.1 is single-vendor ("an invitation, not yet a standard") with a paid serving layer ([[knowledge-catalog]]) behind it. The export is cheap insurance with zero disruption; revisit in-place conformance if OKF gains non-Google adoption.

## Graph
- **Entities:** [[open-knowledge-format]] · [[knowledge-catalog]] · [[mcp]]
- **Concepts:** [[llm-wiki]]
