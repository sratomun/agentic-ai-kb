---
type: source
source_type: arxiv
title: "Multi-agent Framework for Time-Sensitive Complementary Collaboration in Minecraft"
authors: Juheon Yi, Jinglu Wang, Xiaoyi Zhang, Yan Lu
url: https://arxiv.org/abs/2606.15684v1
date: 2026-06-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Multi-agent Framework for Time-Sensitive Complementary Collaboration in Minecraft

**arXiv:** [2606.15684v1](https://arxiv.org/abs/2606.15684v1) · 2026-06-14 · cs.AI
**Authors:** Juheon Yi, Jinglu Wang, Xiaoyi Zhang, Yan Lu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present TickingCollabBench, a Minecraft-based multi-agent benchmark for a novel class of time-sensitive complementary collaboration tasks. Our benchmark reflects four core characteristics of real-world collaboration: agent heterogeneity, mandatory collaboration, dynamic environments, and strict real-time constraints with failure risks. To enable this, we develop the TickingCollab framework, which supports the generation of diverse dynamic environments and abstracts Minecraft's primitive APIs to enable declarative YAML task specifications for composing these events. Building on this, we design a feasibility-aware automated benchmark generation pipeline, where an LLM drafts structurally diverse task configurations and feasibility verifier filters out invalid ones using approximate constraints. Evaluations demonstrate that lang latency and inherent difficulty of coordinating under partial observability and agent heterogeneity cause LLMs to frequently fail under dynamic environments and fall significantly short of a global-knowledge oracle.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.15684v1)
