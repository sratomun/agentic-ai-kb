---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "LLaDA-MoE: A Sparse MoE Diffusion Language Model"
authors: Fengqi Zhu, Zebin You, Yipeng Xing, Zenan Huang et al.
url: https://arxiv.org/abs/2509.24389v1
date: 2025-09-29
citationCount: 38
influentialCitationCount: 3
velocity: 4.35
ingested: 2026-06-22
tags: [coding-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# LLaDA-MoE: A Sparse MoE Diffusion Language Model

**arXiv [2509.24389v1](https://arxiv.org/abs/2509.24389v1)** · 2025-09-29 · **38 citations** (3 influential · 4.35/mo) · Fengqi Zhu, Zebin You, Yipeng Xing, Zenan Huang et al.

## Abstract
We introduce LLaDA-MoE, a large language diffusion model with the Mixture-of-Experts (MoE) architecture, trained from scratch on approximately 20T tokens. LLaDA-MoE achieves competitive performance with significantly reduced computational overhead by maintaining a 7B-parameter capacity while activating only 1.4B parameters during inference. Our empirical evaluation reveals that LLaDA-MoE achieves state-of-the-art performance among diffusion language models with larger parameters, surpassing previous diffusion language models LLaDA, LLaDA 1.5, and Dream across multiple benchmarks. The instruct-tuned model LLaDA-MoE-7B-A1B-Instruct demonstrates capabilities comparable to Qwen2.5-3B-Instruct in knowledge understanding, code generation, mathematical reasoning, agent and alignment tasks, despite using fewer active parameters. Our results show that integrating a sparse MoE architecture into the training objective of masked diffusion language models still brings out MoE's strengths under efficient inference with few active parameters, and opens ample room for further exploration of diffusion language models. LLaDA-MoE models are available at Huggingface.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Diffusion Language Models 2.2 The MoE Architecture 3 LLaDA-MoE 3.1 Overview 3.2 Training and Inference for LLaDA-MoE 4 Experiments 5 Conclusion \useunder \ul † † footnotetext: † Corresponding Authors. ‡ Team Leaders. ∗ Core Contributors. LLaDA-MoE: A Sparse MoE Diffusion Language Model Fengqi Zhu 1,2,∗ Zebin You 1,2,∗ Yipeng Xing 2,∗ Zenan Huang 2,∗ Lin Liu 2,∗ Yihong Zhuang 2,∗ Guoshan Lu 2,∗ Kangyu Wang 2,3 Xudong Wang 2 Lanning Wei 2 Hongrui Guo 2 Jiaqi Hu 2,4 Wentao Ye 2,4 Tieyuan Chen 2,3 Chenchen Li 2 Chengfu Tang 2 Haibo Feng 2 Jun Hu 2 Jun Zhou 2 Xiaolu Zhang 2,‡ Zhenzhong Lan 2,‡ Junbo Zhao 2,4,‡ Da Zheng 2,‡ Chongxuan Li 1,† Jianguo Li 2,† Ji-Rong Wen 1,† 1 Renmin University of China, 2 Ant Group, 3 Shanghai Jiao Tong University, 4 Zhejiang University Abstract We introduce LLaDA-MoE, a large language diffusion model with the Mixture-of-Experts (MoE) architecture, trained from scratch on approximately 20T tokens. LLaDA-MoE a…

**Method / approach.** Method Pretrain Pretrain Continue Pretrain Pretrain # Total Params 7B 8B 7B 3B # Activated Params 1B 8B 7B 3B General Tasks MMLU 64.59 65.90 69.50 67.98 MMLU-Pro 39.16 41.80 48.15 35.50 CEval 65.56 70.50 59.18 75.00 CMMLU 65.65 69.90 60.87 73.65 RACE 84.96 88.37 44.70 87.88 Reasoning Tasks BBH 52.71 49.80 57.90 56.50 Drop 65.86 72.93 75.16 51.61 KorBench 31.20 33.68 37.44 27.44 Math Tasks GSM8K 66.41 70.70 77.79 78.17 MATH 36.10 27.30 39.60 40.94 OlympiadBench 10.07 6.85 10.22 9.33 Coding Tasks CRUX-O 39.00 31.00 37.75 35.62 MBPP 52.40 38.20 56.20 69.56 MultiPL-E 41.13 23.61 27.60 40.80 HumanEval 45.73 33.50 57.90 57.93 LiveCodeBench v6 16.18 2.53 14.87 16.99 BigCodeBench-Full 21.23 13.42 18.33 30.88 Avg 46.94 43.53 46.66 50.…

**Results.** Experiments 5 Conclusion \useunder \ul † † footnotetext: † Corresponding Authors. ‡ Team Leaders. ∗ Core Contributors. LLaDA-MoE: A Sparse MoE Diffusion Language Model Fengqi Zhu 1,2,∗ Zebin You 1,2,∗ Yipeng Xing 2,∗ Zenan Huang 2,∗ Lin Liu 2,∗ Yihong Zhuang 2,∗ Guoshan Lu 2,∗ Kangyu Wang 2,3 Xudong Wang 2 Lanning Wei 2 Hongrui Guo 2 Jiaqi Hu 2,4 Wentao Ye 2,4 Tieyuan Chen 2,3 Chenchen Li 2 Chengfu Tang 2 Haibo Feng 2 Jun Hu 2 Jun Zhou 2 Xiaolu Zhang 2,‡ Zhenzhong Lan 2,‡ Junbo Zhao 2,4,‡ Da Zheng 2,‡ Chongxuan Li 1,† Jianguo Li 2,† Ji-Rong Wen 1,† 1 Renmin University of China, 2 Ant Group, 3 Shanghai Jiao Tong University, 4 Zhejiang University Abstract We introduce LLaDA-MoE, a large language diffusion model with the Mixture-of-Experts (MoE) architecture, trained from scratch on approximately 20T tokens. LLaDA-MoE achieves competitive per…

**Conclusion.** Conclusion \useunder \ul † † footnotetext: † Corresponding Authors. ‡ Team Leaders. ∗ Core Contributors. LLaDA-MoE: A Sparse MoE Diffusion Language Model Fengqi Zhu 1,2,∗ Zebin You 1,2,∗ Yipeng Xing 2,∗ Zenan Huang 2,∗ Lin Liu 2,∗ Yihong Zhuang 2,∗ Guoshan Lu 2,∗ Kangyu Wang 2,3 Xudong Wang 2 Lanning Wei 2 Hongrui Guo 2 Jiaqi Hu 2,4 Wentao Ye 2,4 Tieyuan Chen 2,3 Chenchen Li 2 Chengfu Tang 2 Haibo Feng 2 Jun Hu 2 Jun Zhou 2 Xiaolu Zhang 2,‡ Zhenzhong Lan 2,‡ Junbo Zhao 2,4,‡ Da Zheng 2,‡ Chongxuan Li 1,† Jianguo Li 2,† Ji-Rong Wen 1,† 1 Renmin University of China, 2 Ant Group, 3 Shanghai Jiao Tong University, 4 Zhejiang University Abstract We in…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2509.24389v1.md` · `raw/arxiv/2509.24389v1.fulltext.md`
