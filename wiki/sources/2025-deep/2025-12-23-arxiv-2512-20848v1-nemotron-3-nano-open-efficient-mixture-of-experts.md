---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Nemotron 3 Nano: Open, Efficient Mixture-of-Experts Hybrid Mamba-Transformer Model for Agentic Reasoning"
authors: NVIDIA, :, Aaron Blakeman, Aaron Grattafiori et al.
url: https://arxiv.org/abs/2512.20848v1
date: 2025-12-23
citationCount: 48
influentialCitationCount: 7
velocity: 8.07
ingested: 2026-06-22
tags: [agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Nemotron 3 Nano: Open, Efficient Mixture-of-Experts Hybrid Mamba-Transformer Model for Agentic Reasoning

**arXiv [2512.20848v1](https://arxiv.org/abs/2512.20848v1)** · 2025-12-23 · **48 citations** (7 influential · 8.07/mo) · NVIDIA, :, Aaron Blakeman, Aaron Grattafiori et al.

## Abstract
We present Nemotron 3 Nano 30B-A3B, a Mixture-of-Experts hybrid Mamba-Transformer language model. Nemotron 3 Nano was pretrained on 25 trillion text tokens, including more than 3 trillion new unique tokens over Nemotron 2, followed by supervised fine tuning and large-scale RL on diverse environments. Nemotron 3 Nano achieves better accuracy than our previous generation Nemotron 2 Nano while activating less than half of the parameters per forward pass. It achieves up to 3.3x higher inference throughput than similarly-sized open models like GPT-OSS-20B and Qwen3-30B-A3B-Thinking-2507, while also being more accurate on popular benchmarks. Nemotron 3 Nano demonstrates enhanced agentic, reasoning, and chat abilities and supports context lengths up to 1M tokens. We release both our pretrained Nemotron 3 Nano 30B-A3B Base and post-trained Nemotron 3 Nano 30B-A3B checkpoints on Hugging Face.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Pretraining 2.1 Model Architecture 2.2 Pretraining Data 2.2.1 Nemotron-CC-Code-v1 2.2.2 Nemotron-Pretraining-Code-v2 2.2.3 Nemotron-CC-v2.1 2.2.4 Nemotron-Pretraining-Specialized-v1 2.3 Data Mixture and Ordering 2.4 Hyperparameters 2.5 Long-Context Extension 2.6 Base Model Evaluations 3 Post-Training 3.1 Supervised Fine Tuning 3.1.1 Chat Template 3.1.2 Data 3.1.3 Data Filtering 3.1.4 Data Mixture 3.1.5 Reasoning Control 3.1.6 Hyperparameters 3.2 Multi environment Reinforcement Learning from Verifiable Rewards 3.2.1 Environments 3.2.2 Data Mixture and Curriculum 3.2.3 Surpassing SFT with RLVR 3.2.4 Infrastructure 3.2.5 Algorithm 3.3 Reinforcement Learning from Human Feedback 3.3.1 Scaling Reinforcement Learning for Generative Reward‑Model Training 3.3.2 RLHF with Group Relative Length Control Length-Normalized Reward Adjustment. Quality-Gated Conciseness Bonus. 3.4 Post-trained Model Evaluations 3.4.1 Evaluation Benchmarks 4 Quantization 4.1 Post-Training Quantization Calibr…

**Method / approach.** method reliably recovered complete code snippets and technical context at scale. 2.2.2 Nemotron-Pretraining-Code-v2 We sourced additional code from GitHub for repositories we identified as missing from our existing corpus in addition to collecting recent data with a cut-off date of April 15, 2025. We used the same pipeline as described in NVIDIA ( 2025d ) to curate the data and we remove exact and near-duplicate files already present in our existing corpus. In addition to our raw source-code corpus, we synthetically generated additional mixed natural-language and source code documents using the Qwen3 32B LLM. Similar to our approach described in NVIDIA ( 2025e ) , we prompted the model to generate question and answer pairs using our new source-code data as seeds. Additionally, we prompted the model to generate student-teacher (Python only) and code-review (Python/C++) style dialogue grounded with a combination of code snippets and full source files. Following the code-rew…

**Results.** Evaluations 3 Post-Training 3.1 Supervised Fine Tuning 3.1.1 Chat Template 3.1.2 Data 3.1.3 Data Filtering 3.1.4 Data Mixture 3.1.5 Reasoning Control 3.1.6 Hyperparameters 3.2 Multi environment Reinforcement Learning from Verifiable Rewards 3.2.1 Environments 3.2.2 Data Mixture and Curriculum 3.2.3 Surpassing SFT with RLVR 3.2.4 Infrastructure 3.2.5 Algorithm 3.3 Reinforcement Learning from Human Feedback 3.3.1 Scaling Reinforcement Learning for Generative Reward‑Model Training 3.3.2 RLHF with Group Relative Length Control Length-Normalized Reward Adjustment. Quality-Gated Conciseness Bonus. 3.4 Post-trained Model Evaluations 3.4.1 Evaluation Benchmarks 4 Quantization 4.1 Post-Training Quantization Calibration Dataset 4.2 Selective Post-Training Quantization 4.3 Accuracy and Throughput 5 Conclusion A Base model evaluations B MMLU-redux evaluation C DPO for Re…

**Conclusion.** Conclusion A Base model evaluations B MMLU-redux evaluation C DPO for Reducing Tool Hallucination D Safety Preference Data E Prompt Sensitivity Analysis Nemotron 3 Nano: Open, Efficient Mixture-of-Experts Hybrid Mamba-Transformer Model for Agentic Reasoning NVIDIA Abstract Abstract. We present Nemotron 3 Nano 30B-A3B, a Mixture-of-Experts hybrid Mamba-Transformer language model. Nemotron 3 Nano was pretrained on 25 trillion text tokens, including more than 3 trillion new unique tokens over Nemotron 2, followed by supervised fine tuning and large-scale RL on diverse environments. Nemotron 3 Nano achieves better accuracy than our previous generation Nemotron 2 Nano while activating less than half of the parameters per f…

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2512.20848v1.md` · `raw/arxiv/2512.20848v1.fulltext.md`
