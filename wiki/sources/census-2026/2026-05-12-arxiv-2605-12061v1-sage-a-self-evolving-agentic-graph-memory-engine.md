---
type: source
source_type: arxiv
title: "SAGE: A Self-Evolving Agentic Graph-Memory Engine for Structure-Aware Associative Memory"
authors: Juntong Wang, Haoyue Zhao, guanghui Pan, Xiyuan Wang et al.
url: https://arxiv.org/abs/2605.12061v1
date: 2026-05-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-reliability, self-evolving-agents, agentic-rag, arxiv, auto-ingested]
---

# SAGE: A Self-Evolving Agentic Graph-Memory Engine for Structure-Aware Associative Memory

**arXiv:** [2605.12061v1](https://arxiv.org/abs/2605.12061v1) · 2026-05-12 · cs.AI
**Authors:** Juntong Wang, Haoyue Zhao, guanghui Pan, Xiyuan Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-term memory is becoming a central bottleneck for language agents. Exsting RAG and GraphRAG systems largely treat memory graphs as static retrieval middleware, which limits their ability to recover complete evidence chains from partial cues, exploit reusable graph-structrual roles, and improve the memory itself through downstream feedback. We introduce SAGE, a Self-evolving Agentic Graph-memory Engine that models graph memory as a dynamic long-term memory substrate. SAGE couples two roles: a memory writer that incrementally constucts structured graph memory from interaction histories, and a Graph Foundation Model-based memory reader to perform retrieval and provide feedback to the memory writer. We provide rigorooous theoretical annalyses supporting the framework. Across multi-hop QA, open-domain retireval, domain-specific review QA, and long-term agent-memory benchmarks, SAGE improves evidence recovery, answer grounding, and retrieval efficiency: after two self-evolution rounds, it achieves the best average rank on multi-hop QA; in zero-shot open-domain transfer, it reaches 82.5/91.6 Recall@2/5 on NQ. Further results on LongMemEval and HaluMem show that traning and reader-writer feedback improve multiple long-term memory and hallucination-diagnostic metrics, suggesting that self-evolving, structure-aware graph memory is a promising foundation for robust long-horizon language agents.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.12061v1)
