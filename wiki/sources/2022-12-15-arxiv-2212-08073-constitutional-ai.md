---
type: source
source_type: arxiv
kind: deep
depth: report
title: "Constitutional AI: Harmlessness from AI Feedback"
authors: Yuntao Bai et al.
url: https://arxiv.org/abs/2212.08073
date: 2022-12-15
ingested: 2026-06-22
tags: [arxiv, constitutional-ai, post-training]
---

# Constitutional AI: Harmlessness from AI Feedback

**arXiv [2212.08073](https://arxiv.org/abs/2212.08073)** · 2022-12-15 · Yuntao Bai, Saurav Kadavath, Sandipan Kundu, Amanda Askell, et al. (Anthropic)

**Significance.** The founding method of RLAIF and the "constitution" idea: train a harmless-but-not-evasive assistant using AI-generated feedback against written principles, with essentially no human harm labels in the RL stage. The recipe behind Claude's alignment.

> **Capture note.** alphaXiv full-text extraction timed out repeatedly for this paper; this note is built from the verbatim abstract plus alphaXiv's structured report (raw/arxiv/2212.08073.fulltext.md), not the verbatim paper body. The method and qualitative findings below are grounded in that report; specific quantitative figures from the paper body were not available and are deliberately not asserted here.

## Abstract
As AI systems become more capable, we would like to enlist their help to supervise other AIs. We experiment with methods for training a harmless AI assistant through self-improvement, without any human labels identifying harmful outputs. The only human oversight is provided through a list of rules or principles, and so we refer to the method as 'Constitutional AI'. The process involves both a supervised learning and a reinforcement learning phase. In the supervised phase we sample from an initial model, then generate self-critiques and revisions, and then finetune the original model on revised responses. In the RL phase, we sample from the finetuned model, use a model to evaluate which of the two samples is better, and then train a preference model from this dataset of AI preferences. We then train with RL using the preference model as the reward signal, i.e. we use 'RL from AI Feedback' (RLAIF). As a result we are able to train a harmless but non-evasive AI assistant that engages with harmful queries by explaining its objections to them. Both the SL and RL methods can leverage chain-of-thought style reasoning to improve the human-judged performance and transparency of AI decision making. These methods make it possible to control AI behavior more precisely and with far fewer human labels.

## From the paper (full-text)
**Contribution / method.** Constitutional AI (CAI) is a two-stage pipeline that replaces human harm labels with a written "constitution" of natural-language principles. (1) Supervised stage (SL-CAI): a helpful-only model responds to harmful prompts, then critiques and revises its own response against a sampled constitutional principle, iterating multiple rounds; the base model is fine-tuned on the revised responses. (2) RL stage (RL-CAI / RLAIF): the SL-CAI model generates response pairs to harmful prompts, an AI model picks which better satisfies the constitution, those AI preferences train a preference model, and RL optimizes the policy against it. Both stages can use chain-of-thought reasoning to make the critique/evaluation more transparent and accurate.

**Results.** (Qualitative, from the alphaXiv report — exact paper-body numbers were not retrievable.) CAI with chain-of-thought reasoning achieves a Pareto improvement over standard RLHF on the harmlessness/helpfulness frontier, producing models that are both more harmless and less evasive. RLAIF-trained models match or exceed RLHF on harmlessness. AI labelers identify harmful content more accurately as model size grows, especially with chain-of-thought. Each critique-revision round progressively reduces harmfulness with diminishing returns after ~2–3 rounds; even 1–2 constitutional principles yield significant improvement, though more principles help. Critiqued revisions outperform direct revisions.

**Takeaway.** You can train a harmless, non-evasive assistant largely from AI feedback against written principles — replacing expensive human harm labels with a scalable self-critique + RLAIF loop, and breaking the usual harmlessness-vs-helpfulness tradeoff.

## Graph
- **Concepts:** [[constitutional-ai|Constitutional AI]]
- **Entities:** [[anthropic]] · [[rlhf]] · [[chain-of-thought]]
- **Raw:** `raw/arxiv/2212.08073.fulltext.md`
