---
type: source
source_type: blog
title: "What comes next with reinforcement learning"
author: Nathan Lambert
outlet: Interconnects
url: https://www.interconnects.ai/p/what-comes-next-with-reinforcement
resource: https://www.interconnects.ai/p/what-comes-next-with-reinforcement
date: 2025-06-09
stake: Researcher (AI2 at time of writing); open-models advocate; low commercial stake
ingested: 2026-06-22
tags: [perspective, agentic-rl, reasoning-models]
---

# What comes next with reinforcement learning

**Blog** · Nathan Lambert (Interconnects) · 2025-06-09 · [link](https://www.interconnects.ai/p/what-comes-next-with-reinforcement)

**The take (attributed):** Lambert argues **scaling [[rlvr|RLVR]] makes models more *robust at individual tasks* — it does not, by itself, unlock complex new long-horizon domains**, which are still assembled by scaffolding, not learned end-to-end.

**Stake:** Researcher who coined RLVR (Tülu 3); open-models advocate — low commercial stake.

## Argument
- Three avenues now that RL works: (1) keep scaling RLVR for reasoning; (2) push RL to **sparser domains** (hours/days feedback — science, robotics); (3) **continual learning**.
- Key nuance: "scaling RL is the shortest path" means scaling *current* techniques, **not** magically training end-to-end on whole codebases or real experiments — "major discoveries and infrastructure improvements are needed."
- On **Deep Research / Claude Code**: trained with o1-style RL to get robust at *individual* tasks; "the final long-horizon behavior is put together with prompting and letting the model run longer, **not** sparse credit assignment." → long-horizon = scaffold, not learned.
- Leans **pessimist on sparse scaled RL** (resembles robotics, where end-to-end RL isn't SOTA). Longer RL runs → more frequent releases that *feel* like continual learning.
- Opinion: true continual-learning-from-*you* is "a destiny to dystopia" — concentrates a powerful optimizer on intimate context; prefers personalization / on-device / open "n-of-1" models.

## Why it matters / where it cuts
A rare *nuanced* expert voice between the bulls and the skeptics: RL is real and scaling, but long-horizon agency is still **scaffolded**, not learned — which sharpens the "base model vs scaffold" question in [[reasoning-models]] and informs the AGI debate.

## Graph
- **Author:** [[nathan-lambert]]
- **Concepts:** [[agentic-rl]] · [[reasoning-models]] · [[deep-research-agents]] · [[self-evolving-agents]]
- **Entities:** [[rlvr]] · [[grpo]]
- **Debate:** [[debate-llms-path-to-agi]]
- **Raw:** `raw/blogs/2025-06-09-nathan-lambert-what-comes-next-rl.md`
