---
type: source
source_type: arxiv
title: "Atomix: Timely, Transactional Tool Use for Reliable Agentic Workflows"
authors: Bardia Mohammadi, Nearchos Potamitis, Lars Klein, Akhil Arora et al.
url: https://arxiv.org/abs/2602.14849v2
date: 2026-02-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.LG
tags: [agent-reliability, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Atomix: Timely, Transactional Tool Use for Reliable Agentic Workflows

**arXiv:** [2602.14849v2](https://arxiv.org/abs/2602.14849v2) · 2026-02-16 · cs.LG
**Authors:** Bardia Mohammadi, Nearchos Potamitis, Lars Klein, Akhil Arora et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM agents execute multi-step workflows that mutate external state through tools. Common orchestrators treat tool return as the settlement trigger, so faults, speculation, and concurrent agents can leave partial effects, losing-branch residue, stale writes, or irreversible sends. Correct settlement needs two facts that retries, checkpoint replay, locks, and compensation each conflate: which effects must settle together, and when earlier conflicting work is exhausted. Atomix makes this split explicit with progress-aware transactions. The runtime records reads and effects during execution, seals a transaction when its footprint is complete, and commits only after per-resource frontiers show that no earlier conflicting work can still arrive. Commit is final settlement: Atomix releases bufferable effects, accepts reversible external effects as final, and lets irreversible effects leave the gate. Abort suppresses unreleased effects and compensates externalized reversible effects where possible. On representative agent workloads, this composition improves clean recovery under injected faults, isolates contending and speculative work, and prevents correctly classified irreversible actions from leaking; microbenchmarks show microsecond-scale wrapper overhead relative to tool latency.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.14849v2)
