---
type: entity
entity_type: benchmark
tags: [agents, benchmark, nlu]
created: 2026-06-23
updated: 2026-06-23
---

# CLINC150

*Standard intent-classification benchmark with built-in out-of-scope queries (150 intents across 10 domains).*

## What it is
CLINC150 (Larson et al., 2019) is the canonical dataset for intent classification *and* out-of-scope detection, designed to test whether systems can refuse queries outside their intent set.

## Why it matters
The yardstick for the component view of [[intent-understanding]] — and still used to stress-test modern routers (e.g. Arch-Router). OOS handling is the production pain point it captures.

## Relationships
- benchmark for [[intent-understanding]]
- used by [[arch-router]]
- companion to [[banking77]] · [[multiwoz]]

## Cited by
- [[2024-10-02-arxiv-2410-01627-intent-detection-in-the-age-of-llms]]
- [[2025-06-19-arxiv-2506-16655-arch-router-aligning-llm-routing-with-human-preferences]]
