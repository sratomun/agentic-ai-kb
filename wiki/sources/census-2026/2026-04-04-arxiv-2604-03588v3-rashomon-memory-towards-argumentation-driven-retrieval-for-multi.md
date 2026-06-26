---
type: source
source_type: arxiv
title: "Rashomon Memory: Towards Argumentation-Driven Retrieval for Multi-Perspective Agent Memory"
authors: Albert Sadowski, Jarosław A. Chudziak
url: https://arxiv.org/abs/2604.03588v3
date: 2026-04-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.AI
tags: [agent-economies, knowledge-graph, agent-security, agent-memory, arxiv, auto-ingested]
---

# Rashomon Memory: Towards Argumentation-Driven Retrieval for Multi-Perspective Agent Memory

**arXiv:** [2604.03588v3](https://arxiv.org/abs/2604.03588v3) · 2026-04-04 · cs.AI
**Authors:** Albert Sadowski, Jarosław A. Chudziak

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
AI agents operating over extended time horizons accumulate experiences that serve multiple concurrent goals, and must often maintain conflicting interpretations of the same events. A concession during a client negotiation encodes as a ``trust-building investment'' for one strategic goal and a ``contractual liability'' for another. Current memory architectures assume a single correct encoding, or at best support multiple views over unified storage. We propose Rashomon Memory: an architecture where parallel goal-conditioned agents encode experiences according to their priorities and negotiate at query time through argumentation. Each perspective maintains its own ontology and knowledge graph. At retrieval, perspectives propose interpretations, critique each other's proposals using asymmetric domain knowledge, and Dung's argumentation semantics determines which proposals survive. The resulting attack graph is itself an explanation: it records which interpretation was selected, which alternatives were considered, and on what grounds they were rejected. We present a proof-of-concept showing that retrieval modes (selection, composition, conflict surfacing) emerge from attack graph topology, and that the conflict surfacing mode, where the system reports genuine disagreement rather than forcing resolution, lets decision-makers see the underlying interpretive conflict directly.

## Graph
- **Concepts:** [[agent-economies|Agent economies]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.03588v3)
