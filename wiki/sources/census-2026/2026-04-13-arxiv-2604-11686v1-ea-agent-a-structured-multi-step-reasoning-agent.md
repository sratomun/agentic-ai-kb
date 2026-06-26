---
type: source
source_type: arxiv
title: "EA-Agent: A Structured Multi-Step Reasoning Agent for Entity Alignment"
authors: Yixuan Nan, Xixun Lin, Yanmin Shang, Ge Zhang et al.
url: https://arxiv.org/abs/2604.11686v1
date: 2026-04-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.IR
tags: [knowledge-graph, agent-evaluation, arxiv, auto-ingested]
---

# EA-Agent: A Structured Multi-Step Reasoning Agent for Entity Alignment

**arXiv:** [2604.11686v1](https://arxiv.org/abs/2604.11686v1) · 2026-04-13 · cs.IR
**Authors:** Yixuan Nan, Xixun Lin, Yanmin Shang, Ge Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Entity alignment (EA) aims to identify entities across different knowledge graphs (KGs) that refer to the same real-world object and plays a critical role in knowledge fusion and integration. Traditional EA methods mainly rely on knowledge representation learning, but their performance is often limited under noisy or sparsely supervised scenarios. Recently, large language models (LLMs) have been introduced to EA and achieved notable improvements by leveraging rich semantic knowledge. However, existing LLM-based EA approaches typically treat LLMs as black-box decision makers, resulting in limited interpretability, and the direct use of large-scale triples substantially increases inference cost. To address these challenges, we propose \textbf{EA-Agent}, a reasoning-driven agent for EA. EA-Agent formulates EA as a structured reasoning process with multi-step planning and execution, enabling interpretable alignment decisions. Within this process, it introduces attribute and relation triple selectors to filter redundant triples before feeding them into the LLM, effectively addressing efficiency challenges. Experimental results on three benchmark datasets demonstrate that EA-Agent consistently outperforms existing EA methods and achieves state-of-the-art performance. The source code is available at https://github.com/YXNan0110/EA-Agent.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.11686v1)
