---
type: source
source_type: blog
title: "DeepSeek R1's recipe to replicate o1 and the future of reasoning LMs"
author: Nathan Lambert
outlet: Interconnects
url: https://www.interconnects.ai/p/deepseek-r1-recipe-for-o1
resource: https://www.interconnects.ai/p/deepseek-r1-recipe-for-o1
date: 2025-01-21
stake: Researcher who coined RLVR (Tülu 3, Ai2 at time of writing); open-models advocate; low commercial stake
ingested: 2026-06-22
tags: [perspective, reasoning-models, agentic-rl]
---

# DeepSeek R1's recipe to replicate o1 and the future of reasoning LMs

**Blog** · Nathan Lambert (Interconnects) · 2025-01-21 · [link](https://www.interconnects.ai/p/deepseek-r1-recipe-for-o1)

**The take (attributed):** Lambert argues [[deepseek|DeepSeek]] R1 is the true *open* replication of [[openai-o1|o1]] — proof that **reasoning comes from scaled RL, not search**, and that "new technical recipes normally aren't moats."

**Stake:** Coined [[rlvr|RLVR]] in Tülu 3; open-models advocate — clearly cheering an MIT-licensed open reasoning model.

## Argument
- Calls R1 "a major transition point" — the missing seminal reasoning paper. MIT-licensed flagship + R1-Zero (RL-only from V3 base, no SFT) + distilled small models + a technical report. "Reasoning research and progress is now locked in."
- The 4-stage R1 recipe Lambert reconstructs: (1) "cold-start" SFT on a few thousand filtered R1-Zero traces (readability + final perf); (2) large-scale RL on reasoning problems "until convergence"; (3) rejection sampling (800K completions, 600K reasoning / 200K general) to reintroduce general ability; (4) final RL mixing verifiable rewards + RLHF preference reward models.
- Three reward components in the reasoning RL: accuracy (verifiable — "drives the majority of the learning"), format ([[chain-of-thought|<think>]]/<answer> tags), and language-consistency (slight perf hit, better human prefs — "evaluation scores are not all that matters"). Uses [[grpo|GRPO]] (a [[ppo|PPO]] update with Monte Carlo advantage, no value model), "the mature implementation in their infrastructure."
- Headline technical claim: R1-Zero shows **training-time RL scaling** (not just inference-time) correlated with eval performance, with response length growing during training — "the real foundational result." Curves look "still going up."
- "The winds of o1 replication have been blowing strongly away from any sort of explicit search... It really was, and is, a language model with the new reasoning behaviors coming from a lot of RL training." → signals the demise of process reward models and [[mcts|MCTS]] for this paradigm.
- Pricing collapse: [[openai-o1|o1]] at $15/$60 per M tokens vs R1 at $0.55/$2.19 (~10x); predicts a reasoning price war like the 2023 Mixtral race to the bottom.
- Biggest open question (from the paper's distillation results): distilling strong models into small ones beats small-model RL; pushing the intelligence frontier "may still require more powerful base models and larger-scale RL." His 2025 question: "How *small* will... research drive advanced reasoning capabilities?"

## Why it matters / where it cuts
The foundational, dated marker for the [[rlvr|RLVR]]/reasoning era in the exec's radar — explains *why* every lab pivoted to RL-trained reasoners and seeds Lambert's later, more cautious arc on [[2025-06-09-blog-lambert-what-comes-next-rl|what RL does and doesn't unlock]]. Grounds the "RL, not search" position that runs through his whole catalog.

## Graph
- **Author:** [[nathan-lambert]]
- **Concepts:** [[reasoning-models]] · [[agentic-rl]]
- **Entities:** [[deepseek]] · [[openai-o1]] · [[rlvr]] · [[grpo]] · [[ppo]] · [[mcts]] · [[chain-of-thought]]
- **Raw:** `raw/blogs/2025-01-21-nathan-lambert-deepseek-r1-recipe.md`
