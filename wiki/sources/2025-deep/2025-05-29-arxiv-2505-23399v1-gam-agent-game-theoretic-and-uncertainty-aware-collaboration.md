---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GAM-Agent: Game-Theoretic and Uncertainty-Aware Collaboration for Complex Visual Reasoning"
authors: Jusheng Zhang, Yijia Fan, Wenjun Lin, Ruiqi Chen et al.
url: https://arxiv.org/abs/2505.23399v1
date: 2025-05-29
citationCount: 64
influentialCitationCount: 1
velocity: 5.01
ingested: 2026-06-22
tags: [agent-reliability, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# GAM-Agent: Game-Theoretic and Uncertainty-Aware Collaboration for Complex Visual Reasoning

**arXiv [2505.23399v1](https://arxiv.org/abs/2505.23399v1)** · 2025-05-29 · **64 citations** (1 influential · 5.01/mo) · Jusheng Zhang, Yijia Fan, Wenjun Lin, Ruiqi Chen et al.

## Abstract
We propose GAM-Agent, a game-theoretic multi-agent framework for enhancing vision-language reasoning. Unlike prior single-agent or monolithic models, GAM-Agent formulates the reasoning process as a non-zero-sum game between base agents--each specializing in visual perception subtasks--and a critical agent that verifies logic consistency and factual correctness. Agents communicate via structured claims, evidence, and uncertainty estimates. The framework introduces an uncertainty-aware controller to dynamically adjust agent collaboration, triggering multi-round debates when disagreement or ambiguity is detected. This process yields more robust and interpretable predictions. Experiments on four challenging benchmarks--MMMU, MMBench, MVBench, and V*Bench--demonstrate that GAM-Agent significantly improves performance across various VLM backbones. Notably, GAM-Agent boosts the accuracy of small-to-mid scale models (e.g., Qwen2.5-VL-7B, InternVL3-14B) by 5--6\%, and still enhances strong models like GPT-4o by up to 2--3\%. Our approach is modular, scalable, and generalizable, offering a path toward reliable and explainable multi-agent multimodal reasoning.

## From the paper (full-text excerpts)
**Introduction.** Introduction Recently, large language models (LLMs) [43, 31, 2, 19, 49, 52] has made significant progress in tasks such as complex reasoning, code generation, and knowledge integration, overcoming the limitations of single models through multi-agent collaboration [66, 11, 28, 33, 4]. In contrast, although there have been advances in integrating visual perception with language understanding in the field of vision language models (VLMs) [42, 27, 6, 10, 9], the potential of multi-agent collaboration for VLMs remains largely untapped. Most existing VLM approaches rely on single models or simple ensemble strategies, which struggle to address challenges like multi-step reasoning and visual ambiguity in complex visual reasoning tasks [17, 10]. Benefiting from the development of multi-agent systems [8, 54, 7], some recent studies have proposed multi-agent debate frameworks to compensate for the shortcomings of VLMs and have obtained promising results[55, 11, 56, 25]. However, these methods typically adopt simple mechanisms such as averaging or voting mechanisms and lack visual reasoningbase…

**Method / approach.** methods typically adopt simple mechanisms such as averaging or voting mechanisms and lack visual reasoningbased strategic interactions between agents [54, 18]. Hence, they perform poorly in high-complexity visual reasoning scenarios (e.g., MMMU [63]). Just as human experts reach consensus through strategic game-like interactions when they disagree [47, 45, 57, 3], introducing a deep collaborative game-theoretic mechanism into complex visual reasoning is a valuable endeavor[13], which has already seen preliminary applications in some LLM-based works [33, 51]. However, current collaborative game-theoretic methods are often highly complex and heavily rely on reasoning paths, clues, and the fusion of multiple information, making them difficult to apply Preprint. Under review. directly to visual reasoning [53, 14, 12]. To address this issue, this paper explores the underlying architecture of existing VLMs, effectively utilizes important intermediate results in the reasoning process, and…

**Results.** Experiments on four challenging benchmarks—MMMU, MMBench, MVBench, and V*Bench—demonstrate that GAM-Agent significantly improves performance across various VLM backbones. Notably, GAM-Agent boosts the accuracy of small-to-mid scale models (e.g., Qwen2.5-VL-7B, InternVL3-14B) by 5–6%, and still enhances strong models like GPT-4o by up to 2–3%. Our approach is modular, scalable, and generalizable, offering a path toward reliable and explainable multi-agent multimodal reasoning. 1 Introduction Recently, large language models (LLMs) [43, 31, 2, 19, 49, 52] has made significant progress in tasks such as complex reasoning, code generation, and knowledge integration, overcoming the limitations of single models through multi-agent collaboration [66, 11, 28, 33, 4]. In contrast, although there have been advances in integrating visual perception with language understanding in the field of vision language models (VLMs) [42, 27, 6, 10, 9], the p…

**Conclusion.** conclusions presented. With these two tiers of expert agents, our GAM-Agent introduces an iterative game-theoretic interplay and information refinement process via uncertainty quantification to perform robust and accurate visual reasoning. 2.2 Uncertainty Quantification Function (Φ) We propose a dual-level Φi that models uncertainty from both response generation and overall semantics. Generation-Process Based Uncertainty (Φigen+ ) When the probability distribution Pi,t of the underlying VLM during the generation of the token sequence Yi = (yi,1 , . . . , yi,Ti ) is accessible, we propose an integrated multi-feature uncertainty metric Φigen+ (Ri )   T Φigen+ (Ri ) = i  1 X α · Ti t=1  H(Pi,t ) | {z } Information Entropy (Hesitation)…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2505.23399v1.md` · `raw/arxiv/2505.23399v1.fulltext.md`
