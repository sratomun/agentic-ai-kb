---
type: source
source_type: arxiv
title: "MACReD: A Multi-Agent Collaborative Reasoning Framework for Reaction Diagram Parsing"
authors: Chuang Tang, Chenhao Lin, Yin Xu, Hao Wang et al.
url: https://arxiv.org/abs/2605.28077v1
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MACReD: A Multi-Agent Collaborative Reasoning Framework for Reaction Diagram Parsing

**arXiv:** [2605.28077v1](https://arxiv.org/abs/2605.28077v1) · 2026-05-27 · cs.AI
**Authors:** Chuang Tang, Chenhao Lin, Yin Xu, Hao Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Parsing chemical reaction diagrams from scientific literature is challenging due to heterogeneous layouts, intertwined visual elements, and the difficulty of integrating recognition and reasoning. Existing vision-language models advance multimodal understanding but still fail on complex diagrams, struggling to maintain spatial coherence and to integrate multidimensional information during reasoning. To address these issues, we propose MACReD, a hierarchical multi-agent framework that coordinates specialized agents for molecular perception, arrow understanding, text extraction, and reaction reconstruction within a unified VLM-guided architecture. The planning and perception layers use flexible, fine-grained detection to handle visual complexity, while the reasoning layer uses a multigraph fusion mechanism to integrate heterogeneous cues and enforce chemically consistent global reasoning. Experiments on the RxnScribe benchmark show that MACReD achieves state-of-the-art performance, with F1 scores of 75.2% and 84.6% under hard and soft match criteria, outperforming the RxnScribe baseline, which obtains 69.1% and 80.0%, respectively. These results demonstrate the robustness of MACReD across diverse diagram layouts, including multi-step and tree-structured reactions.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.28077v1)
