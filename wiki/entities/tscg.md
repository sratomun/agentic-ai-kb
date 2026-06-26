---
type: entity
entity_type: method
tags: [agents, method, tool-use, efficiency, schema]
created: 2026-06-21
updated: 2026-06-22
---

# TSCG (Tool-Schema Compilation)

*A deterministic compiler converting JSON tool schemas into token-efficient structured text — no model access, no fine-tuning, ships as a zero-dependency TypeScript package.*

## What it is
TSCG reframes small-model tool-use failure as a representation mismatch rather than a capability gap. It converts JSON tool schemas into structured text at the API boundary — restoring Phi-4 14B from 0%→84.4% accuracy at 20 tools with 52–57% token savings, without touching the model.

## Why it matters
If tool-use failure is a representation problem rather than a size problem, cheap on-prem models become viable for enterprise tool-calling — a significant cost and data-residency win for any organization that can't run frontier APIs due to compliance constraints.

## Relationships
- optimizes [[tool-use]] over [[mcp]]
- part of the efficiency thread in [[agent-protocols]]
- benchmarked on [[bfcl]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-05-04-arxiv-2605-04107v1-tscg-tool-schema-compilation]]
