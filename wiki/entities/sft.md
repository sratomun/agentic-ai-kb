---
type: entity
entity_type: method
tags: [agents, method, post-training]
created: 2026-06-22
updated: 2026-06-22
---

# SFT

*Supervised fine-tuning — training a base model on curated input→output demonstrations; the first and cheapest post-training step.*

## What it is
Fine-tuning a pre-trained model on high-quality demonstration pairs (instructions and ideal responses, or distilled reasoning traces) so it follows instructions and adopts a format. It's stage one of the [[post-training]] recipe, before preference optimization and RL. Data quality dominates quantity — LIMA showed strong alignment from ~1,000 well-chosen examples.

## Why it matters
SFT is where most of the *behavior* you see in a chat model is installed, and where distillation enters the pipeline (SFT a small model on a big model's outputs — see [[distillation]], [[synthetic-data]]). So what: it's the highest-leverage, lowest-cost lever for teams that can't run full RL — the 80/20 of post-training.

## Relationships
- stage of [[post-training]]; precedes [[rlhf]], [[dpo]], [[rlvr]]
- mechanism for [[distillation]]; consumes [[synthetic-data]]
- explained by [[sebastian-raschka]]

## Key papers (full-text ingested)
- [[2022-03-04-arxiv-2203-02155-instructgpt|InstructGPT]] — SFT is stage 1 of the alignment recipe
- [[2023-05-18-arxiv-2305-11206-lima-less-is-more-for-alignment|LIMA]] — a 65B SFT'd on just 1,000 curated examples rivals RLHF'd models
- [[2024-11-22-arxiv-2411-15124-tulu-3|Tülu 3]] — open SFT data + recipe
