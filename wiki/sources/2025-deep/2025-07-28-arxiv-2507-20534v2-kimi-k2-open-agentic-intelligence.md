---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Kimi K2: Open Agentic Intelligence"
authors: Kimi Team, Yifan Bai, Yiping Bao, Y. Charles et al.
url: https://arxiv.org/abs/2507.20534v2
date: 2025-07-28
citationCount: 296
influentialCitationCount: 37
velocity: 27.39
ingested: 2026-06-22
tags: [coding-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# Kimi K2: Open Agentic Intelligence

**arXiv [2507.20534v2](https://arxiv.org/abs/2507.20534v2)** · 2025-07-28 · **296 citations** (37 influential · 27.39/mo) · Kimi Team, Yifan Bai, Yiping Bao, Y. Charles et al.

## Abstract
We introduce Kimi K2, a Mixture-of-Experts (MoE) large language model with 32 billion activated parameters and 1 trillion total parameters. We propose the MuonClip optimizer, which improves upon Muon with a novel QK-clip technique to address training instability while enjoying the advanced token efficiency of Muon. Based on MuonClip, K2 was pre-trained on 15.5 trillion tokens with zero loss spike. During post-training, K2 undergoes a multi-stage post-training process, highlighted by a large-scale agentic data synthesis pipeline and a joint reinforcement learning (RL) stage, where the model improves its capabilities through interactions with real and synthetic environments. Kimi K2 achieves state-of-the-art performance among open-source non-thinking models, with strengths in agentic capabilities. Notably, K2 obtains 66.1 on Tau2-Bench, 76.5 on ACEBench (En), 65.8 on SWE-Bench Verified, and 47.3 on SWE-Bench Multilingual -- surpassing most open and closed-sourced baselines in non-thinking settings. It also exhibits strong capabilities in coding, mathematics, and reasoning tasks, with a score of 53.7 on LiveCodeBench v6, 49.5 on AIME 2025, 75.1 on GPQA-Diamond, and 27.1 on OJBench, all without extended thinking. These results position Kimi K2 as one of the most capable open-source large language models to date, particularly in software engineering and agentic tasks. We release our base and post-trained model checkpoints to facilitate future research and applications of agentic intelligence.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Pre-training 2.1 MuonClip: Stable Training with Weight Clipping Training instability when scaling Muon Taming Muon with QK-Clip MuonClip: The New Optimizer 2.2 Pre-training Data: Improving Token Utility with Rephrasing Knowledge Data Rephrasing Mathematics Data Rephrasing Pre-training Data Overall 2.3 Model Architecture Sparsity Scaling Law Number of Attention Heads 2.4 Training Infrastructure 2.4.1 Compute Cluster 2.4.2 Parallelism for Model Scaling EP communication overlap with interleaved 1F1B Smaller EP size 2.4.3 Activation Reduction Selective recomputation FP8 storage for insensitive activations Activation CPU offload 2.5 Training recipe 3 Post-Training 3.1 Supervised Fine-Tuning 3.1.1 Large-Scale Agentic Data Synthesis for Tool Use Learning Domain Evolution and Tool Generation. Agent Diversification. Rubric-Based Task Generation. Multi-turn Trajectory Generation. Quality Evaluation and Filtering. Hybrid Approach with Real Execution Environments. 3.2 Reinforcement Learning…

**Method / approach.** method mitigates implicit output length limitations that typically exist with LLMs. An overview of this pipeline is presented in Figure 4 . • Fidelity verification: To ensure consistency between original and rewritten content, we perform fidelity checks that compare the semantic alignment of each rephrased passage with its source. This serves as an initial quality control step prior to training. We compare data rephrasing with multi-epoch repetition by testing their corresponding accuracy on SimpleQA. We experiment with an early checkpoint of K2 and evaluate three training strategies: (1) repeating the original dataset for 10 epochs, (2) rephrasing the data once and repeating it for 10 epochs, and (3) rephrasing the data 10 times with a single training pass. As shown in Table 1 , the accuracy consistently improves across these strategies, demonstrating the efficacy of our rephrasing-based augmentation. We extended this method to other large-scale knowledge corpora and obse…

**Results.** Experiment Settings 4.3.2 Safety Evaluation Results 5 Limitations 6 Conclusions 7 Acknowledgments A Contributions B Token Template of Tool Calling C Evaluation Details Coding Tasks. Tool Use Tasks. Math STEM Logical Tasks. General Tasks. Long Context and Factuality Tasks. Open-Ended Evaluation D QK-Clip Does Not Impair Model Quality Small-Scale Ablations Self-deactivation E Why Muon is More Prone to Logit Explosion Structural difference in updates SVD formulation Attention-specific amplification F K2 Critic Rubrics for General RL F.1 Core Rubrics F.2 Prescriptive Rubrics F.3 Limitations G Engine Switching Pipeline for RL Training Theoretical three-stage pipeline. Two-stage pipeline due to PCIe saturation. Kimi K2: Open Agentic Intelligence Kimi Team Abstract We introduce Kimi K2, a Mixture-of-Experts (MoE) large language model with 32 billion activated para…

**Conclusion.** Conclusions 7 Acknowledgments A Contributions B Token Template of Tool Calling C Evaluation Details Coding Tasks. Tool Use Tasks. Math STEM Logical Tasks. General Tasks. Long Context and Factuality Tasks. Open-Ended Evaluation D QK-Clip Does Not Impair Model Quality Small-Scale Ablations Self-deactivation E Why Muon is More Prone to Logit Explosion Structural difference in updates SVD formulation Attention-specific amplification F K2 Critic Rubrics for General RL F.1 Core Rubrics F.2 Prescriptive Rubrics F.3 Limitations G Engine Switching Pipeline for RL Training Theoretical three-stage pipeline. Two-stage pipeline due to PCIe saturation. Kimi K2: Open Agentic Intelligence…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]] · [[kimi-k2]]
- **Raw:** `raw/arxiv/2507.20534v2.md` · `raw/arxiv/2507.20534v2.fulltext.md`
