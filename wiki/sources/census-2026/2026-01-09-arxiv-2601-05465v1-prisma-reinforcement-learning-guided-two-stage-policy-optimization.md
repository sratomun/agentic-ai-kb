---
type: source
source_type: arxiv
title: "PRISMA: Reinforcement Learning Guided Two-Stage Policy Optimization in Multi-Agent Architecture for Open-Domain Multi-Hop Question Answering"
authors: Yu Liu, Wenxiao Zhang, Cong Cao, Wenxuan Lu et al.
url: https://arxiv.org/abs/2601.05465v1
date: 2026-01-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agent-reliability, agentic-rl, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# PRISMA: Reinforcement Learning Guided Two-Stage Policy Optimization in Multi-Agent Architecture for Open-Domain Multi-Hop Question Answering

**arXiv:** [2601.05465v1](https://arxiv.org/abs/2601.05465v1) · 2026-01-09 · cs.AI
**Authors:** Yu Liu, Wenxiao Zhang, Cong Cao, Wenxuan Lu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Answering real-world open-domain multi-hop questions over massive corpora is a critical challenge in Retrieval-Augmented Generation (RAG) systems. Recent research employs reinforcement learning (RL) to end-to-end optimize the retrieval-augmented reasoning process, directly enhancing its capacity to resolve complex queries. However, reliable deployment is hindered by two obstacles. 1) Retrieval Collapse: iterative retrieval over large corpora fails to locate intermediate evidence containing bridge answers without reasoning-guided planning, causing downstream reasoning to collapse. 2) Learning Instability: end-to-end trajectory training suffers from weak credit assignment across reasoning chains and poor error localization across modules, causing overfitting to benchmark-specific heuristics that limit transferability and stability. To address these problems, we propose PRISMA, a decoupled RL-guided framework featuring a Plan-Retrieve-Inspect-Solve-Memoize architecture. PRISMA's strength lies in reasoning-guided collaboration: the Inspector provides reasoning-based feedback to refine the Planner's decomposition and fine-grained retrieval, while enforcing evidence-grounded reasoning in the Solver. We optimize individual agent capabilities via Two-Stage Group Relative Policy Optimization (GRPO). Stage I calibrates the Planner and Solver as specialized experts in planning and reasoning, while Stage II utilizes Observation-Aware Residual Policy Optimization (OARPO) to enhance the Inspector's ability to verify context and trigger targeted recovery. Experiments show that PRISMA achieves state-of-the-art performance on ten benchmarks and can be deployed efficiently in real-world scenarios.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.05465v1)
