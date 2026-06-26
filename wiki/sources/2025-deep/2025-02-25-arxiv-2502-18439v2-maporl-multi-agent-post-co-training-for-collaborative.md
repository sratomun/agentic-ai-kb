---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MAPoRL: Multi-Agent Post-Co-Training for Collaborative Large Language Models with Reinforcement Learning"
authors: Chanwoo Park, Seungju Han, Xingzhi Guo, Asuman Ozdaglar et al.
url: https://arxiv.org/abs/2502.18439v2
date: 2025-02-25
citationCount: 75
influentialCitationCount: 3
velocity: 4.74
ingested: 2026-06-22
tags: [agentic-rl, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# MAPoRL: Multi-Agent Post-Co-Training for Collaborative Large Language Models with Reinforcement Learning

**arXiv [2502.18439v2](https://arxiv.org/abs/2502.18439v2)** · 2025-02-25 · **75 citations** (3 influential · 4.74/mo) · Chanwoo Park, Seungju Han, Xingzhi Guo, Asuman Ozdaglar et al.

## Abstract
Leveraging multiple large language models (LLMs) to build collaborative multi-agentic workflows has demonstrated significant potential. However, most previous studies focus on prompting the out-of-the-box LLMs, relying on their innate capability for collaboration, which may not improve LLMs' performance as shown recently. In this paper, we introduce a new post-training paradigm MAPoRL (Multi-Agent Post-co-training for collaborative LLMs with Reinforcement Learning), to explicitly elicit the collaborative behaviors and further unleash the power of multi-agentic LLM frameworks. In MAPoRL, multiple LLMs first generate their own responses independently and engage in a multi-turn discussion to collaboratively improve the final answer. In the end, a MAPoRL verifier evaluates both the answer and the discussion, by assigning a score that verifies the correctness of the answer, while adding incentives to encourage corrective and persuasive discussions. The score serves as the co-training reward, and is then maximized through multi-agent RL. Unlike existing LLM post-training paradigms, MAPoRL advocates the co-training of multiple LLMs together using RL for better generalization. Accompanied by analytical insights, our experiments demonstrate that training individual LLMs alone is insufficient to induce effective collaboration. In contrast, multi-agent co-training can boost the collaboration performance across benchmarks, with generalization to unseen domains.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Analytical Insights: Collaborate to Solve Hard Questions 2.1 Problem Setup 2.2 Analytical Observations 2.3 Toy Experiments with T = 10 , 20 𝑇 10 20 T=10,20 italic_T = 10 , 20 Turns 3 Post-Co-Training with MARL 3.1 Multi-Agent System - Collaborative Debate Formulation 3.2 Multi-Agent RL Formulation 3.3 Reward Shaping to Incentivize Collaboration 4 Experiments 4.1 Datasets GSM8K (Cobbe et al., 2021 ) and TinyGSM (Liu et al., 2023 ) . Adversarial Natural Language Inference (ANLI) (Nie et al., 2020 ) . Evaluation Method. 4.2 Models 4.3 Experiment 1: Vanilla Collaboration by Off-the-shelf LLMs Cannot Improve Performance, While \ours -Trained LLMs Can 4.4 Experiment 2: Reward Shaping with Collaboration Incentives Analysis of α 0 subscript 𝛼 0 \alpha_{0} italic_α start_POSTSUBSCRIPT 0 end_POSTSUBSCRIPT and α 1 subscript 𝛼 1 \alpha_{1} italic_α start_POSTSUBSCRIPT 1 end_POSTSUBSCRIPT . Analysis of β 0 subscript 𝛽 0 \beta_{0} italic_β start_POSTSUBSCRIPT 0 end_POSTSUBSCRIPT and β 1 subscript 𝛽 1 \beta_{1} italic_β start_POSTS…

**Method / approach.** Method. 4.2 Models 4.3 Experiment 1: Vanilla Collaboration by Off-the-shelf LLMs Cannot Improve Performance, While \ours -Trained LLMs Can 4.4 Experiment 2: Reward Shaping with Collaboration Incentives Analysis of α 0 subscript 𝛼 0 \alpha_{0} italic_α start_POSTSUBSCRIPT 0 end_POSTSUBSCRIPT and α 1 subscript 𝛼 1 \alpha_{1} italic_α start_POSTSUBSCRIPT 1 end_POSTSUBSCRIPT . Analysis of β 0 subscript 𝛽 0 \beta_{0} italic_β start_POSTSUBSCRIPT 0 end_POSTSUBSCRIPT and β 1 subscript 𝛽 1 \beta_{1} italic_β start_POSTSUBSCRIPT 1 end_POSTSUBSCRIPT . 4.5 Experiment 3: Collaboration Ability Acquired by \ours Is Transferable 4.6 Experiment 4: MAPoRL with Heterogeneous LLMs Can Help 4.7 Experiment 5: Naïve Supervised Fine-Tuning Using High-Quality Collaboration Samples May Not Induce Collaborative Behaviors 5 Concluding Remarks, Limitations, and Potential Risks A Detailed Related Work Discussion Multi-Agent Reinforcement Learning. Multi-Agent Collaboration with…

**Results.** Experiments with T = 10 , 20 𝑇 10 20 T=10,20 italic_T = 10 , 20 Turns 3 Post-Co-Training with MARL 3.1 Multi-Agent System - Collaborative Debate Formulation 3.2 Multi-Agent RL Formulation 3.3 Reward Shaping to Incentivize Collaboration 4 Experiments 4.1 Datasets GSM8K (Cobbe et al., 2021 ) and TinyGSM (Liu et al., 2023 ) . Adversarial Natural Language Inference (ANLI) (Nie et al., 2020 ) . Evaluation Method. 4.2 Models 4.3 Experiment 1: Vanilla Collaboration by Off-the-shelf LLMs Cannot Improve Performance, While \ours -Trained LLMs Can 4.4 Experiment 2: Reward Shaping with Collaboration Incentives Analysis of α 0 subscript 𝛼 0 \alpha_{0} italic_α start_POSTSUBSCRIPT 0 end_POSTSUBSCRIPT and α 1 subscript 𝛼 1 \alpha_{1} italic_α start_POSTSUBSCRIPT 1 end_POSTSUBSCRIPT . Analysis of β 0 subscript 𝛽 0 \beta_{0} italic_β start_POSTSUBSCRIPT 0 end_POSTSUBSCRIPT and β 1 subscript 𝛽 1 \beta_{1} italic_β…

**Conclusion.** Discussion Multi-Agent Reinforcement Learning. Multi-Agent Collaboration with LLMs. RL for LLM Training. B Additional Literature Review Multi-Agent RL. Teaching LLM Self-Correction. Multi-Agent LLMs with Game Theory. C Deferred Content of Section 2 D Deferred Details in Section 2.3 Choices of R col ⁢ ( q ) , R ind ⁢ ( q ) , R syn ⁢ ( q ) , C ⁢ ( q ) subscript 𝑅 col 𝑞 subscript 𝑅 ind 𝑞 subscript 𝑅 syn 𝑞 𝐶 𝑞 R_{\text{col}}(q),R_{\text{ind}}(q),R_{\text{syn}}(q),C(q) italic_R start_POSTSUBSCRIPT col end_POSTSUBSCRIPT ( italic_q ) , italic_R start_POSTSUBSCRIPT ind end_POSTSUBSCRIPT ( italic_q ) , italic_R start_POSTSUBSCRIPT syn end_POSTSUBSCRIPT ( italic_q ) , italic_C ( italic_q ) . E Deferred Details of…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.18439v2.md` · `raw/arxiv/2502.18439v2.fulltext.md`
