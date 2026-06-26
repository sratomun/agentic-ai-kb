---
type: source
source_type: arxiv
title: "Scaling Agentic Capabilities via Grounded Interaction Synthesis"
authors: Wenhang Shi, Jinhao Dong, Yiren Chen, Zhe Zhao et al.
url: https://arxiv.org/abs/2606.02001v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agent-security, agent-protocols, agent-memory, arxiv, auto-ingested]
---

# Scaling Agentic Capabilities via Grounded Interaction Synthesis

**arXiv:** [2606.02001v1](https://arxiv.org/abs/2606.02001v1) · 2026-06-01 · cs.CL
**Authors:** Wenhang Shi, Jinhao Dong, Yiren Chen, Zhe Zhao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
General agentic intelligence hinges on the ability to interact with diverse real-world tools to complete complex tasks, a capability fundamentally tied to the quality of interaction data. To bypass the prohibitive costs of human annotation, prevailing paradigms depend entirely on Large Language Models (LLMs) to scale the synthesis of agentic environments and tasks. However, such unconstrained generation often degenerates into biased random sampling of LLMs' internal priors, failing to capture the diversity and difficulty of real-world domains or construct high-fidelity, long-horizon tasks. In this work, we introduce Grounded Agentic Interaction Synthesis (GAIS), a framework that automates the scalable construction of diverse environments and complex tasks via a two-phase grounding mechanism. Specifically, we construct protocol-anchored environments derived from real-world Model Context Protocol (MCP) servers to ensure functional diversity and difficulty. Subsequently, we employ structure-guided planning to navigate these environments, actively enforcing logical dependencies and adversarial policies to generate complex tasks. Experiments on BFCL, $τ^2$-Bench, and ACEBench demonstrate that GAIS-synthesized data significantly outperforms state-of-the-art baselines, enabling base models to match or even surpass their official instruction-tuned counterparts. Furthermore, GAIS exhibits superior data efficiency and scalability, achieving exceptional capabilities with significantly less data while maintaining continuous growth where baselines stagnate. Our code and dataset are publicly available at https://github.com/Eric8932/GAIS.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]]
- **Entities:** [[mcp]] · [[bfcl]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.02001v1)
