---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Acting Less is Reasoning More! Teaching Model to Act Efficiently"
authors: Hongru Wang, Cheng Qian, Wanjun Zhong, Xiusi Chen et al.
url: https://arxiv.org/abs/2504.14870v2
date: 2025-04-21
citationCount: 62
influentialCitationCount: 6
velocity: 4.42
ingested: 2026-06-22
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, 2025, cited]
---

# Acting Less is Reasoning More! Teaching Model to Act Efficiently

**arXiv [2504.14870v2](https://arxiv.org/abs/2504.14870v2)** · 2025-04-21 · **62 citations** (6 influential · 4.42/mo) · Hongru Wang, Cheng Qian, Wanjun Zhong, Xiusi Chen et al.

## Abstract
Tool-integrated reasoning (TIR) augments large language models (LLMs) with the ability to invoke external tools during long-form reasoning, such as search engines and code interpreters, to solve tasks beyond the capabilities of internal reasoning. While reinforcement learning (RL) has shown promise in training such agents, most of existing approaches typically optimize only for final correctness without considering the efficiency or necessity of external tool use. This often leads to excessive tool calling, incurring high computational costs and hindering the development of internal reasoning capabilities - a phenomenon known as \textit{cognitive offloading}. To this end, we propose Optimal Tool Call-controlled Policy Optimization (OTC-PO), a simple yet effective RL-based framework that encourages models to produce accurate answers with minimal tool calls. Our method introduces a tool-integrated reward that jointly considers answer correctness and corresponding tool use behavior of model to reach that answer. To validate the effectiveness, we introduce the metric of \textit{tool productivity}, defined as the ratio between the number of correct answers and the total number of tool calls across all test cases. This metric reflects how efficiently tool usage contributes to successful task completion, with higher values indicating smarter and more autonomous reasoning. We instantiate this framework within both Proximal Policy Optimization (PPO) and Group Relative Preference Optimization (GRPO), resulting in OTC-PPO and OTC-GRPO. Experiments with Qwen-2.5 and Qwen-Math across multiple QA benchmarks show that our approach reduces tool calls by up to 68.3\% and improves tool productivity by up to 215.4\%, while maintaining comparable answer accuracy.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Tool Utilization for LLMs. Tool-integrated Reasoning Efficiency. 3 Methodology 3.1 Task Definition 3.2 Tool-integrated Reinforcement Learning Reward Design. 3.3 OTC-PO: Optimal Tool Call-controlled Policy Optimization OTC-PPO. OTC-GRPO. Tool-integrated Reward Design. 4 Experiments 4.1 Set up Datasets and Baselines. Evaluation Metrics. Implementation Details. 4.2 Main Results Search as Tool. Code as Tool. 5 Analysis 5.1 Tool Use Behavior Analysis Training. Inference. 5.2 Out-of-domain Evaluation 5.3 Case Study 6 Conclusion and Future Work A Related Work Reward Shaping in RL. B Tool-integrated Reinforcement Learning PPO in TRL. GRPO in TRL. C Search Template D Reward Function D.1 Figure Illustration D.2 Theoretical Justification D.3 Generalization of Reward E Analysis of Search as Tool E.1 Base v.s. Instruct Model E.2 The Effects of α 𝛼 \alpha italic_α F Analysis of Code as Tool F.1 The Effects of C 𝐶 C italic_C Acting Less is Rea…

**Method / approach.** Methodology 3.1 Task Definition 3.2 Tool-integrated Reinforcement Learning Reward Design. 3.3 OTC-PO: Optimal Tool Call-controlled Policy Optimization OTC-PPO. OTC-GRPO. Tool-integrated Reward Design. 4 Experiments 4.1 Set up Datasets and Baselines. Evaluation Metrics. Implementation Details. 4.2 Main Results Search as Tool. Code as Tool. 5 Analysis 5.1 Tool Use Behavior Analysis Training. Inference. 5.2 Out-of-domain Evaluation 5.3 Case Study 6 Conclusion and Future Work A Related Work Reward Shaping in RL. B Tool-integrated Reinforcement Learning PPO in TRL. GRPO in TRL. C Search Template D Reward Function D.1 Figure Illustration D.2 Theoretical Justification D.3 Generalization of Reward E Analysis of Search as Tool E.1 Base v.s. Instruct Model E.2 The Effects of α 𝛼 \alpha italic_α F Analysis of Code as Tool F.1 The Effects of C 𝐶 C italic_C Acting Less is Reasoning…

**Results.** Experiments 4.1 Set up Datasets and Baselines. Evaluation Metrics. Implementation Details. 4.2 Main Results Search as Tool. Code as Tool. 5 Analysis 5.1 Tool Use Behavior Analysis Training. Inference. 5.2 Out-of-domain Evaluation 5.3 Case Study 6 Conclusion and Future Work A Related Work Reward Shaping in RL. B Tool-integrated Reinforcement Learning PPO in TRL. GRPO in TRL. C Search Template D Reward Function D.1 Figure Illustration D.2 Theoretical Justification D.3 Generalization of Reward E Analysis of Search as Tool E.1 Base v.s. Instruct Model E.2 The Effects of α 𝛼 \alpha italic_α F Analysis of Code as Tool F.1 The Effects of C 𝐶 C italic_C Acting Less is Reasoning More ! Teaching Model to Act Efficiently Hongru Wang α , Cheng Qian β , Wanjun Zhong δ , Xiusi Chen β , Jiahao Qiu σ , Shijue Huang μ , Bowen Jin β , Mengdi Wang σ , Kam-Fai…

**Conclusion.** Conclusion and Future Work A Related Work Reward Shaping in RL. B Tool-integrated Reinforcement Learning PPO in TRL. GRPO in TRL. C Search Template D Reward Function D.1 Figure Illustration D.2 Theoretical Justification D.3 Generalization of Reward E Analysis of Search as Tool E.1 Base v.s. Instruct Model E.2 The Effects of α 𝛼 \alpha italic_α F Analysis of Code as Tool F.1 The Effects of C 𝐶 C italic_C Acting Less is Reasoning More ! Teaching Model to Act Efficiently Hongru Wang α , Cheng Qian β , Wanjun Zhong δ , Xiusi Chen β , Jiahao Qiu σ , Shijue Huang μ , Bowen Jin β , Mengdi Wang σ , Kam-Fai Wong α , Heng Ji β α The Chinese University of Hong Kong, β University of Illinois U…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]] · [[ppo]] · [[qwen]]
- **Raw:** `raw/arxiv/2504.14870v2.md` · `raw/arxiv/2504.14870v2.fulltext.md`
