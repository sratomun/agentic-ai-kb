---
type: source
source_type: arxiv
title: "ExpWeaver: LLM Agents Learn from Experience via Latent RAG"
authors: Tao Feng, Tianyang Luo, Jingjun Xu, Zhigang Hua et al.
url: https://arxiv.org/abs/2606.01041v1
date: 2026-05-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.CL
tags: [recommendation-agents, agentic-rl, agentic-rag, arxiv, auto-ingested]
---

# ExpWeaver: LLM Agents Learn from Experience via Latent RAG

**arXiv:** [2606.01041v1](https://arxiv.org/abs/2606.01041v1) · 2026-05-31 · cs.CL
**Authors:** Tao Feng, Tianyang Luo, Jingjun Xu, Zhigang Hua et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Experience learning has achieved promising results in enhancing LLM agent planning and reasoning by integrating past interactions as reusable knowledge. However, existing methods remain confined to explicit text space, retrieving experiences via semantic similarity and concatenating them into the context window, leading to substantial token overhead and a decoupled architecture that separates retrieval from generation. To address these limitations, we propose ExpWeaver, a framework that enables LLM agents to learn from experience via latent retrieval-augmented generation, without requiring a separate RAG module. ExpWeaver encodes experiences using the LLM's own hidden states, retrieves relevant experiences directly in latent space at each decoding step, and integrates them through cross-attention aggregation and gated residual mechanisms. The entire pipeline is optimized end-to-end with reinforcement learning, supporting both generative and ranking tasks. We evaluate ExpWeaver on 13 diverse tasks spanning question answering, reasoning, coding, scientific prediction, and recommendation. Results demonstrate that ExpWeaver achieves state-of-the-art performance on 12 out of 13 tasks, outperforming the strongest baseline by over 6.8%; maintains token efficiency comparable to non-retrieval baselines while text-based retrieval methods require 1.5 to 2 times more tokens; and exhibits superior cross-domain generalization, outperforming the strongest baseline by 16.32% under zero-shot transfer and 15.21% under few-shot transfer. Our code for ExpWeaver is released at https://github.com/ulab-uiuc/ExpWeaver.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.01041v1)
