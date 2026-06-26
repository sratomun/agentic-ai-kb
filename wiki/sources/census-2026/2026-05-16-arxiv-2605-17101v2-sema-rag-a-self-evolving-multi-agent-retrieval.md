---
type: source
source_type: arxiv
title: "SEMA-RAG: A Self-Evolving Multi-Agent Retrieval-Augmented Generation Framework for Medical Reasoning"
authors: Yongfeng Huang, Ruiying Chen, James Cheng
url: https://arxiv.org/abs/2605.17101v2
date: 2026-05-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [clinical-agents, agent-reliability, self-evolving-agents, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# SEMA-RAG: A Self-Evolving Multi-Agent Retrieval-Augmented Generation Framework for Medical Reasoning

**arXiv:** [2605.17101v2](https://arxiv.org/abs/2605.17101v2) · 2026-05-16 · cs.CL
**Authors:** Yongfeng Huang, Ruiying Chen, James Cheng

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-Augmented Generation (RAG) is widely employed to mitigate risks such as hallucinations and knowledge obsolescence in medical question answering, yet its predominantly single-round, static retrieval paradigm misaligns with the multi-stage process of clinical reasoning. This compressed workflow induces two structural deficiencies: question-to-query translation often lacks clinically grounded semantic interpretation, and retrieval lacks iterative sufficiency feedback, making it difficult to form reliable evidence chains. We argue that both issues stem from a deeper cause: overloading a single reasoning chain with heterogeneous tasks of interpretation, exploration, and adjudication. The remedy is to reconstruct the workflow via task decoupling and dynamic multi-round exploration. To this end, we propose SEMA-RAG, a Self-Evolving Multi-Agent RAG framework for medical question answering, which assigns these roles to three specialist agents: the Interpreter Agent for clinical schema interpretation, the Explorer Agent for sufficiency-driven self-evolving retrieval, and the Arbiter Agent for evidence adjudication and answer selection. Across five benchmarks and five LLM backbones, SEMA-RAG improves the strongest baseline by +6.46 accuracy points on average, measured per backbone.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.17101v2)
