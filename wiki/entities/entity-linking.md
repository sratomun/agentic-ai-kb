---
type: entity
entity_type: method
tags: [agents, method, nlu, knowledge-graph]
created: 2026-06-23
updated: 2026-06-23
---

# Entity linking

*Mapping ambiguous text mentions to canonical entities in a knowledge base — the binding step that grounds intent into a structure.*

## What it is
Entity linking (EL) aligns surface mentions ("Apple", "the Seattle support team") with the right node in a knowledge base or graph. Modern EL is increasingly zero-shot and KG-triple-enhanced, no fine-tuning required.

## Why it matters
EL is the mechanism by which fuzzy user language gets pinned to the semantic layer — the disambiguation primitive under [[intent-grounding]]. Without it, the structure can't be reached.

## Relationships
- primitive of [[intent-grounding]]
- operates over [[knowledge-graph]]
- exemplified by [[2026-01-08-arxiv-2601-05192-lela-zero-shot-entity-linking|LELA]] · [[2025-04-21-arxiv-2504-15135-kgmel-kg-enhanced-multimodal-entity-linking|KGMEL]]

## Cited by
- [[2026-01-08-arxiv-2601-05192-lela-zero-shot-entity-linking]]
- [[2025-04-21-arxiv-2504-15135-kgmel-kg-enhanced-multimodal-entity-linking]]
