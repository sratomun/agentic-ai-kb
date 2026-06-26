---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Scaling Laws for Reward Model Overoptimization"
authors: Leo Gao et al.
url: https://arxiv.org/abs/2210.10760
date: 2022-10-19
ingested: 2026-06-22
tags: [arxiv, reward-modeling, post-training]
---

# Scaling Laws for Reward Model Overoptimization

**arXiv [2210.10760](https://arxiv.org/abs/2210.10760)** · 2022-10-19 · Leo Gao, John Schulman, Jacob Hilton (OpenAI)

**Significance.** Puts Goodhart's law on a curve. The first careful measurement of reward-model overoptimization — RLHF's central failure mode — yielding clean, predictive scaling laws for how far a learned reward can be safely optimized before true performance degrades.

## Abstract
In reinforcement learning from human feedback, it is common to optimize against a reward model trained to predict human preferences. Because the reward model is an imperfect proxy, optimizing its value too much can hinder ground truth performance, in accordance with Goodhart's law. This effect has been frequently observed, but not carefully measured due to the expense of collecting human preference data. In this work, we use a synthetic setup in which a fixed "gold-standard" reward model plays the role of humans, providing labels used to train a proxy reward model. We study how the gold reward model score changes as we optimize against the proxy reward model using either reinforcement learning or best-of-n sampling. We find that this relationship follows a different functional form depending on the method of optimization, and that in both cases its coefficients scale smoothly with the number of reward model parameters. We also study the effect on this relationship of the size of the reward model dataset, the number of reward model and policy parameters, and the coefficient of the KL penalty added to the reward in the reinforcement learning setup. We explore the implications of these empirical results for theoretical considerations in AI alignment.

## From the paper (full-text)
**Contribution / method.** A synthetic setup sidesteps expensive human labels: a fixed 6B "gold" reward model (from InstructGPT, Ouyang et al. 2022) plays the role of humans and deterministically labels pairs of policy rollouts, producing 100,000 synthetic comparisons (10% held out) used to train a proxy RM. Proxy RMs range from 3M to 3B parameters. The policy is then optimized against the proxy RM via either best-of-n (BoN) sampling or PPO reinforcement learning, and the gold RM score is tracked as a function of KL distance from the initial policy. Because KL is a quadratic distance, results are written in terms of d := √(KL); for BoN, KL is computed analytically as log n − (n−1)/n.

**Results.** The gold score R follows distinct functional forms by optimization method (with R(0):=0):
- Best-of-n: **R_bon(d) = d(α_bon − β_bon·d)**
- RL: **R_RL(d) = d(α_RL − β_RL·log d)**

The BoN form, hypothesized on data up to n=1,000 (KL≈6 nats), held as a true advance prediction up to n=60,000 (KL≈10 nats). Coefficients vary smoothly with proxy-RM size (logarithmic trends); notably α_RL is nearly independent of RM parameter count, so a single scaling curve in β_RL captures RL overoptimization, and max BoN gold score is α_bon/2β_bon. RM dataset size matters sharply: below ~2,000 comparisons there is almost no improvement over chance; above it, more unique data (not more SGD steps) reduces goodharting. Policy size has only weak dependence — larger policies (1.2B vs 6B) score higher and benefit less from optimization but do not overoptimize more, peaking at nearly the same KL. The KL penalty in PPO does not shift the KL–gold frontier (it acts like early stopping) and widens the proxy–gold gap, so it was set to 0 elsewhere. The α term is interpreted as regressional Goodhart, the β term (which drives nonmonotonicity and unbounded utility loss) as extremal Goodhart.

**Takeaway.** Overoptimizing an imperfect proxy reward is measurable and predictable — quadratic-in-√KL for best-of-n, logarithmic for RL — and the coefficients improve smoothly with reward-model size, letting you forecast how hard a learned reward can be pushed before ground-truth performance turns down.

## Graph
- **Concepts:** [[reward-modeling|Reward modeling]]
- **Entities:** [[rlhf]] · [[openai]] · [[ppo]]
- **Raw:** `raw/arxiv/2210.10760.fulltext.md`
