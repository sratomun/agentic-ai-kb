---
type: source
source_type: arxiv
title: "MLEvolve: A Self-Evolving Framework for Automated Machine Learning Algorithm Discovery"
authors: Shangheng Du, Xiangchao Yan, Jinxin Shi, Zongsheng Cao et al.
url: https://arxiv.org/abs/2606.06473v1
date: 2026-06-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [coding-agents, science-agents, self-evolving-agents, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# MLEvolve: A Self-Evolving Framework for Automated Machine Learning Algorithm Discovery

**arXiv:** [2606.06473v1](https://arxiv.org/abs/2606.06473v1) · 2026-06-04 · cs.AI
**Authors:** Shangheng Du, Xiangchao Yan, Jinxin Shi, Zongsheng Cao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM) agents are increasingly applied to long-horizon tasks such as scientific discovery and machine learning engineering (MLE), where sustained self-evolution becomes a key capability. However, existing MLE agents suffer from inter-branch information isolation, memoryless search, and lack of hierarchical control, which together hinder long-horizon optimization. We present MLEvolve, an LLM-based self-evolving multi-agent framework for end-to-end machine learning algorithm discovery. By extending tree search to Progressive MCGS, MLEvolve enables cross-branch information flow through graph-based reference edges and gradually shifts the search from broad exploration to focused exploitation with an entropy-inspired progressive schedule. To allow the agent to evolve with accumulated experience, we introduce Retrospective Memory, which combines a cold-start domain knowledge base with a dynamic global memory for task-specific experience retrieval and reuse. For stable long-horizon iteration, we further decouple strategic planning from code generation with adaptive coding modes. Evaluation on MLE-Bench shows that MLEvolve achieves state-of-the-art performance across multiple dimensions including average medal rate and valid submission rate under a 12-hour budget (half the standard runtime). Moreover, MLEvolve also outperforms specialized algorithm discovery methods including AlphaEvolve on mathematical algorithm optimization tasks, demonstrating strong cross-domain generalization. Our code is available at https://github.com/InternScience/MLEvolve.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[science-agents|Science agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mle-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.06473v1)
