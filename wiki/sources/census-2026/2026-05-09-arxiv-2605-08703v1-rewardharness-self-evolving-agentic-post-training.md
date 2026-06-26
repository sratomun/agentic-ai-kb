---
type: source
source_type: arxiv
title: "RewardHarness: Self-Evolving Agentic Post-Training"
authors: Yuxuan Zhang, Penghui Du, Bo Li, Cong Wei et al.
url: https://arxiv.org/abs/2605.08703v1
date: 2026-05-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [self-evolving-agents, agentic-rl, agent-skills, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# RewardHarness: Self-Evolving Agentic Post-Training

**arXiv:** [2605.08703v1](https://arxiv.org/abs/2605.08703v1) · 2026-05-09 · cs.AI
**Authors:** Yuxuan Zhang, Penghui Du, Bo Li, Cong Wei et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Evaluating instruction-guided image edits requires rewards that reflect subtle human preferences, yet current reward models typically depend on large-scale preference annotation and additional model training. This creates a data-efficiency gap: humans can often infer the target evaluation criteria from only a few examples, while models are usually trained on hundreds of thousands of comparisons. We present RewardHarness, a self-evolving agentic reward framework that reframes reward modeling as context evolution rather than weight optimization. Instead of learning from large-scale annotations, RewardHarness aligns with human preferences by iteratively evolving a library of tools and skills from as few as 100 preference demonstrations. Given a source image, candidate edited images, and an editing instruction, an Orchestrator selects the most relevant subset of tools and skills from the maintained library, and a frozen Sub-Agent uses them to construct a reasoning chain that produces a preference judgment. By comparing predicted judgments with ground-truth preferences and analyzing successes and failures in the reasoning process, the Orchestrator automatically refines its library of tools and skills without additional human annotation. Using only 0.05% of the EditReward preference data, RewardHarness achieves 47.4% average accuracy on image-editing evaluation benchmarks, surpassing GPT-5 by 5.3 points. When used as a reward signal for GRPO fine-tuning, RL-tuned models achieve 3.52 on ImgEdit-Bench. Project page: https://rewardharness.com.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.08703v1)
