---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Direct Preference Optimization: Your Language Model is Secretly a Reward Model"
authors: Rafael Rafailov et al.
url: https://arxiv.org/abs/2305.18290
date: 2023-05-29
ingested: 2026-06-22
tags: [arxiv, reward-modeling, post-training]
---

# Direct Preference Optimization: Your Language Model is Secretly a Reward Model

**arXiv [2305.18290](https://arxiv.org/abs/2305.18290)** · 2023-05-29 · Rafael Rafailov, Archit Sharma, Eric Mitchell, Stefano Ermon, Christopher D. Manning, Chelsea Finn (Stanford University)

**Significance.** Collapses RLHF into a single classification loss. DPO derives the optimal policy in closed form, eliminating the separate reward model and the RL sampling loop entirely — yet matches or beats PPO-RLHF. Became the default open-source preference-tuning method.

## Abstract
While large-scale unsupervised language models (LMs) learn broad world knowledge and some reasoning skills, achieving precise control of their behavior is difficult due to the completely unsupervised nature of their training. Existing methods for gaining such steerability collect human labels of the relative quality of model generations and fine-tune the unsupervised LM to align with these preferences, often with reinforcement learning from human feedback (RLHF). However, RLHF is a complex and often unstable procedure, first fitting a reward model that reflects the human preferences, and then fine-tuning the large unsupervised LM using reinforcement learning to maximize this estimated reward without drifting too far from the original model. In this paper we introduce a new parameterization of the reward model in RLHF that enables extraction of the corresponding optimal policy in closed form, allowing us to solve the standard RLHF problem with only a simple classification loss. The resulting algorithm, which we call Direct Preference Optimization (DPO), is stable, performant, and computationally lightweight, eliminating the need for sampling from the LM during fine-tuning or performing significant hyperparameter tuning. Our experiments show that DPO can fine-tune LMs to align with human preferences as well as or better than existing methods. Notably, fine-tuning with DPO exceeds PPO-based RLHF in ability to control sentiment of generations, and matches or improves response quality in summarization and single-turn dialogue while being substantially simpler to implement and train.

## From the paper (full-text)
**Contribution / method.** DPO starts from the same KL-constrained reward-maximization objective as RLHF, whose optimal policy has a known closed form π_r(y|x) = (1/Z(x))·π_ref(y|x)·exp((1/β)r(x,y)). Rearranging gives the reward in terms of the optimal policy, r(x,y) = β·log[π_r(y|x)/π_ref(y|x)] + β·log Z(x). Because the Bradley-Terry preference model depends only on the *difference* of rewards between two completions, the intractable partition function Z(x) cancels, yielding a loss expressed purely over policies — the DPO loss: L_DPO = −E[log σ(β·log(π_θ(y_w|x)/π_ref(y_w|x)) − β·log(π_θ(y_l|x)/π_ref(y_l|x)))]. The implicit reward is r̂_θ(x,y) = β·log[π_θ(y|x)/π_ref(y|x)]. This change-of-variables avoids fitting a standalone reward model and needs no sampling from the LM during fine-tuning; the per-example gradient up-weights examples where the implicit reward is most wrong, preventing degeneration.

**Results.** Across three tasks — IMDb sentiment (GPT-2-large), Reddit TL;DR summarization (GPT-J ≈6B), and Anthropic-HH single-turn dialogue (Pythia-2.8B) — DPO matches or beats PPO-RLHF. On the sentiment reward–KL frontier, DPO strictly dominates PPO and beats even PPO with ground-truth rewards. On TL;DR summarization (GPT-4-judged win rate vs reference), DPO reaches ≈61% at temperature 0.0 vs PPO's 57%, and is far more robust to sampling temperature; head-to-head, DPO at temp 0.25 was preferred 58% over PPO at temp 0. On Anthropic-HH, DPO is the only computationally efficient method that improves over the preferred completions, matching/beating Best-of-128. Under distribution shift (CNN/DailyMail, GPT-4 win rate, temp 0): DPO 0.36 vs PPO 0.26. A human study validated the GPT-4 judge — GPT-4 agreed with humans about as often as humans agreed with each other (e.g. DPO human win rate 58%).

**Takeaway.** You can solve the RLHF objective with a single binary-cross-entropy loss over policies — no reward model, no RL loop, no sampling during training — and still match or exceed PPO-based RLHF. The LM is "secretly" its own reward model.

## Graph
- **Concepts:** [[reward-modeling|Reward modeling]]
- **Entities:** [[dpo]] · [[rlhf]] · [[ppo]]
- **Raw:** `raw/arxiv/2305.18290.fulltext.md`
