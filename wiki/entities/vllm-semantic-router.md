---
type: entity
entity_type: product
tags: [agents, product, routing, open-source]
created: 2026-06-23
updated: 2026-06-23
---

# vLLM Semantic Router

*System-level intelligent router for mixture-of-models across cloud, data center, and edge.*

## What it is
An open-source project (vllm-project) doing signal-driven request routing for mixture-of-model serving, with releases through early 2026 (v0.2, March 2026).

## Why it matters
The infrastructure-grade expression of intent routing: classify each request and serve it from the right model, with semantic caching to short-circuit repeats. Tracks where the serving layer is heading.

## Relationships
- infrastructure for [[intent-routing]]
- peer of [[semantic-router]] · [[arch-router]]
- relates to [[mixture-of-experts]] serving

## Cited by
- [[intent-routing]]
