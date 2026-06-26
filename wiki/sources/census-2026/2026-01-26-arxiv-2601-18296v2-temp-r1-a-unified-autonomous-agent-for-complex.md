---
type: source
source_type: arxiv
title: "Temp-R1: A Unified Autonomous Agent for Complex Temporal KGQA via Reverse Curriculum Reinforcement Learning"
authors: Zhaoyan Gong, Zhiqiang Liu, Songze Li, Xiaoke Guo et al.
url: https://arxiv.org/abs/2601.18296v2
date: 2026-01-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.CL
tags: [knowledge-graph, agentic-rl, arxiv, auto-ingested]
---

# Temp-R1: A Unified Autonomous Agent for Complex Temporal KGQA via Reverse Curriculum Reinforcement Learning

**arXiv:** [2601.18296v2](https://arxiv.org/abs/2601.18296v2) · 2026-01-26 · cs.CL
**Authors:** Zhaoyan Gong, Zhiqiang Liu, Songze Li, Xiaoke Guo et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Temporal Knowledge Graph Question Answering (TKGQA) is inherently challenging, as it requires sophisticated reasoning over dynamic facts with multi-hop dependencies and complex temporal constraints. Existing methods rely on fixed workflows and expensive closed-source APIs, limiting flexibility and scalability. We propose Temp-R1, the first autonomous end-to-end agent for TKGQA trained through reinforcement learning. To address cognitive overload in single-action reasoning, we expand the action space with specialized internal actions alongside external action. To prevent shortcut learning on simple questions, we introduce reverse curriculum learning that trains on difficult questions first, forcing the development of sophisticated reasoning before transferring to easier cases. Our 8B-parameter Temp-R1 achieves state-of-the-art performance on MultiTQ and TimelineKGQA, improving 19.8% over strong baselines on complex questions. Our work establishes a new paradigm for autonomous temporal reasoning agents. The code is available at https://github.com/zjukg/Temp-R1.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.18296v2)
