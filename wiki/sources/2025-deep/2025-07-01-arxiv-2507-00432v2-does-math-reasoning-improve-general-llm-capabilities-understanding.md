---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Does Math Reasoning Improve General LLM Capabilities? Understanding Transferability of LLM Reasoning"
authors: Maggie Huan, Yuetai Li, Tuney Zheng, Xiaoyu Xu et al.
url: https://arxiv.org/abs/2507.00432v2
date: 2025-07-01
citationCount: 89
influentialCitationCount: 18
velocity: 7.61
ingested: 2026-06-22
tags: [agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Does Math Reasoning Improve General LLM Capabilities? Understanding Transferability of LLM Reasoning

**arXiv [2507.00432v2](https://arxiv.org/abs/2507.00432v2)** · 2025-07-01 · **89 citations** (18 influential · 7.61/mo) · Maggie Huan, Yuetai Li, Tuney Zheng, Xiaoyu Xu et al.

## Abstract
Math reasoning has become the poster child of progress in large language models (LLMs), with new models rapidly surpassing human-level performance on benchmarks like MATH and AIME. But as math leaderboards improve week by week, it is worth asking: do these gains reflect broader problem-solving ability or just narrow overfitting? To answer this question, we evaluate over 20 open-weight reasoning-tuned models across a broad suite of tasks, including math, scientific QA, agent planning, coding, and standard instruction-following. We surprisingly find that most models that succeed in math fail to transfer their gains to other domains. To rigorously study this phenomenon, we conduct controlled experiments on Qwen3-14B models using math-only data but different tuning methods. We find that reinforcement learning (RL)-tuned models generalize well across domains, while supervised fine-tuning (SFT)-tuned models often forget general capabilities. Latent-space representation and token-space distribution shift analyses reveal that SFT induces substantial representation and output drift, while RL preserves general-domain structure. Our results suggest a need to rethink standard post-training recipes, particularly the reliance on SFT-distilled data for advancing reasoning models.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Phenomena: Performance Discrepancies of Reasoning Models 2.1 Observed Performance Discrepancies Between RL and SFT Results. 2.2 Control Study 3 Latent Representation Shifts: Insights from PCA Analysis 3.1 Experimental Setup 3.2 Investigating Latent Space Shift 4 Token Distribution Shifts: Insights from KL Divergence and Rank Analyses 4.1 Setup 4.2 Result 5 Ablation: Which Components of RL Drive Generalization? 5.1 Contrasting Objectives 5.2 Ablation Results 5.3 Related Works 6 Conclusion A Appendix A.1 The Use of Large Language Models A.2 Detailed Evidence of Our Observed Phenomena A.3 Full Evaluation Setup A.3.1 Post-training Methods A.3.2 Training Datasets A.3.3 Baselines A.3.4 Evaluation Benchmarks Math Reasoning Datasets Other Reasoning Datasets Non-reasoning Datasets A.3.5 Evaluation metrics A.4 PCA Analysis under Varying Settings A.5 Details on Ablation Study A.5.1 Gradient Norm of SFT and RL A.5.2 Response Length of online RL and online SFT A.6 Token Distribution S…

**Method / approach.** Methods A.3.2 Training Datasets A.3.3 Baselines A.3.4 Evaluation Benchmarks Math Reasoning Datasets Other Reasoning Datasets Non-reasoning Datasets A.3.5 Evaluation metrics A.4 PCA Analysis under Varying Settings A.5 Details on Ablation Study A.5.1 Gradient Norm of SFT and RL A.5.2 Response Length of online RL and online SFT A.6 Token Distribution Shifts A.6.1 Case study and details A.6.2 Details about the result analysis A.7 Breakdown Evaluation Results Does Math Reasoning Improve General LLM Capabilities? Understanding Transferability of LLM Reasoning Maggie Huan 1,2 Yuetai Li 3 1 1 footnotemark: 1 Tuney Zheng 4 1 1 footnotemark: 1 Xiaoyu Xu 5 Seungone Kim 1 Minxin Du 5 Radha Poovendran 3 Graham Neubig 1 Xiang Yue 1 1 Carnegie Mellon University 2 University of Pennsylvania 3 University of Washington 4 M-A-P 5 The Hong Kong Polytechnic University ziyuh@seas.upenn.edu, yuetaili@uw.edu, xyue2@andrew.cmu.edu Eq…

**Results.** Experimental Setup 3.2 Investigating Latent Space Shift 4 Token Distribution Shifts: Insights from KL Divergence and Rank Analyses 4.1 Setup 4.2 Result 5 Ablation: Which Components of RL Drive Generalization? 5.1 Contrasting Objectives 5.2 Ablation Results 5.3 Related Works 6 Conclusion A Appendix A.1 The Use of Large Language Models A.2 Detailed Evidence of Our Observed Phenomena A.3 Full Evaluation Setup A.3.1 Post-training Methods A.3.2 Training Datasets A.3.3 Baselines A.3.4 Evaluation Benchmarks Math Reasoning Datasets Other Reasoning Datasets Non-reasoning Datasets A.3.5 Evaluation metrics A.4 PCA Analysis under Varying Settings A.5 Details on Ablation Study A.5.1 Gradient Norm of SFT and RL A.5.2 Response Length of online RL and online SFT A.6 Token Distribution Shifts A.6.1 Case study and details A.6.2 Details about the result analysis A.7 Br…

**Conclusion.** Conclusion A Appendix A.1 The Use of Large Language Models A.2 Detailed Evidence of Our Observed Phenomena A.3 Full Evaluation Setup A.3.1 Post-training Methods A.3.2 Training Datasets A.3.3 Baselines A.3.4 Evaluation Benchmarks Math Reasoning Datasets Other Reasoning Datasets Non-reasoning Datasets A.3.5 Evaluation metrics A.4 PCA Analysis under Varying Settings A.5 Details on Ablation Study A.5.1 Gradient Norm of SFT and RL A.5.2 Response Length of online RL and online SFT A.6 Token Distribution Shifts A.6.1 Case study and details A.6.2 Details about the result analysis A.7 Breakdown Evaluation Results Does Math Reasoning Improve General LLM Capabilities? Understanding Tran…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2507.00432v2.md` · `raw/arxiv/2507.00432v2.fulltext.md`
