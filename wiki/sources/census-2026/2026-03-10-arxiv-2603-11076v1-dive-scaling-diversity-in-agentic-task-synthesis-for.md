---
type: source
source_type: arxiv
title: "DIVE: Scaling Diversity in Agentic Task Synthesis for Generalizable Tool Use"
authors: Aili Chen, Chi Zhang, Junteng Liu, Jiangjie Chen et al.
url: https://arxiv.org/abs/2603.11076v1
date: 2026-03-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# DIVE: Scaling Diversity in Agentic Task Synthesis for Generalizable Tool Use

**arXiv:** [2603.11076v1](https://arxiv.org/abs/2603.11076v1) · 2026-03-10 · cs.AI
**Authors:** Aili Chen, Chi Zhang, Junteng Liu, Jiangjie Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent work synthesizes agentic tasks for post-training tool-using LLMs, yet robust generalization under shifts in tasks and toolsets remains an open challenge. We trace this brittleness to insufficient diversity in synthesized tasks. Scaling diversity is difficult because training requires tasks to remain executable and verifiable, while generalization demands coverage of diverse tool types, toolset combinations, and heterogeneous tool-use patterns. We propose DIVE, an evidence-driven recipe that inverts synthesis order, executing diverse, real-world tools first and reverse-deriving tasks strictly entailed by the resulting traces, thereby providing grounding by construction. DIVE scales structural diversity along two controllable axes, tool-pool coverage and per-task toolset variety, and an Evidence Collection--Task Derivation loop further induces rich multi-step tool-use patterns across 373 tools in five domains. Training Qwen3-8B on DIVE data (48k SFT + 3.2k RL) improves by +22 average points across 9 OOD benchmarks and outperforms the strongest 8B baseline by +68. Remarkably, controlled scaling analysis reveals that diversity scaling consistently outperforms quantity scaling for OOD generalization, even with 4x less data.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.11076v1)
