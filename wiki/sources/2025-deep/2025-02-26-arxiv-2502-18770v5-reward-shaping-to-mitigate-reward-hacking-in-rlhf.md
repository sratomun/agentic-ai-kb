---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Reward Shaping to Mitigate Reward Hacking in RLHF"
authors: Jiayi Fu, Xuandong Zhao, Chengyuan Yao, Heng Wang et al.
url: https://arxiv.org/abs/2502.18770v5
date: 2025-02-26
citationCount: 78
influentialCitationCount: 7
velocity: 4.94
ingested: 2026-06-22
tags: [agent-reliability, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Reward Shaping to Mitigate Reward Hacking in RLHF

**arXiv [2502.18770v5](https://arxiv.org/abs/2502.18770v5)** · 2025-02-26 · **78 citations** (7 influential · 4.94/mo) · Jiayi Fu, Xuandong Zhao, Chengyuan Yao, Heng Wang et al.

## Abstract
Reinforcement Learning from Human Feedback (RLHF) is essential for aligning large language models (LLMs) with human values. However, RLHF is susceptible to \emph{reward hacking}, where the agent exploits flaws in the reward function rather than learning the intended behavior, thus degrading alignment. Although reward shaping helps stabilize RLHF and partially mitigate reward hacking, a systematic investigation into shaping techniques and their underlying principles remains lacking. To bridge this gap, we present a comprehensive study of the prevalent reward shaping methods. Our analysis suggests two key design principles: (1) the RL reward should be bounded, and (2) the RL reward benefits from rapid initial growth followed by gradual convergence. Guided by these insights, we propose Preference As Reward (PAR), a novel approach that leverages the latent preferences embedded within the reward model as the signal for reinforcement learning. Moreover, PAR exhibits two critical variance-reduction properties that contribute to stabilizing the RLHF training process and effectively extending the tolerance window for early stopping. We evaluated PAR on the base model Gemma2-2B using two datasets, Ultrafeedback-Binarized and HH-RLHF. Experimental results demonstrate PAR's superior performance over other reward shaping methods. On the AlpacaEval 2.0 benchmark, PAR achieves a win rate of at least 5 percentage points higher than competing approaches. Furthermore, PAR exhibits remarkable data efficiency, requiring only a single reference reward for optimal performance, and maintains robustness against reward hacking even after two full epochs of training. The code is available at https://github.com/PorUna-byte/PAR.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Method 3.1 Design Principles 3.2 Preference as Reward 3.3 Theoretical Analysis 3.4 Connection to Practice 4 Experiment 4.1 Experimental Setting Datasets and Models Mitigation Baselines Evaluation Metrics Training Details 4.2 Principle One 4.3 Principle Two 4.4 PAR Effectively Mitigates Reward Hacking Reward and Winrate Curve Benchmark Performance 4.5 Data Efficiency and Robustness 4.6 Calibration of Preference Score 5 Discussion 6 Conclusion 7 Limitations 8 Ethical Consideration A Notations B Training Details Dataset Base Models SFT Model Reward Model Policy Model Critic Model Hyper-Parameters C Evaluation C.1 Winrate on Test Set C.2 Benchmark D Gemma2-2B with HH-RLHF E GRPO F Comparison of Some Reward Shaping Techniques G Theoretical Analysis G.1 Bounded Rewards Reduce Return Variance G.2 The Justification of Sigmoid function Probability space and notation. H Case Study I PPO Training Reward Shaping to Mitigate Reward Hacking in RLH…

**Method / approach.** Method 3.1 Design Principles 3.2 Preference as Reward 3.3 Theoretical Analysis 3.4 Connection to Practice 4 Experiment 4.1 Experimental Setting Datasets and Models Mitigation Baselines Evaluation Metrics Training Details 4.2 Principle One 4.3 Principle Two 4.4 PAR Effectively Mitigates Reward Hacking Reward and Winrate Curve Benchmark Performance 4.5 Data Efficiency and Robustness 4.6 Calibration of Preference Score 5 Discussion 6 Conclusion 7 Limitations 8 Ethical Consideration A Notations B Training Details Dataset Base Models SFT Model Reward Model Policy Model Critic Model Hyper-Parameters C Evaluation C.1 Winrate on Test Set C.2 Benchmark D Gemma2-2B with HH-RLHF E GRPO F Comparison of Some Reward Shaping Techniques G Theoretical Analysis G.1 Bounded Rewards Reduce Return Variance G.2 The Justification of Sigmoid function Probability space and notation. H Case Study I…

**Results.** Experiment 4.1 Experimental Setting Datasets and Models Mitigation Baselines Evaluation Metrics Training Details 4.2 Principle One 4.3 Principle Two 4.4 PAR Effectively Mitigates Reward Hacking Reward and Winrate Curve Benchmark Performance 4.5 Data Efficiency and Robustness 4.6 Calibration of Preference Score 5 Discussion 6 Conclusion 7 Limitations 8 Ethical Consideration A Notations B Training Details Dataset Base Models SFT Model Reward Model Policy Model Critic Model Hyper-Parameters C Evaluation C.1 Winrate on Test Set C.2 Benchmark D Gemma2-2B with HH-RLHF E GRPO F Comparison of Some Reward Shaping Techniques G Theoretical Analysis G.1 Bounded Rewards Reduce Return Variance G.2 The Justification of Sigmoid function Probability space and notation. H Case Study I PPO Training Reward Shaping to Mitigate Reward Hacking in RLHF Ji…

**Conclusion.** Conclusion 7 Limitations 8 Ethical Consideration A Notations B Training Details Dataset Base Models SFT Model Reward Model Policy Model Critic Model Hyper-Parameters C Evaluation C.1 Winrate on Test Set C.2 Benchmark D Gemma2-2B with HH-RLHF E GRPO F Comparison of Some Reward Shaping Techniques G Theoretical Analysis G.1 Bounded Rewards Reduce Return Variance G.2 The Justification of Sigmoid function Probability space and notation. H Case Study I PPO Training Reward Shaping to Mitigate Reward Hacking in RLHF Jiayi Fu Xuandong Zhao Chengyuan Yao Heng Wang Qi Han Yanghua Xiao Abstract Reinforcement Learning from Human Feedback (RLHF) is essential for aligning l…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.18770v5.md` · `raw/arxiv/2502.18770v5.fulltext.md`
