---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GLM-4.5: Agentic, Reasoning, and Coding (ARC) Foundation Models"
authors: GLM-4. 5 Team, :, Aohan Zeng, Xin Lv et al.
url: https://arxiv.org/abs/2508.06471v1
date: 2025-08-08
citationCount: 358
influentialCitationCount: 19
velocity: 34.27
ingested: 2026-06-22
tags: [coding-agents, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# GLM-4.5: Agentic, Reasoning, and Coding (ARC) Foundation Models

**arXiv [2508.06471v1](https://arxiv.org/abs/2508.06471v1)** · 2025-08-08 · **358 citations** (19 influential · 34.27/mo) · GLM-4. 5 Team, :, Aohan Zeng, Xin Lv et al.

## Abstract
We present GLM-4.5, an open-source Mixture-of-Experts (MoE) large language model with 355B total parameters and 32B activated parameters, featuring a hybrid reasoning method that supports both thinking and direct response modes. Through multi-stage training on 23T tokens and comprehensive post-training with expert model iteration and reinforcement learning, GLM-4.5 achieves strong performance across agentic, reasoning, and coding (ARC) tasks, scoring 70.1% on TAU-Bench, 91.0% on AIME 24, and 64.2% on SWE-bench Verified. With much fewer parameters than several competitors, GLM-4.5 ranks 3rd overall among all evaluated models and 2nd on agentic benchmarks. We release both GLM-4.5 (355B parameters) and a compact version, GLM-4.5-Air (106B parameters), to advance research in reasoning and agentic AI systems. Code, models, and more information are available at https://github.com/zai-org/GLM-4.5.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large language models (LLMs) are rapidly evolving from general knowledge repositories [6; 37; 50; 33; 23] into general problem-solvers. The ultimate ambition, often associated with Artificial General Intelligence (AGI), is to create models with human-level cognitive capabilities across diverse domains. This requires a unified mastery of complex problem-solving, generalization, and self-improvement, moving beyond task-specific excellence. As LLMs become more integrated into real-world scenarios, the key to enhancing actual productivity and solving complex professional tasks lies in developing specific core capabilities. We identify three critical, interconnected capabilities as the measure of a truly generalist model: Agentic abilities for interacting with external tools and the real world; complex Reasoning for solving multi-step problems in domains like mathematics and science; and advanced Coding skills for tackling realworld software engineering tasks. While state-of-the-art proprietary models like OpenAI’s o1/o3 [18] and Anthropic’s Claude Sonnet 4 have demonstrated…

**Method / approach.** method that supports both thinking and direct response modes. Through multi-stage training on 23T tokens and comprehensive post-training with expert model iteration and reinforcement learning, GLM-4.5 achieves strong performance across agentic, reasoning, and coding (ARC) tasks, scoring 70.1% on TAU-Bench, 91.0% on AIME 24, and 64.2% on SWE-bench Verified. With much fewer parameters than several competitors, GLM-4.5 ranks 3rd overall among all evaluated models and 2nd on agentic benchmarks. We release both GLM-4.5 (355B parameters) and a compact version, GLM-4.5-Air (106B parameters), to advance research in reasoning and agentic AI systems. Code, models, and more information are available at https://github.com/zai-org/GLM-4.5. LLM Performance Evaluation: Agentic, Reasoning, and Coding Benchmarks 12 benchmarks: MMLU-Pro, AIME 24, MATH-500, SciCode, GPQA, HLE, LCB (2407-2501), SWE-Bench Verified, Terminal-Bench, TAU-Bench, BFCL V3, BrowseComp Reasoning Reasoning Benchmarks: MMLU-Pro…

**Results.** experiments showed that models trained with the WSD schedule perform worse on general benchmarks (SimpleQA, MMLU), indicating underfitting in the stable stage. The learning rate went through a warm-up stage from 0 to 2.5e-4 and a decaying stage to 2.5e-5 until the end of mid-training. We used a batch size warmup strategy, where the batch size was gradually increased from 16M tokens to 64M tokens in the training of the first 500B tokens, and remained constant in the remaining of training. For regularization, we set the weight decay ratio to 0.1 and did not use dropout. We set the maximum sequence length to 4,096 during pre-training, and extended it to 32,768 and 131,072 during the mid-training stage as shown in Figure 3. When extending the sequence length to 32K, we also adjusted RoPE’s base frequency from 10,000 to 1,000,000 for better long-context modeling ability. For loss-free balance routing, we set the bias update rate to 0.001 for…

**Conclusion.** conclusions. For code RL, we find that the choice of loss calculation is critical for training efficiency. As illustrated in Figure 7 (left), adopting a token-weighted mean loss is highly beneficial compared to a conventional sequence-mean loss. The token-weighted approach provides a finer-grained and more stable gradient signal, which leads to significantly faster convergence. This method also helps to alleviate the length bias inherent in sequence-level rewards and effectively suppresses the generation of overly simplistic or repetitive “base case” samples during training. For science RL, our findings on the GPQA-Diamond benchmark highlight that data quality and type are paramount factors. As shown in Figure 7 (right), using exclusively e…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]] · [[glm-45]]
- **Raw:** `raw/arxiv/2508.06471v1.md` · `raw/arxiv/2508.06471v1.fulltext.md`
