---
type: source
source_type: arxiv
title: "MedCoG: Maximizing LLM Inference Density in Medical Reasoning via Meta-Cognitive Regulation"
authors: Yu Zhao, Hao Guan, Yongcheng Jing, Ying Zhang et al.
url: https://arxiv.org/abs/2602.07905v2
date: 2026-02-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# MedCoG: Maximizing LLM Inference Density in Medical Reasoning via Meta-Cognitive Regulation

**arXiv:** [2602.07905v2](https://arxiv.org/abs/2602.07905v2) · 2026-02-08 · cs.AI
**Authors:** Yu Zhao, Hao Guan, Yongcheng Jing, Ying Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have shown strong potential in complex medical reasoning yet face diminishing gains under inference scaling laws. While existing studies augment LLMs with various knowledge types, it remains unclear how effectively the additional costs translate into accuracy. In this paper, we explore how meta-cognition of LLMs, i.e., their self-assessment of their own cognitive states, can regulate the reasoning process. Specifically, we propose MedCoG, a Medical Meta-Cognition Agent with Knowledge Graph, where the meta-cognitive assessments of task complexity, familiarity, and knowledge density dynamically regulate utilization of procedural, episodic, and factual knowledge. The LLM-centric on-demand reasoning aims to mitigate the diminishing returns under scaling law by (1) reducing costs via avoiding indiscriminate scaling, (2) improving accuracy via filtering out distractive knowledge. To validate this, we empirically characterize the scaling curve and introduce inference density to quantify inference efficiency. Experiments demonstrate the effectiveness and efficiency of MedCoG on five hard sets of medical benchmarks, yielding 6.2x inference density. Furthermore, the Oracle study highlights the significant potential of meta-cognitive regulation.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.07905v2)
