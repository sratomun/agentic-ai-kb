---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Reinforcement Learning with Action Chunking"
authors: Qiyang Li, Zhiyuan Zhou, Sergey Levine
url: https://arxiv.org/abs/2507.07969v4
date: 2025-07-10
citationCount: 71
influentialCitationCount: 16
velocity: 6.23
ingested: 2026-06-22
tags: [embodied-agents, agentic-rl, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Reinforcement Learning with Action Chunking

**arXiv [2507.07969v4](https://arxiv.org/abs/2507.07969v4)** · 2025-07-10 · **71 citations** (16 influential · 6.23/mo) · Qiyang Li, Zhiyuan Zhou, Sergey Levine

## Abstract
We present Q-chunking, a simple yet effective recipe for improving reinforcement learning (RL) algorithms for long-horizon, sparse-reward tasks. Our recipe is designed for the offline-to-online RL setting, where the goal is to leverage an offline prior dataset to maximize the sample-efficiency of online learning. Effective exploration and sample-efficient learning remain central challenges in this setting, as it is not obvious how the offline data should be utilized to acquire a good exploratory policy. Our key insight is that action chunking, a technique popularized in imitation learning where sequences of future actions are predicted rather than a single action at each timestep, can be applied to temporal difference (TD)-based RL methods to mitigate the exploration challenge. Q-chunking adopts action chunking by directly running RL in a 'chunked' action space, enabling the agent to (1) leverage temporally consistent behaviors from offline data for more effective online exploration and (2) use unbiased $n$-step backups for more stable and efficient TD learning. Our experimental results demonstrate that Q-chunking exhibits strong offline performance and online sample efficiency, outperforming prior best offline-to-online methods on a range of long-horizon, sparse-reward manipulation tasks.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Background 4 Q-Chunking 4.1 Q-learning on a temporally extended action space 4.2 Behavior constraints for temporally coherent exploration 4.3 Practical implementations 5 Experimental Results 5.1 Environments and Datasets 5.2 Comparisons 5.3 How well does our method compare to prior offline-to-online RL methods? 5.4 Why does action chunking help exploration? 5.5 How does action chunk length, critic ensemble size, and UTD ratio affect performance? 6 Discussions References A Theoretical Justification B Domain Details B.1 OGBench environments. B.2 Robomimic environments. C Implementation Details C.1 QC-FQL C.2 FQL C.3 FQL-n C.4 QC C.5 RLPD , RLPD-AC , QC-RLPD C.6 SUPE-GT D Experiment Details D.1 Computational resources D.2 Evaluation protocol D.3 Hyperparameter tuning E Full Results E.1 End-effector visualization E.2 OGBench results by individual task E.3 Robomimic ablation results E.4 How resource efficient is Q-chunking? License: arXiv.org perpetual non-exclusive li…

**Method / approach.** method compare to prior offline-to-online RL methods? 5.4 Why does action chunking help exploration? 5.5 How does action chunk length, critic ensemble size, and UTD ratio affect performance? 6 Discussions References A Theoretical Justification B Domain Details B.1 OGBench environments. B.2 Robomimic environments. C Implementation Details C.1 QC-FQL C.2 FQL C.3 FQL-n C.4 QC C.5 RLPD , RLPD-AC , QC-RLPD C.6 SUPE-GT D Experiment Details D.1 Computational resources D.2 Evaluation protocol D.3 Hyperparameter tuning E Full Results E.1 End-effector visualization E.2 OGBench results by individual task E.3 Robomimic ablation results E.4 How resource efficient is Q-chunking? License: arXiv.org perpetual non-exclusive license arXiv:2507.07969v4 [cs.LG] 11 May 2026 Reinforcement Learning with Action Chunking Qiyang Li, Zhiyuan Zhou, Sergey Levine UC Berkeley {qcli,zhiyuan_zhou,svlevine}@eecs.berkeley.edu Abstract We…

**Results.** Experimental Results 5.1 Environments and Datasets 5.2 Comparisons 5.3 How well does our method compare to prior offline-to-online RL methods? 5.4 Why does action chunking help exploration? 5.5 How does action chunk length, critic ensemble size, and UTD ratio affect performance? 6 Discussions References A Theoretical Justification B Domain Details B.1 OGBench environments. B.2 Robomimic environments. C Implementation Details C.1 QC-FQL C.2 FQL C.3 FQL-n C.4 QC C.5 RLPD , RLPD-AC , QC-RLPD C.6 SUPE-GT D Experiment Details D.1 Computational resources D.2 Evaluation protocol D.3 Hyperparameter tuning E Full Results E.1 End-effector visualization E.2 OGBench results by individual task E.3 Robomimic ablation results E.4 How resource efficient is Q-chunking? License: arXiv.org perpetual non-exclusive license arXiv:2507.07969v4 [cs.LG] 11 May 2026 Reinforcement Learni…

**Conclusion.** Discussions References A Theoretical Justification B Domain Details B.1 OGBench environments. B.2 Robomimic environments. C Implementation Details C.1 QC-FQL C.2 FQL C.3 FQL-n C.4 QC C.5 RLPD , RLPD-AC , QC-RLPD C.6 SUPE-GT D Experiment Details D.1 Computational resources D.2 Evaluation protocol D.3 Hyperparameter tuning E Full Results E.1 End-effector visualization E.2 OGBench results by individual task E.3 Robomimic ablation results E.4 How resource efficient is Q-chunking? License: arXiv.org perpetual non-exclusive license arXiv:2507.07969v4 [cs.LG] 11 May 2026 Reinforcement Learning with Action Chunking Qiyang Li, Zhiyuan Zhou, Sergey Levine UC Berkeley {qcli,zhiyuan_z…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.07969v4.md` · `raw/arxiv/2507.07969v4.fulltext.md`
