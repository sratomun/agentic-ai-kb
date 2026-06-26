---
type: source
source_type: arxiv
title: "LIDL: LLM Integration Defect Localization via Knowledge Graph-Enhanced Multi-Agent Analysis"
authors: Gou Tan, Zilong He, Min Li, Pengfei Chen et al.
url: https://arxiv.org/abs/2601.05539v1
date: 2026-01-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.SE
tags: [knowledge-graph, multi-agent-systems, arxiv, auto-ingested]
---

# LIDL: LLM Integration Defect Localization via Knowledge Graph-Enhanced Multi-Agent Analysis

**arXiv:** [2601.05539v1](https://arxiv.org/abs/2601.05539v1) · 2026-01-09 · cs.SE
**Authors:** Gou Tan, Zilong He, Min Li, Pengfei Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-integrated software, which embeds or interacts with large language models (LLMs) as functional components, exhibits probabilistic and context-dependent behaviors that fundamentally differ from those of traditional software. This shift introduces a new category of integration defects that arise not only from code errors but also from misaligned interactions among LLM-specific artifacts, including prompts, API calls, configurations, and model outputs. However, existing defect localization techniques are ineffective at identifying these LLM-specific integration defects because they fail to capture cross-layer dependencies across heterogeneous artifacts, cannot exploit incomplete or misleading error traces, and lack semantic reasoning capabilities for identifying root causes. To address these challenges, we propose LIDL, a multi-agent framework for defect localization in LLM-integrated software. LIDL (1) constructs a code knowledge graph enriched with LLM-aware annotations that represent interaction boundaries across source code, prompts, and configuration files, (2) fuses three complementary sources of error evidence inferred by LLMs to surface candidate defect locations, and (3) applies context-aware validation that uses counterfactual reasoning to distinguish true root causes from propagated symptoms. We evaluate LIDL on 146 real-world defect instances collected from 105 GitHub repositories and 16 agent-based systems. The results show that LIDL significantly outperforms five state-of-the-art baselines across all metrics, achieving a Top-3 accuracy of 0.64 and a MAP of 0.48, which represents a 64.1% improvement over the best-performing baseline. Notably, LIDL achieves these gains while reducing cost by 92.5%, demonstrating both high accuracy and cost efficiency.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.05539v1)
