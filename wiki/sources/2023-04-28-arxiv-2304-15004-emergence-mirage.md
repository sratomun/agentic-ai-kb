---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Are Emergent Abilities of Large Language Models a Mirage?"
authors: Rylan Schaeffer et al.
url: https://arxiv.org/abs/2304.15004
date: 2023-04-28
citationCount: omit
tags: [arxiv, scaling-laws]
---

# Are Emergent Abilities of Large Language Models a Mirage?

**arXiv [2304.15004](https://arxiv.org/abs/2304.15004)** · 2023-04-28 · Rylan Schaeffer et al. (Stanford)

**Significance.** Argues emergence is largely an artifact of the researcher's choice of nonlinear/discontinuous metric — swap the metric and the sharp jump dissolves into a smooth curve.

## Abstract
Recent work claims that large language models display emergent abilities, abilities not present in smaller-scale models that are present in larger-scale models. What makes emergent abilities intriguing is two-fold: their sharpness, transitioning seemingly instantaneously from not present to present, and their unpredictability, appearing at seemingly unforeseeable model scales. Here, we present an alternative explanation for emergent abilities: that for a particular task and model family, when analyzing fixed model outputs, emergent abilities appear due the researcher's choice of metric rather than due to fundamental changes in model behavior with scale. Specifically, nonlinear or discontinuous metrics produce apparent emergent abilities, whereas linear or continuous metrics produce smooth, continuous, predictable changes in model performance. We present our alternative explanation in a simple mathematical model, then test it in three complementary ways: we (1) make, test and confirm three predictions on the effect of metric choice using the InstructGPT/GPT-3 family on tasks with claimed emergent abilities, (2) make, test and confirm two predictions about metric choices in a meta-analysis of emergent abilities on BIG-Bench; and (3) show how to choose metrics to produce never-before-seen seemingly emergent abilities in multiple vision tasks across diverse deep networks. Via all three analyses, we provide evidence that alleged emergent abilities evaporate with different metrics or with better statistics, and may not be a fundamental property of scaling AI models.

## From the paper (full-text)
**Contribution / method.** Posit that when per-token cross-entropy falls smoothly as a power law with scale, a nonlinear metric (Accuracy: all L tokens correct, ≈exp(−(N/c)^α)^L decays geometrically) or a discontinuous metric (Multiple Choice Grade, a step) manufactures apparent emergence, while a linear metric (Token Edit Distance) or continuous one (Brier Score) reveals a smooth curve. Tested three ways.

**Results.** (1) On the InstructGPT/GPT-3 family (350M, 1.3B, 6.7B, 175B) doing 2-shot multiplication and 4-digit addition: emergence appears under Accuracy at 4–5 digit targets, but switching to Token Edit Distance makes performance smooth and predictable; adding test data shows even small models score above chance (accuracy decays geometrically with target length, as predicted). (2) Meta-analysis of BIG-Bench: of 39 preferred metrics, at most 5 show emergence; hand-annotated data shows emergence under only 4/39 metrics, and >92% of claimed emergent abilities appear under just two — Multiple Choice Grade (discontinuous) and Exact String Match (nonlinear). For LaMDA, emergence under Multiple Choice Grade disappears under continuous Brier Score. (3) The authors induce never-before-seen "emergent" abilities in vision nets (autoencoders on CIFAR100, transformers on Omniglot, LeNet on MNIST) purely by redefining the metric as subset accuracy. They also flag a multiple-comparisons issue: BIG-Bench has ≥220 tasks × ~40 metrics × ~10 model families ≈ 10^6 triplets.

**Takeaway.** Emergence may be a measurement artifact, not a fundamental scaling property — though the authors stress this doesn't prove LLMs cannot have genuine emergent abilities.

## Graph
- **Concepts:** [[scaling-laws|Scaling laws]]
- **Entities:** GPT-3, InstructGPT, LaMDA, BIG-Bench, Stanford
- **Raw:** `raw/arxiv/2304.15004.fulltext.md`
