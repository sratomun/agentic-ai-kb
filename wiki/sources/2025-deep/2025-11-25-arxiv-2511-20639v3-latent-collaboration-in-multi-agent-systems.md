---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Latent Collaboration in Multi-Agent Systems"
authors: Jiaru Zou, Ruizhong Qiu, Gaotang Li, Xiyuan Yang et al.
url: https://arxiv.org/abs/2511.20639v3
date: 2025-11-25
citationCount: 32
influentialCitationCount: 5
velocity: 4.66
ingested: 2026-06-22
tags: [coding-agents, agent-memory, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Latent Collaboration in Multi-Agent Systems

**arXiv [2511.20639v3](https://arxiv.org/abs/2511.20639v3)** · 2025-11-25 · **32 citations** (5 influential · 4.66/mo) · Jiaru Zou, Ruizhong Qiu, Gaotang Li, Xiyuan Yang et al.

## Abstract
Multi-agent systems (MAS) extend large language models (LLMs) from independent single-model reasoning to coordinative system-level intelligence. While existing LLM agents depend on text-based mediation for reasoning and communication, we take a step forward by enabling models to collaborate directly within the continuous latent space. We introduce LatentMAS, an end-to-end training-free framework that enables pure latent collaboration among LLM agents. In LatentMAS, each agent first performs auto-regressive latent thoughts generation through last-layer hidden embeddings instead of text. Then, a shared latent working memory preserves and transfers each agent's internal representations and latent thoughts, ensuring lossless information exchange without re-encoding. We provide detailed theoretical analyses showing that LatentMAS achieves higher expressiveness and lossless information preservation with lower overall complexity than standard text-based MAS. In addition, empirical evaluations across 9 comprehensive benchmarks spanning math and science reasoning, commonsense understanding, and code generation show that LatentMAS outperforms advanced single agents and text-based MAS baselines, achieving up to 14.6% higher accuracy, reducing output token usage by 70.8%-83.7%, and providing 4$\times$-4.3$\times$ faster end-to-end inference. Code and data are fully open-sourced at https://github.com/Gen-Verse/LatentMAS.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminary and Notations 3 LatentMAS 3.1 Auto-regressive Latent Thoughts Generation 3.2 Thoughts Transfer via Latent Working Memory 3.3 End-to-End Pipeline with Complexity Analyses 4 Empirical Evaluations 4.1 Main Results 4.2 Efficiency Analyses on Latent Collaboration. 5 In-depth Analyses on LatentMAS 6 Related Work 7 Conclusion References A Input-Output Alignment in LatentMAS A.1 Theoretical Justification on W a W_{a} A.2 Solving the Alignment Matrix W a W_{a} B Theoretical Analysis B.1 Proof of Theorem 3.1 B.2 Proof of Theorem 3.3 Induction step. Induction base case. Conclusion. B.3 Proof of Theorem 3.4 Time complexity of our method. Time complexity of the vanilla text-based MAS. C Experiment Setups C.1 Evaluation Details Math Science Reasoning. Commonsense Reasoning. Code Generation. C.2 Implementation Details Software Backend Evaluation protocol. D Additional Experiments D.1 Performance of LatentMAS under Hierarchical MAS Setting D.2 LatentMAS on Llama Backbon…

**Method / approach.** method. Time complexity of the vanilla text-based MAS. C Experiment Setups C.1 Evaluation Details Math Science Reasoning. Commonsense Reasoning. Code Generation. C.2 Implementation Details Software Backend Evaluation protocol. D Additional Experiments D.1 Performance of LatentMAS under Hierarchical MAS Setting D.2 LatentMAS on Llama Backbones D.3 Additional Efficiency Analyses on LatentMAS E Detailed Analyses on LatentMAS E.1 Additional Analyses on Input-Output Alignment E.2 Quantifying Latent Thought Diversity. E.3 Ablations on Latent Reasoning and Communication in LatentMAS F How to Debug LatentMAS? G Additional Discussions on LatentMAS H Additional Related Works I Case Study on Intermediate Error Tracking of LatentMAS J Case Study on LatentMAS K Prompt Template for LatentMAS License: CC BY 4.0 arXiv:2511.20639v3 [cs.CL] 01 Jun 2026 Latent Collaboration in Multi-Agent Systems Jiaru Zou Ruizhong Qiu Gaotang Li…

**Results.** Experiment Setups C.1 Evaluation Details Math Science Reasoning. Commonsense Reasoning. Code Generation. C.2 Implementation Details Software Backend Evaluation protocol. D Additional Experiments D.1 Performance of LatentMAS under Hierarchical MAS Setting D.2 LatentMAS on Llama Backbones D.3 Additional Efficiency Analyses on LatentMAS E Detailed Analyses on LatentMAS E.1 Additional Analyses on Input-Output Alignment E.2 Quantifying Latent Thought Diversity. E.3 Ablations on Latent Reasoning and Communication in LatentMAS F How to Debug LatentMAS? G Additional Discussions on LatentMAS H Additional Related Works I Case Study on Intermediate Error Tracking of LatentMAS J Case Study on LatentMAS K Prompt Template for LatentMAS License: CC BY 4.0 arXiv:2511.20639v3 [cs.CL] 01 Jun 2026 Latent Collaboration in Multi-Agent Systems Jiaru Zou Ruizhong Qiu Gaotang Li Xiyuan Yang…

**Conclusion.** Conclusion References A Input-Output Alignment in LatentMAS A.1 Theoretical Justification on W a W_{a} A.2 Solving the Alignment Matrix W a W_{a} B Theoretical Analysis B.1 Proof of Theorem 3.1 B.2 Proof of Theorem 3.3 Induction step. Induction base case. Conclusion. B.3 Proof of Theorem 3.4 Time complexity of our method. Time complexity of the vanilla text-based MAS. C Experiment Setups C.1 Evaluation Details Math Science Reasoning. Commonsense Reasoning. Code Generation. C.2 Implementation Details Software Backend Evaluation protocol. D Additional Experiments D.1 Performance of LatentMAS under Hierarchical MAS Setting D.2 LatentMAS on Llama Backbones D.3 Addition…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.20639v3.md` · `raw/arxiv/2511.20639v3.fulltext.md`
