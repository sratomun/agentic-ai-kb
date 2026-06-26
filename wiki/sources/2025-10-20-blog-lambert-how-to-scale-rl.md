---
type: source
source_type: blog
title: "How to scale RL"
author: Nathan Lambert
outlet: Interconnects
url: https://www.interconnects.ai/p/the-new-rl-scaling-laws
resource: https://www.interconnects.ai/p/the-new-rl-scaling-laws
date: 2025-10-20
stake: Researcher / open-models advocate (Ai2 at time of writing); low commercial stake
ingested: 2026-06-22
tags: [perspective, agentic-rl, reasoning-models]
---

# How to scale RL

**Blog** · Nathan Lambert (Interconnects) · 2025-10-20 · [link](https://www.interconnects.ai/p/the-new-rl-scaling-laws)

**The take (attributed):** Lambert argues the first real **RL scaling laws** (Meta's "ScaleRL" paper) are a major step — but warns they're "**more art than science**": a tool for *ablating which algorithm to run longer*, not a deep law like pretraining scaling.

**Stake:** Open-models advocate whose AI2 team races to reproduce frontier RL in public — talking up open-RL infra (Open Instruct).

## Argument
- Reviews "The Art of Scaling Reinforcement Learning Compute for LLMs" (Khatri & Madaan et al. 2025, "ScaleRL", Meta + collaborators) — "the first definitive paper on scaling RL." His AI2 reasoning team named its Slack channel "scaling-rl" all year in anticipation.
- Method: fit a sigmoid (A = asymptotic accuracy, B = slope, C = compute) from early RL training points to predict a long run's endpoint; in the paper, 1/4 of compute predicts the remaining 3/4.
- KEY CAVEAT (his emphasis): these are NOT pretraining scaling laws. RL-train accuracy is "a far more bounded measure than next token prediction"; the laws are for **ablating design choices**, not "something fundamental." Scaling RL is "more like an art."
- Recurring meta-claim across his catalog: "**Most of the key ideas are out there, but open labs tend to not have the resources to put them all together in the right configuration**." The gap is organizational, not secret algorithms.
- Algorithms blessed: truncated importance sampling (TIS), GSPO, CISPO (MiniMax M1). The actor↔learner importance-sampling correction (e.g. vLLM-generating vs Transformers-updating) is "essential to getting modern RL infrastructure right." Systems: PipelineRL's in-flight weight updates + continuous batching → 4X+ throughput; AI2's [[grpo|Open Instruct]] has both.
- On the "[[grpo|GRPO]] is far behind frontier labs" debate: *vanilla* GRPO is far behind; the trick-set that works on your model/data is a well-kept secret, and ScaleRL helps bridge it. Open questions: data regime (uses Polaris 53K math) and base-model choice (bigger base RL's better — a 17Bx16 MoE beat an 8B dense using 1/6 the RL compute). Footnote: "very long horizon" RL for scientific discovery "is still much further off."

## Why it matters / where it cuts
The infrastructure-level companion to his reasoning posts: it explains the *open-vs-closed* dynamic the exec tracks — frontier labs win by assembling known tricks at scale, and the public catches up unevenly. Reinforces the through-line from [[2025-06-09-blog-lambert-what-comes-next-rl|"What comes next with RL"]] that scaled RL is real but long-horizon agency remains beyond current method.

## Graph
- **Author:** [[nathan-lambert]]
- **Concepts:** [[agentic-rl]] · [[reasoning-models]]
- **Entities:** [[grpo]] · [[ppo]] · [[rlvr]]
- **Raw:** `raw/blogs/2025-10-20-nathan-lambert-how-to-scale-rl.md`
