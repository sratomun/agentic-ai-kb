---
type: source
source_type: arxiv
title: "Paper2Rebuttal: A Multi-Agent Framework for Transparent Author Response Assistance"
authors: Qianli Ma, Chang Guo, Zhiheng Tian, Siyu Wang et al.
url: https://arxiv.org/abs/2601.14171v1
date: 2026-01-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [multi-agent-systems, arxiv, auto-ingested]
---

# Paper2Rebuttal: A Multi-Agent Framework for Transparent Author Response Assistance

**arXiv:** [2601.14171v1](https://arxiv.org/abs/2601.14171v1) · 2026-01-20 · cs.AI
**Authors:** Qianli Ma, Chang Guo, Zhiheng Tian, Siyu Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Writing effective rebuttals is a high-stakes task that demands more than linguistic fluency, as it requires precise alignment between reviewer intent and manuscript details. Current solutions typically treat this as a direct-to-text generation problem, suffering from hallucination, overlooked critiques, and a lack of verifiable grounding. To address these limitations, we introduce $\textbf{RebuttalAgent}$, the first multi-agents framework that reframes rebuttal generation as an evidence-centric planning task. Our system decomposes complex feedback into atomic concerns and dynamically constructs hybrid contexts by synthesizing compressed summaries with high-fidelity text while integrating an autonomous and on-demand external search module to resolve concerns requiring outside literature. By generating an inspectable response plan before drafting, $\textbf{RebuttalAgent}$ ensures that every argument is explicitly anchored in internal or external evidence. We validate our approach on the proposed $\textbf{RebuttalBench}$ and demonstrate that our pipeline outperforms strong baselines in coverage, faithfulness, and strategic coherence, offering a transparent and controllable assistant for the peer review process. Code will be released.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.14171v1)
