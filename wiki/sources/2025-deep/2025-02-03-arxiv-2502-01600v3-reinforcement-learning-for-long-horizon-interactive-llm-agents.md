---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Reinforcement Learning for Long-Horizon Interactive LLM Agents"
authors: Kevin Chen, Marco Cusumano-Towner, Brody Huval, Aleksei Petrenko et al.
url: https://arxiv.org/abs/2502.01600v3
date: 2025-02-03
citationCount: 76
influentialCitationCount: 7
velocity: 4.59
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Reinforcement Learning for Long-Horizon Interactive LLM Agents

**arXiv [2502.01600v3](https://arxiv.org/abs/2502.01600v3)** · 2025-02-03 · **76 citations** (7 influential · 4.59/mo) · Kevin Chen, Marco Cusumano-Towner, Brody Huval, Aleksei Petrenko et al.

## Abstract
Interactive digital agents (IDAs) leverage APIs of stateful digital environments to perform tasks in response to user requests. While IDAs powered by instruction-tuned large language models (LLMs) can react to feedback from interface invocations in multi-step exchanges, they have not been trained in their respective digital environments. Prior methods accomplish less than half of tasks in sophisticated benchmarks such as AppWorld. We present a reinforcement learning (RL) approach that trains IDAs directly in their target environments. We formalize this training as a partially observable Markov decision process and derive LOOP, a data- and memory-efficient variant of proximal policy optimization. LOOP uses no value network and maintains exactly one copy of the underlying LLM in memory, making its implementation straightforward and as memory-efficient as fine-tuning a single LLM. A 32-billion-parameter agent trained with LOOP in the AppWorld environment outperforms the much larger OpenAI o1 agent by 9 percentage points (15% relative). To our knowledge, this is the first reported application of RL to IDAs that interact with a stateful, multi-domain, multi-app environment via direct API calls. Our analysis sheds light on the effectiveness of RL in this area, showing that the agent learns to consult the API documentation, avoid unwarranted assumptions, minimize confabulation, and recover from setbacks.

## From the paper (full-text excerpts)
**Introduction.** Introduction Consider an interactive digital agent (IDA) faced with the task illustrated in Figure 1. The task spans multiple software apps and requires common-sense knowledge about human life and language. Successful completion requires chains * Equal contribution 1 Apple Inc.. Correspondence to: Kevin Chen <kchen29@apple.com>, Philipp Krähenbühl <philkr@apple.com>. We present a framework for RL with LLM-based IDAs and provide a systematic evaluation of various design choices for policy gradient in this domain. Our best approach, LOOP, 1 Reinforcement Learning for Long-Horizon Interactive LLM Agents Reinforcement learning for LLMs. RL was first used to train LLMs in the setting of reinforcement learning from human feedback (RLHF) (Ziegler et al., 2019; Stiennon et al., 2020; Ouyang et al., 2022). These works used proximal policy optimization (PPO) (Schulman et al., 2017) to train an LLM policy based on a reward model inferred from human preferences. RLHF with PPO uses up to four separate LLMs during training: a reward model, trained policy, reference policy, and critic. Ahmad…

**Method / approach.** methods accomplish less than half of tasks in sophisticated benchmarks such as AppWorld. We present a reinforcement learning (RL) approach that trains IDAs directly in their target environments. We formalize this training as a partially observable Markov decision process and derive LOOP, a data- and memory-efficient variant of proximal policy optimization. LOOP uses no value network and maintains exactly one copy of the underlying LLM in memory, making its implementation straightforward and as memoryefficient as fine-tuning a single LLM. A 32-billionparameter agent trained with LOOP in the AppWorld environment outperforms the much larger OpenAI o1 agent by 9 percentage points (15% relative). To our knowledge, this is the first reported application of RL to IDAs that interact with a stateful, multi-domain, multi-app environment via direct API calls. Our analysis sheds light on the effectiveness of RL in this area, showing that the agent learns to consult the API documentation, avoid un…

**Results.** experiment with per-token (Eq. 5), pertrajectory (Eq. 4), or per-turn importance weights (Figure 2). 1 Mathematically, the environment replays all code from the entire interaction history in the initial environment state, and responds with the output of the code cells most recently submitted. 4 Reinforcement Learning for Long-Horizon Interactive LLM Agents LOOP as REINFORCE Leave-One-Out (Ahmadian et al., 2024). If LOOP is run purely on-policy (Nepoch = 1, no mini-batches), the algorithm reduces to REINFORCE Leave-One-Out (RLOO), since the policy update in PPO (Eq. 5) reduces to REINFORCE (Eq. 2). 5.3. Evaluated Methods We compare our approach with methods outlined below. For each fine-tuned method, we select the highest performing checkpoint according to the validation (dev) set. No fine-tuning (NFT) baselines evaluate on AppWorld zero-shot. We include current open-weight and closedsource SOTA models (Llama 3 70B (Dubey et al.,…

**Conclusion.** conclusion from Table 1 is that all reinforcement-learning-like methods (EI, DPO-MCTS, DMPO, RLOO, GRPO, LOOP) work much better than supervised fine-tuning (RFT, SFT-GT) or prompt engineering. This is surprising, considering the small amount of training data: 24 scenarios, 72 tasks. Surely, capable RL algorithms should overfit to this data. Why don’t they? One of the answers lies in the diversity of rollouts produced by the LLM. Even in late stages of training, a LOOP LLM policy produces a great variety of rollouts. At a micro-level, sampling from an LLM policy encourages small variations and rarely produces the same solution twice. At a macro- 8 Reinforcement Learning for Long-Horizon Interactive LLM Agents References Kim, G., Baldi,…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.01600v3.md` · `raw/arxiv/2502.01600v3.fulltext.md`
