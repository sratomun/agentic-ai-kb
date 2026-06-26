---
type: source
source_type: arxiv
title: "PhyNiKCE: A Neurosymbolic Agentic Framework for Autonomous Computational Fluid Dynamics"
authors: E Fan, Lisong Shi, Zhengtong Li, Chih-yung Wen
url: https://arxiv.org/abs/2602.11666v1
date: 2026-02-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, agent-security, agentic-rag, governance-gap, arxiv, auto-ingested]
---

# PhyNiKCE: A Neurosymbolic Agentic Framework for Autonomous Computational Fluid Dynamics

**arXiv:** [2602.11666v1](https://arxiv.org/abs/2602.11666v1) · 2026-02-12 · cs.AI
**Authors:** E Fan, Lisong Shi, Zhengtong Li, Chih-yung Wen

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The deployment of autonomous agents for Computational Fluid Dynamics (CFD), is critically limited by the probabilistic nature of Large Language Models (LLMs), which struggle to enforce the strict conservation laws and numerical stability required for physics-based simulations. Reliance on purely semantic Retrieval Augmented Generation (RAG) often leads to "context poisoning," where agents generate linguistically plausible but physically invalid configurations due to a fundamental Semantic-Physical Disconnect. To bridge this gap, this work introduces PhyNiKCE (Physical and Numerical Knowledgeable Context Engineering), a neurosymbolic agentic framework for trustworthy engineering. Unlike standard black-box agents, PhyNiKCE decouples neural planning from symbolic validation. It employs a Symbolic Knowledge Engine that treats simulation setup as a Constraint Satisfaction Problem, rigidly enforcing physical constraints via a Deterministic RAG Engine with specialized retrieval strategies for solvers, turbulence models, and boundary conditions. Validated through rigorous OpenFOAM experiments on practical, non-tutorial CFD tasks using Gemini-2.5-Pro/Flash, PhyNiKCE demonstrates a 96% relative improvement over state-of-the-art baselines. Furthermore, by replacing trial-and-error with knowledge-driven initialization, the framework reduced autonomous self-correction loops by 59% while simultaneously lowering LLM token consumption by 17%. These results demonstrate that decoupling neural generation from symbolic constraint enforcement significantly enhances robustness and efficiency. While validated on CFD, this architecture offers a scalable, auditable paradigm for Trustworthy Artificial Intelligence in broader industrial automation.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]] · [[governance-gap|Governance gap]]
- **Entities:** [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.11666v1)
