---
type: source
source_type: arxiv
title: "UModel: An Agent-Ready Observability Data Modeling Method at Scale"
authors: Changhua Pei, Zheyuan Li, Zexin Wang, Hang Cui et al.
url: https://arxiv.org/abs/2606.04799v1
date: 2026-06-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.SE
tags: [clinical-agents, knowledge-graph, agent-reliability, arxiv, auto-ingested]
---

# UModel: An Agent-Ready Observability Data Modeling Method at Scale

**arXiv:** [2606.04799v1](https://arxiv.org/abs/2606.04799v1) · 2026-06-03 · cs.SE
**Authors:** Changhua Pei, Zheyuan Li, Zexin Wang, Hang Cui et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
When networked system failures occur, automatically performing Root Cause Analysis (RCA) using observability data is critical for ensuring networked system reliability. Recently, LLM-based agents have shown promise for automating this diagnosis process through advanced reasoning and autonomous exploration. However, existing observability frameworks remain archaic, characterized by fragmented data silos, incompatible schemas, and insufficient semantic metadata, preventing agents from establishing the complex relationships required for effective RCA. To address these challenges, we present UModel, a unified ontological framework that shifts observability from data-centric to object-centric modeling. UModel constructs a virtual ontological layer where heterogeneous telemetry, entities, and expert knowledge are standardized as objects and interconnected via semantic graphs. In addition, we introduce U-SPL, a pipeline-based query interface that enables agents to autonomously explore system topologies and correlate multimodal data. By re-modeling the "AIOps 2025 Challenge" dataset using UModel, the precision of root cause localization improved by 8%, demonstrating that enhanced data organization can significantly increase the accuracy of downstream tasks. UModel provides a scalable modeling framework that, in its deployment at Alibaba Cloud for more than one year, has served tens of thousands of users, sustained millions of operations per second, and delivered sub-second query latency.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.04799v1)
