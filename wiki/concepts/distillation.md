---
type: concept
tags: [agents, frontier-models, distillation, efficiency]
created: 2026-06-22
updated: 2026-06-22
kind: domain
---

# Distillation

*Transferring a large model's capability into a smaller one by training the student on the teacher's outputs — how frontier capability gets compressed into deployable, cheap-to-run models.*

## What it is
A teacher→student transfer: a small model is trained to mimic a larger model's outputs (logits, or generated reasoning traces and answers), inheriting much of its capability at a fraction of the size and serving cost. In the LLM era the dominant form is *data distillation* — generate high-quality outputs from a strong model and SFT a smaller one on them ([[synthetic-data]] is the mechanism). Borders [[open-models]] (most distilled open releases) and [[post-training]] (distillation is often a post-training route).

## Why it matters
Distillation is the deployment economics of the frontier: it's how a 671B reasoning model becomes a 7B model you can actually run in production. The 2025 finding that reset expectations: for small models, **distilling from a strong teacher beats running RL on the small model directly** — capability flows down cheaper than it can be grown bottom-up. For the exec that means the practical play for most teams isn't training frontier models, it's distilling them — and it's why a single strong open release (DeepSeek-R1) instantly seeded a family of small, capable models.

## What the evidence shows
**Foundations.** The teacher-student idea is Hinton, Vinyals & Dean (arXiv:1503.02531); sequence-level KD adapted it to generation (arXiv:1606.07947); DistilBERT showed it at language-model scale (arXiv:1910.01108). The headline modern result is DeepSeek-R1, which open-sourced six dense models (1.5B–70B) distilled from the 671B reasoner and showed distillation beats small-model RL (arXiv:2501.12948).

**Recent developments.** The distillation-vs-RL trade-off and the "$42 distilled-plus-RL small model" result are walked through in [[2025-02-05-blog-raschka-understanding-reasoning-llms]] and [[2025-04-19-blog-raschka-state-of-rl-for-llm-reasoning]]; the open question of how far distillation scales is flagged in [[2025-01-21-blog-lambert-deepseek-r1-recipe]].

## Relationships
- stage of [[frontier-model-training]]; uses [[synthetic-data]]; often a [[post-training]] route
- produces small models for [[open-models]], [[reasoning-models]]
- the dominant way [[small-language-models]] are produced (teacher→student)
- efficiency lever behind cheap intent classifiers / routers in [[intent-understanding]], [[intent-routing]]
- exemplified by [[deepseek]]
- explained by [[sebastian-raschka]], [[nathan-lambert]]

## Key papers (full-text ingested)
- [[2026-06-22-arxiv-1503-02531-distilling-knowledge|Distilling the Knowledge (Hinton)]] — soft targets at temperature; transfers >80% of an ensemble's gain
- [[2026-06-22-arxiv-1606-07947-sequence-level-knowledge-distillation|Sequence-Level KD]] — +4.2 BLEU student, ~10x faster; prune to 13x fewer params at −0.4 BLEU
- [[2026-06-22-arxiv-1910-01108-distilbert|DistilBERT]] — 40% smaller, 60% faster, retains 97% of GLUE
- [[2026-06-22-arxiv-2501-12948-deepseek-r1|DeepSeek-R1]] — distilled 1.5B–70B dense models beat small-model RL
