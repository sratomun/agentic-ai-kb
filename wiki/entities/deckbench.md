---
type: entity
entity_type: benchmark
tags: [agents, benchmark, content-generation, summarization, evaluation]
created: 2026-06-22
updated: 2026-06-22
---

# DECKBench

*A benchmark for multi-agent academic slide generation and editing — formalizing faithfulness vs. fidelity for generative content.*

## What it is
DECKBench (Jang et al., KDD '26) is an eval suite for multi-agent slide generation: 294 paper–slide pairs, 5 multi-turn editing rounds, and a simulated user agent. It operationalizes Faithfulness (anti-hallucination) and Fidelity (coverage) as distinct metrics.

## Why it matters
Generative content agents — for decks, reports, and documents — are among the most deployable near-term enterprise tools. DECKBench's faithfulness/fidelity split is a reusable eval template for any content-generation agent deployment.

## Relationships
- evaluates [[agent-evaluation]]
- stresses [[multi-agent-systems]]
- relates to [[llm-as-judge]]

## Cited by
- [[2026-02-10-arxiv-2602-13318v1-deckbench-slide-generation]]
