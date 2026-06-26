---
type: source
source_type: arxiv
title: "TheraAgent: Multi-Agent Framework with Self-Evolving Memory and Evidence-Calibrated Reasoning for PET Theranostics"
authors: Zhihao Chen, Jiahui Wang, Yizhou Chen, Xiaozhong Ji et al.
url: https://arxiv.org/abs/2603.13676v1
date: 2026-03-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [clinical-agents, agent-reliability, self-evolving-agents, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# TheraAgent: Multi-Agent Framework with Self-Evolving Memory and Evidence-Calibrated Reasoning for PET Theranostics

**arXiv:** [2603.13676v1](https://arxiv.org/abs/2603.13676v1) · 2026-03-14 · cs.AI
**Authors:** Zhihao Chen, Jiahui Wang, Yizhou Chen, Xiaozhong Ji et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
PET theranostics is transforming precision oncology, yet treatment response varies substantially; many patients receiving 177Lu-PSMA radioligand therapy (RLT) for metastatic castration-resistant prostate cancer (mCRPC) fail to respond, demanding reliable pre-therapy prediction. While LLM-based agents have shown remarkable potential in complex medical diagnosis, their application to PET theranostic outcome prediction remains unexplored, which faces three key challenges: (1) data and knowledge scarcity: RLT was only FDA-approved in 2022, yielding few training cases and insufficient domain knowledge in general LLMs; (2) heterogeneous information integration: robust prediction hinges on structured knowledge extraction from PET/CT, laboratory tests, and free-text clinical documentation; (3) evidence-grounded reasoning: clinical decisions must be anchored in trial evidence rather than LLM hallucinations. In this paper, we present TheraAgent, to our knowledge, the first agentic framework for PET theranostics, with three core innovations: (1) Multi-Expert Feature Extraction with Confidence-Weighted Consensus, where three specialized experts process heterogeneous inputs with uncertainty quantification; (2) Self-Evolving Agentic Memory (SEA-Mem), which learns prognostic patterns from accumulated cases, enabling case-based reasoning from limited data; (3) Evidence-Calibrated Reasoning, integrating a curated theranostics knowledge base to ground predictions in VISION/TheraP trial evidence. Evaluated on 35 real patients and 400 synthetic cases, TheraAgent achieves 75.7% overall accuracy on real patients and 87.0% on synthetic cases, outperforming MDAgents and MedAgent-Pro by over 20%. These results highlight a promising blueprint for trustworthy AI agents in PET theranostics, enabling trial-calibrated, multi-source decision support. Code will be released upon acceptance.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.13676v1)
