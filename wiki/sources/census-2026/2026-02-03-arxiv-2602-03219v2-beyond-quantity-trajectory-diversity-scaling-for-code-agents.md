---
type: source
source_type: arxiv
title: "Beyond Quantity: Trajectory Diversity Scaling for Code Agents"
authors: Guhong Chen, Chenghao Sun, Cheng Fu, Qiyao Wang et al.
url: https://arxiv.org/abs/2602.03219v2
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [coding-agents, agent-protocols, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Beyond Quantity: Trajectory Diversity Scaling for Code Agents

**arXiv:** [2602.03219v2](https://arxiv.org/abs/2602.03219v2) · 2026-02-03 · cs.AI
**Authors:** Guhong Chen, Chenghao Sun, Cheng Fu, Qiyao Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As code large language models (LLMs) evolve into tool-interactive agents via the Model Context Protocol (MCP), their generalization is increasingly limited by low-quality synthetic data and the diminishing returns of quantity scaling. Moreover, quantity-centric scaling exhibits an early bottleneck that underutilizes trajectory data. We propose TDScaling, a Trajectory Diversity Scaling-based data synthesis framework for code agents that scales performance through diversity rather than raw volume. Under a fixed training budget, increasing trajectory diversity yields larger gains than adding more trajectories, improving the performance-cost trade-off for agent training. TDScaling integrates four innovations: (1) a Business Cluster mechanism that captures real-service logical dependencies; (2) a blueprint-driven multi-agent paradigm that enforces trajectory coherence; (3) an adaptive evolution mechanism that steers synthesis toward long-tail scenarios using Domain Entropy, Reasoning Mode Entropy, and Cumulative Action Complexity to prevent mode collapse; and (4) a sandboxed code tool that mitigates catastrophic forgetting of intrinsic coding capabilities. Experiments on general tool-use benchmarks (BFCL, tau^2-Bench) and code agent tasks (RebenchT, CodeCI, BIRD) demonstrate a win-win outcome: TDScaling improves both tool-use generalization and inherent coding proficiency. We plan to release the full codebase and the synthesized dataset (including 30,000+ tool clusters) upon publication.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[bird-benchmark]] · [[bfcl]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03219v2)
