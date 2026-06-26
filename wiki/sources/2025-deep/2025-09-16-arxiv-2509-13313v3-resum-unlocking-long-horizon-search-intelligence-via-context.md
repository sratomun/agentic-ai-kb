---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization"
authors: Xixi Wu, Kuan Li, Yida Zhao, Liwen Zhang et al.
url: https://arxiv.org/abs/2509.13313v3
date: 2025-09-16
citationCount: 77
influentialCitationCount: 8
velocity: 8.4
ingested: 2026-06-22
tags: [computer-use-agents, agentic-rl, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization

**arXiv [2509.13313v3](https://arxiv.org/abs/2509.13313v3)** · 2025-09-16 · **77 citations** (8 influential · 8.4/mo) · Xixi Wu, Kuan Li, Yida Zhao, Liwen Zhang et al.

## Abstract
Large Language Model (LLM)-based web agents excel at knowledge-intensive tasks but face a fundamental conflict between the need for extensive exploration and the constraints of limited context windows. Current solutions typically rely on architectural modifications, e.g., internal memory tokens, which break compatibility with pre-existing agents and necessitate costly end-to-end retraining. To overcome these limitations, we introduce ReSum, a lightweight, plug-and-play paradigm that enables unbounded exploration by periodically invoking an external tool to condense interaction histories into compact summaries. Although this paradigm functions without training, standard agents are not inherently aligned to reason over such compressed contexts. To bridge this gap, we propose ReSum-GRPO, which adapts Group Relative Policy Optimization (GRPO) via advantage broadcasting to propagate final rewards across segmented trajectories, enabling credit assignments over long-horizons. Extensive experiments show that ReSum achieves a 4.5% improvement over ReAct in training-free settings, with ReSum-GRPO yielding a further 8.2% gain. Notably, with only 1K training samples, a ReSum-enhanced 30B agent achieves competitive performance with leading open-source models, showing ReSum's effectiveness.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminary 3 Methodology 3.1 ReSum Paradigm 3.2 Summary Tool Specification 3.3 ReSum-GRPO 4 Experiments and Analysis 4.1 Experimental Setup 4.2 Performance of the Training-free ReSum 4.3 Performance of ReSum-GRPO 4.4 Applicability to Agents with Extensive Context 5 Conclusion References A Related Works B Algorithm Pseudo-Code C Prompt D Implementation Details D.1 Implementation of Inference Paradigms D.2 RL Training Configuration E Supplementary Materials for ReSumTool-30B E.1 Cases of LLMs in Context Summarization E.2 Training Configurations E.3 Evaluation for ReSumTool-30B F Supplementary Materials for Experiments F.1 Training Efficiency F.2 Inference Costs F.3 Efficiency Comparison with MEM1 F.4 Case Study G Justification for LLM-as-Judge Evaluation License: CC Zero arXiv:2509.13313v3 [cs.CL] 26 Mar 2026 ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization Xixi Wu Kuan Li Yida Zhao Liwen Zhang Litu Ou Huifeng Yin Zhongwang Zhang Xinmiao Yu D…

**Method / approach.** Methodology 3.1 ReSum Paradigm 3.2 Summary Tool Specification 3.3 ReSum-GRPO 4 Experiments and Analysis 4.1 Experimental Setup 4.2 Performance of the Training-free ReSum 4.3 Performance of ReSum-GRPO 4.4 Applicability to Agents with Extensive Context 5 Conclusion References A Related Works B Algorithm Pseudo-Code C Prompt D Implementation Details D.1 Implementation of Inference Paradigms D.2 RL Training Configuration E Supplementary Materials for ReSumTool-30B E.1 Cases of LLMs in Context Summarization E.2 Training Configurations E.3 Evaluation for ReSumTool-30B F Supplementary Materials for Experiments F.1 Training Efficiency F.2 Inference Costs F.3 Efficiency Comparison with MEM1 F.4 Case Study G Justification for LLM-as-Judge Evaluation License: CC Zero arXiv:2509.13313v3 [cs.CL] 26 Mar 2026 ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization Xixi Wu Kuan Li Yida Zhao Liwe…

**Results.** Experiments and Analysis 4.1 Experimental Setup 4.2 Performance of the Training-free ReSum 4.3 Performance of ReSum-GRPO 4.4 Applicability to Agents with Extensive Context 5 Conclusion References A Related Works B Algorithm Pseudo-Code C Prompt D Implementation Details D.1 Implementation of Inference Paradigms D.2 RL Training Configuration E Supplementary Materials for ReSumTool-30B E.1 Cases of LLMs in Context Summarization E.2 Training Configurations E.3 Evaluation for ReSumTool-30B F Supplementary Materials for Experiments F.1 Training Efficiency F.2 Inference Costs F.3 Efficiency Comparison with MEM1 F.4 Case Study G Justification for LLM-as-Judge Evaluation License: CC Zero arXiv:2509.13313v3 [cs.CL] 26 Mar 2026 ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization Xixi Wu Kuan Li Yida Zhao Liwen Zhang Litu Ou Huifeng Yin Zhongwa…

**Conclusion.** Conclusion References A Related Works B Algorithm Pseudo-Code C Prompt D Implementation Details D.1 Implementation of Inference Paradigms D.2 RL Training Configuration E Supplementary Materials for ReSumTool-30B E.1 Cases of LLMs in Context Summarization E.2 Training Configurations E.3 Evaluation for ReSumTool-30B F Supplementary Materials for Experiments F.1 Training Efficiency F.2 Inference Costs F.3 Efficiency Comparison with MEM1 F.4 Case Study G Justification for LLM-as-Judge Evaluation License: CC Zero arXiv:2509.13313v3 [cs.CL] 26 Mar 2026 ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization Xixi Wu Kuan Li Yida Zhao Liwen Zhang Litu Ou Huifeng…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]]
- **Raw:** `raw/arxiv/2509.13313v3.md` · `raw/arxiv/2509.13313v3.fulltext.md`
