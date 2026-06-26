---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Reinforcement Learning with Stochastic Reward Machines"
authors: Jan Corazza, Ivan Gavran, Daniel Neider
url: https://arxiv.org/abs/2510.14837v1
date: 2025-10-16
citationCount: 37
influentialCitationCount: 1
velocity: 4.52
ingested: 2026-06-22
tags: [agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# Reinforcement Learning with Stochastic Reward Machines

**arXiv [2510.14837v1](https://arxiv.org/abs/2510.14837v1)** · 2025-10-16 · **37 citations** (1 influential · 4.52/mo) · Jan Corazza, Ivan Gavran, Daniel Neider

## Abstract
Reward machines are an established tool for dealing with reinforcement learning problems in which rewards are sparse and depend on complex sequences of actions. However, existing algorithms for learning reward machines assume an overly idealized setting where rewards have to be free of noise. To overcome this practical limitation, we introduce a novel type of reward machines, called stochastic reward machines, and an algorithm for learning them. Our algorithm, based on constraint solving, learns minimal stochastic reward machines from the explorations of a reinforcement learning agent. This algorithm can easily be paired with existing reinforcement learning algorithms for reward machines and guarantees to converge to an optimal policy in the limit. We demonstrate the effectiveness of our algorithm in two case studies and show that it outperforms both existing methods and a naive approach for handling noisy reward functions.

## From the paper (full-text excerpts)
**Introduction.** Introduction The key assumption of a reinforcement learning (RL) model is that the reward function is Markovian: the received reward depends only on the agent’s immediate state and action. For many practical RL tasks, however, the most natural conceptualization of the state-space is the one in which the reward function depends on the history of actions that the agent has performed. (Those are typically the tasks in which the agent is rewarded for complex behaviors over a longer period.) An emerging tool used for reinforcement learning in environments with such non-Markovian rewards are reward machines. A reward machine is an automatonlike structure which augments the state space of the environment, capturing the temporal component of rewards. It has been demonstrated that Q-learning [16], ⋆ A shorter version of this paper appeared in the Proceedings of the Thirty-Sixth AAAI Conference on Artificial Intelligence (AAAI-22) [5]. Source code available at https://github.com/corazza/srm. 2 J. Corazza et al. a standard RL algorithm, can be adapted to use and benefit from reward machin…

**Method / approach.** methods and a naive approach for handling noisy reward functions. Keywords: Reinforcement Learning · Reward Machines · Non-Markovian Rewards · SMT Solving · SAT Solving · Stochastic Reward Machines. 1 Introduction The key assumption of a reinforcement learning (RL) model is that the reward function is Markovian: the received reward depends only on the agent’s immediate state and action. For many practical RL tasks, however, the most natural conceptualization of the state-space is the one in which the reward function depends on the history of actions that the agent has performed. (Those are typically the tasks in which the agent is rewarded for complex behaviors over a longer period.) An emerging tool used for reinforcement learning in environments with such non-Markovian rewards are reward machines. A reward machine is an automatonlike structure which augments the state space of the environment, capturing the temporal component of rewards. It has been demonstrated that Q-learning […

**Results.** experimental evaluation, we demonstrate the successful working of our algorithm on two noisy, non-Markovian case studies. We compare our algorithm with existing methods (which do not deal explicitly with noise) on the same case studies: as expected, disregarding the noise by using existing inference algorithms for classical RMs performs substantially worse than our new approach. Finally, we compare our algorithm to a baseline method that tries to “average out” the noise. To summarize, in this paper we 1) introduce stochastic reward machines, 2) present a novel algorithm for learning stochastic reward machines by a RL agent, and 3) experimentally demonstrate the efficacy of our algorithm. 1.1 Related Work Using finite state machines to capture non-Markovian reward functions has been proposed already in the early work on the topic [2]. Toro Icarte et al. [17,18] introduced reward machines (known as Mealy machines in other contexts) as a…

**Conclusion.** Conclusion In this work we introduced Stochastic reward machines as a general way of representing non-Markovian stochastic rewards in RL tasks, and the SRMI algorithm that is able to infer an SRM representation of the environment reward based on traces, and use it to learn the optimal policy. We have shown SRMI is an improvement over prior methods. References 1. Andreas, J., Klein, D., Levine, S.: Modular multitask reinforcement learning with policy sketches. In: ICML’2017. pp. 166–175. JMLR. org (2017) 2. Bacchus, F., Boutilier, C., Grove, A.J.: Rewarding behaviors. In: AAAI/IAAI, Vol. 2. pp. 1160–1167. AAAI Press / The MIT Press (1996) 3. Brafman, R.I., Giacomo, G.D., Patrizi, F.: Ltlf/ldlf non-markovian rewards. In: AAAI. pp. 1771–1778…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2510.14837v1.md` · `raw/arxiv/2510.14837v1.fulltext.md`
