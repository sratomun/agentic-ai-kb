---
type: source
source_type: arxiv
title: "Short-Term-to-Long-Term Memory Transfer for Knowledge Graphs under Partial Observability"
authors: Taewoon Kim, Vincent François-Lavet, Michael Cochez
url: https://arxiv.org/abs/2605.22142v2
date: 2026-05-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.LG
tags: [embodied-agents, knowledge-graph, agent-reliability, agentic-rl, agent-memory, arxiv, auto-ingested]
---

# Short-Term-to-Long-Term Memory Transfer for Knowledge Graphs under Partial Observability

**arXiv:** [2605.22142v2](https://arxiv.org/abs/2605.22142v2) · 2026-05-21 · cs.LG
**Authors:** Taewoon Kim, Vincent François-Lavet, Michael Cochez

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement learning under partial observability requires deciding what information to retain, yet most memory-based approaches do not explicitly model short-term-to-long-term transfer of symbolic observations. We study this transfer process in a temporal knowledge-graph memory setting and cast it as a neuro-symbolic value-based decision problem: for each observed triple, the agent chooses whether to keep or drop it before long-term insertion. To handle variable-sized short-term buffers, we use a per-item Q-learning design with shared parameters and a practical temporal-difference update over matched items across consecutive steps. On the RoomKG benchmark at long-term memory capacity 128, learned transfer decisions outperform symbolic and neural baselines, including symbolic baselines with temporal annotations and history-based LSTM/Transformer baselines. Across transfer-policy ablations, a lightweight local short-term-only variant performs best, and step-level behavior shows that the policy keeps navigation- and query-relevant facts while discarding lower-value candidate facts, supporting explicit and interpretable memory decisions under memory constraints.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.22142v2)
