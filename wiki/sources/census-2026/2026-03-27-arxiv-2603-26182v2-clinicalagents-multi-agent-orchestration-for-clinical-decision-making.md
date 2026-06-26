---
type: source
source_type: arxiv
title: "ClinicalAgents: Multi-Agent Orchestration for Clinical Decision Making with Dual-Memory"
authors: Zhuohan Ge, Haoyang Li, Yubo Wang, Nicole Hu et al.
url: https://arxiv.org/abs/2603.26182v2
date: 2026-03-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [clinical-agents, science-agents, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# ClinicalAgents: Multi-Agent Orchestration for Clinical Decision Making with Dual-Memory

**arXiv:** [2603.26182v2](https://arxiv.org/abs/2603.26182v2) · 2026-03-27 · cs.CL
**Authors:** Zhuohan Ge, Haoyang Li, Yubo Wang, Nicole Hu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While Large Language Models (LLMs) have demonstrated potential in healthcare, they often struggle with the complex, non-linear reasoning required for accurate clinical diagnosis. Existing methods typically rely on static, linear mappings from symptoms to diagnoses, failing to capture the iterative, hypothesis-driven reasoning inherent in human clinicians. To bridge this gap, we introduce ClinicalAgents, a novel multi-agent framework designed to simulate the cognitive workflow of expert clinicians. Unlike rigid sequential chains, ClinicalAgents employs a dynamic orchestration mechanism modeled as a Monte Carlo Tree Search (MCTS) process. This allows an orchestrator to iteratively generate hypotheses, actively verify evidence, and trigger backtracking when critical information is missing. The foundation of this framework is a Dual-Memory architecture: a mutable working memory that maintains the evolving patient state for context-aware reasoning, and a static experience memory that retrieves clinical guidelines and historical cases via an active feedback loop. Extensive experiments demonstrate that ClinicalAgents achieves the best performance among evaluated baselines, significantly enhancing both diagnostic accuracy and explainability compared to strong single-agent and multi-agent baselines. Our code is released at https://github.com/ZhuohanGe/ClinicalAgents-Code.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.26182v2)
