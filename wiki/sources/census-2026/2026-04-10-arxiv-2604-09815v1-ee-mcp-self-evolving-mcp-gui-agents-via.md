---
type: source
source_type: arxiv
title: "EE-MCP: Self-Evolving MCP-GUI Agents via Automated Environment Generation and Experience Learning"
authors: Tiantian He, Yihang Chen, Keyue Jiang, Ka Yiu Lee et al.
url: https://arxiv.org/abs/2604.09815v1
date: 2026-04-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [computer-use-agents, self-evolving-agents, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# EE-MCP: Self-Evolving MCP-GUI Agents via Automated Environment Generation and Experience Learning

**arXiv:** [2604.09815v1](https://arxiv.org/abs/2604.09815v1) · 2026-04-10 · cs.AI
**Authors:** Tiantian He, Yihang Chen, Keyue Jiang, Ka Yiu Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Computer-use agents that combine GUI interaction with structured API calls via the Model Context Protocol (MCP) show promise for automating software tasks. However, existing approaches lack a principled understanding of how agents should balance these two modalities and how to enable iterative self-improvement across diverse applications. We formulate MCP-GUI interplay as a unified hybrid policy learning problem where the agent learns when each modality provides complementary advantages, and show that distillation and experience augmentation target fundamentally different failure modes - requiring application-aware mechanism selection. Built on this formulation, we propose a self-evolving framework with a fully automatic pipeline that orchestrates automatic environment generation and validation, trajectory collection, gap-driven task synthesis, and quality-filtered training - all without manual intervention. A key innovation is our experience bank, which accumulates LLM-learned rules from trajectory comparison, enabling inference-time improvement without fine-tuning. Systematic \textbf{cross-application analysis} across three desktop applications reveals that the optimal strategy depends on MCP-GUI composition: distillation achieves 77.8\% pass rate on MCP-dominant tasks (+17.8pp), while the experience bank excels on GUI-intensive tasks (+10.0pp).

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.09815v1)
