---
type: source
source_type: arxiv
title: "Agentic reinforcement learning empowers next-generation chemical language models for molecular design and synthesis"
authors: Hao Li, He Cao, Shenyao Peng, Zijing Liu et al.
url: https://arxiv.org/abs/2601.17687v2
date: 2026-01-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.LG
tags: [science-agents, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# Agentic reinforcement learning empowers next-generation chemical language models for molecular design and synthesis

**arXiv:** [2601.17687v2](https://arxiv.org/abs/2601.17687v2) · 2026-01-25 · cs.LG
**Authors:** Hao Li, He Cao, Shenyao Peng, Zijing Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Language models are revolutionizing the biochemistry domain, assisting scientists in drug design and chemical synthesis with high efficiency. Yet current approaches struggle between small language models prone to hallucination and limited knowledge retention, and large cloud-based language models plagued by privacy risks and high inference costs. To bridge this gap, we introduce ChemCRAFT, a novel framework leveraging agentic reinforcement learning to decouple chemical reasoning from knowledge storage. Instead of forcing the model to memorize vast chemical data, our approach empowers the language model to interact with a sandbox for precise information retrieval. This externalization of knowledge allows a locally deployable small model to achieve superior performance with minimal inference costs. To enable small language models for agent-calling ability, we build an agentic trajectory construction pipeline and a comprehensive chemical-agent sandbox. Based on sandbox interactions, we constructed ChemToolDataset, the first large-scale chemical tool trajectory dataset. Simultaneously, we propose SMILES-GRPO to build a dense chemical reward function, promoting the model's ability to call chemical agents. Evaluations across diverse aspects of drug design show that ChemCRAFT outperforms current cloud-based LLMs in molecular structure analysis, molecular optimization, and synthesis pathway prediction, demonstrating that scientific reasoning is not solely an emergent ability of model scale, but a learnable policy of tool orchestration. This work establishes a cost-effective and privacy-preserving paradigm for AI-aided chemistry, opening new avenues for accelerating molecular discovery with locally deployable agents. Code available at https://github.com/HowardLi1984/ChemCraft.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.17687v2)
