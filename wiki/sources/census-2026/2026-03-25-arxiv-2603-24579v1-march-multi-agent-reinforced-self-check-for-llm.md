---
type: source
source_type: arxiv
title: "MARCH: Multi-Agent Reinforced Self-Check for LLM Hallucination"
authors: Zhuo Li, Yupeng Zhang, Pengyu Cheng, Jiajun Song et al.
url: https://arxiv.org/abs/2603.24579v1
date: 2026-03-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agent-reliability, self-evolving-agents, agentic-rl, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# MARCH: Multi-Agent Reinforced Self-Check for LLM Hallucination

**arXiv:** [2603.24579v1](https://arxiv.org/abs/2603.24579v1) · 2026-03-25 · cs.CL
**Authors:** Zhuo Li, Yupeng Zhang, Pengyu Cheng, Jiajun Song et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Hallucination remains a critical bottleneck for large language models (LLMs), undermining their reliability in real-world applications, especially in Retrieval-Augmented Generation (RAG) systems. While existing hallucination detection methods employ LLM-as-a-judge to verify LLM outputs against retrieved evidence, they suffer from inherent confirmation bias, where the verifier inadvertently reproduces the errors of the original generation. To address this, we introduce Multi-Agent Reinforced Self-Check for Hallucination (MARCH), a framework that enforces rigorous factual alignment by leveraging deliberate information asymmetry. MARCH orchestrates a collaborative pipeline of three specialized agents: a Solver, a Proposer, and a Checker. The Solver generates an initial RAG response, which the Proposer decomposes into claim-level verifiable atomic propositions. Crucially, the Checker validates these propositions against retrieved evidence in isolation, deprived of the Solver's original output. This well-crafted information asymmetry scheme breaks the cycle of self-confirmation bias. By training this pipeline with multi-agent reinforcement learning (MARL), we enable the agents to co-evolve and optimize factual adherence. Extensive experiments across hallucination benchmarks demonstrate that MARCH substantially reduces hallucination rates. Notably, an 8B-parameter LLM equipped with MARCH achieves performance competitive with powerful closed-source models. MARCH paves a scalable path for factual self-improvement of LLMs through co-evolution. The code is at https://github.com/Qwen-Applications/MARCH.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.24579v1)
