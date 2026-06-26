---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Zero-Shot Whole-Body Humanoid Control via Behavioral Foundation Models"
authors: Andrea Tirinzoni, Ahmed Touati, Jesse Farebrother, Mateusz Guzek et al.
url: https://arxiv.org/abs/2504.11054v1
date: 2025-04-15
citationCount: 56
influentialCitationCount: 5
velocity: 3.94
ingested: 2026-06-22
tags: [agentic-rl, arxiv, 2025, cited]
---

# Zero-Shot Whole-Body Humanoid Control via Behavioral Foundation Models

**arXiv [2504.11054v1](https://arxiv.org/abs/2504.11054v1)** · 2025-04-15 · **56 citations** (5 influential · 3.94/mo) · Andrea Tirinzoni, Ahmed Touati, Jesse Farebrother, Mateusz Guzek et al.

## Abstract
Unsupervised reinforcement learning (RL) aims at pre-training agents that can solve a wide range of downstream tasks in complex environments. Despite recent advancements, existing approaches suffer from several limitations: they may require running an RL process on each downstream task to achieve a satisfactory performance, they may need access to datasets with good coverage or well-curated task-specific samples, or they may pre-train policies with unsupervised losses that are poorly correlated with the downstream tasks of interest. In this paper, we introduce a novel algorithm regularizing unsupervised RL towards imitating trajectories from unlabeled behavior datasets. The key technical novelty of our method, called Forward-Backward Representations with Conditional-Policy Regularization, is to train forward-backward representations to embed the unlabeled trajectories to the same latent space used to represent states, rewards, and policies, and use a latent-conditional discriminator to encourage policies to ``cover'' the states in the unlabeled behavior dataset. As a result, we can learn policies that are well aligned with the behaviors in the dataset, while retaining zero-shot generalization capabilities for reward-based and imitation tasks. We demonstrate the effectiveness of this new approach in a challenging humanoid control problem: leveraging observation-only motion capture datasets, we train Meta Motivo, the first humanoid behavioral foundation model that can be prompted to solve a variety of whole-body tasks, including motion tracking, goal reaching, and reward optimization. The resulting model is capable of expressing human-like behaviors and it achieves competitive performance with task-specific methods while outperforming state-of-the-art unsupervised RL and model-based baselines.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries 3 FB with Conditional Policy Regularization 4 Experiments on Humanoid 4.1 Main Results 4.2 Ablations 5 Conclusions 6 Related Work 7 Algorithmic details 8 Experimental Details for the Humanoid Environment 8.1 The SMPL MuJoCo Model 8.2 Data 8.3 Tasks and Metrics 8.3.1 Reward-based evaluation Locomotion. Standing. Handstand. Arm raising. Rotation. Jump. Ground poses. Crawl. 8.3.2 Motion tracking evaluation 8.3.3 Goal-based evaluation 8.4 Training Protocols Online training. Offline training. 8.5 Algorithms Implementation and Parameters 8.5.1 Shared configurations 8.5.2 TD3 8.5.3 FB-CPR 8.5.4 ASE 8.5.5 CALM 8.5.6 PHC 8.5.7 GOAL-GAIL 8.5.8 GOAL-TD3 8.5.9 MPPI 8.5.10 Diffuser 8.5.11 H-GAP 9 Additional Experimental Results 9.1 Detailed Results 9.2 Ablations 9.3 Qualitative Evaluation 9.3.1 Human Evaluation 9.3.2 Reward-based tasks Run. Walking with left hand up. Standing with right foot up. 9.4 Comparison to Unsupervised Skill Discovery…

**Method / approach.** Methods 10 Understanding the Behavioral Latent Space 10.1 Diversity, Dataset Coverage and Transitions 10.2 Dimensionality Reduction of the Behavioral Latent Space 10.3 Behavior Interpolation 11 Ablations on Bipedal Walker 12 Ablations on AntMaze Data. Evaluation. Results. 1]FAIR at Meta 2]Mila, McGill University 3]UCL \contribution [*]Joint first author \contribution [+]Work done at Meta \contribution [†]Joint last author Zero-Shot Whole-Body Humanoid Control via Behavioral Foundation Models Andrea Tirinzoni Ahmed Touati Jesse Farebrother Mateusz Guzek Anssi Kanervisto Yingchen Xu Alessandro Lazaric Matteo Pirotta [ [ [ Abstract Unsupervised reinforcement learning (RL) aims at pre-training agents that can solve a wide range of downstream tasks in complex environments. Despite recent advancements, existing approaches suffer from several limitations: they may require running an RL process on each downstream task to achiev…

**Results.** Experiments on Humanoid 4.1 Main Results 4.2 Ablations 5 Conclusions 6 Related Work 7 Algorithmic details 8 Experimental Details for the Humanoid Environment 8.1 The SMPL MuJoCo Model 8.2 Data 8.3 Tasks and Metrics 8.3.1 Reward-based evaluation Locomotion. Standing. Handstand. Arm raising. Rotation. Jump. Ground poses. Crawl. 8.3.2 Motion tracking evaluation 8.3.3 Goal-based evaluation 8.4 Training Protocols Online training. Offline training. 8.5 Algorithms Implementation and Parameters 8.5.1 Shared configurations 8.5.2 TD3 8.5.3 FB-CPR 8.5.4 ASE 8.5.5 CALM 8.5.6 PHC 8.5.7 GOAL-GAIL 8.5.8 GOAL-TD3 8.5.9 MPPI 8.5.10 Diffuser 8.5.11 H-GAP 9 Additional Experimental Results 9.1 Detailed Results 9.2 Ablations 9.3 Qualitative Evaluation 9.3.1 Human Evaluation 9.3.2 Reward-based tasks Run. Walking with left hand up. Standing wi…

**Conclusion.** Conclusions 6 Related Work 7 Algorithmic details 8 Experimental Details for the Humanoid Environment 8.1 The SMPL MuJoCo Model 8.2 Data 8.3 Tasks and Metrics 8.3.1 Reward-based evaluation Locomotion. Standing. Handstand. Arm raising. Rotation. Jump. Ground poses. Crawl. 8.3.2 Motion tracking evaluation 8.3.3 Goal-based evaluation 8.4 Training Protocols Online training. Offline training. 8.5 Algorithms Implementation and Parameters 8.5.1 Shared configurations 8.5.2 TD3 8.5.3 FB-CPR 8.5.4 ASE 8.5.5 CALM 8.5.6 PHC 8.5.7 GOAL-GAIL 8.5.8 GOAL-TD3 8.5.9 MPPI 8.5.10 Diffuser 8.5.11 H-GAP 9 Additional Experimental Results 9.1 Detailed Results 9.2 Ablations…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]]
- **Raw:** `raw/arxiv/2504.11054v1.md` · `raw/arxiv/2504.11054v1.fulltext.md`
