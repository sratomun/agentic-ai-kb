---
type: source
source_type: blog
title: "A taxonomy for next-generation reasoning models"
author: Nathan Lambert
outlet: Interconnects
url: https://www.interconnects.ai/p/next-gen-reasoners
resource: https://www.interconnects.ai/p/next-gen-reasoners
date: 2025-06-04
stake: Researcher who coined RLVR (Tülu 3, Ai2 at time of writing); open-models advocate; low commercial stake
ingested: 2026-06-22
tags: [perspective, reasoning-models, agentic-rl, agentic-ai]
---

# A taxonomy for next-generation reasoning models

**Blog** · Nathan Lambert (Interconnects) · 2025-06-04 · [link](https://www.interconnects.ai/p/next-gen-reasoners)

**The take (attributed):** Lambert argues the leap from reasoning models to *agentic* models needs **four capabilities solved in order — skills → calibration → strategy → abstraction** — and that the field over-invests in skills and under-invests in **planning**.

**Stake:** Coined [[rlvr|RLVR]]; open-models advocate — a research-framing piece, low commercial stake.

## Argument
- The taxonomy: (1) **Skills** — solve self-contained problems; (2) **Calibration** — judge difficulty, don't overthink; (3) **Strategy** — choose the right high-level plan; (4) **Abstraction** — break a strategy into solvable chunks. First two are native single-pass abilities; strategy + abstraction ("planning") are "skills that are needed to build effective agents" and "additive... but not present by default."
- "The first generation of reasoning models brought us inference-time scaling... The second generation are going to bring us new types of agentic language modeling applications." Best results need *training* models to optimize for planning, not just prompting.
- Grounds in METR's task-horizon chart: skills (via scaling [[rlvr|RLVR]]) unlocked the bump through Claude Sonnet 3.7; "planning well will be the trait of models that make the leap from 1 to 4+ hours in 2026."
- On parallel / inference-time compute (o1-pro, Claude 4's parallel sampling + internal scoring, Gemini Deep Think): "doing something very different than scaling the underlying RL — an added form of robustness." Best framed as "a tool that the agent can call."
- Per Lambert, [[openai-o3|o3]] leads this paradigm (broad skills, some planning via Deep Research) but "I attribute very little of that behavior to planning, but rather just the skill... of knowing to keep searching" — it nearly solves *search* yet fails at *synthesis* across a broad category. [[claude|Claude]] Code leads on software-task planning, possibly because it's "taught to edit and revisit the plan many times while it is running."
- Path: planning likely needs manual data annotation to bootstrap (like the [[mcts|Q*]]-era curation effort), cold-start SFT, *then* the final goal of "training agents end-to-end with RL on long-horizon, sparse tasks." "The real race is towards building systems that people use... rather than... skills that aren't showing clear value."

## Why it matters / where it cuts
The cleanest articulation in his catalog of *what's missing* between reasoning and agency — a useful lens for [[reasoning-models]] and [[deep-research-agents]] (skills are solved; planning/synthesis is the frontier). Directly sets up [[2025-06-09-blog-lambert-what-comes-next-rl|"What comes next with RL"]] (planning is still scaffolded, not learned end-to-end) and the human-orchestration argument in [[2026-01-21-blog-lambert-get-good-at-agents|Get Good at Agents]].

## Graph
- **Author:** [[nathan-lambert]]
- **Concepts:** [[reasoning-models]] · [[agentic-rl]] · [[agentic-ai]] · [[deep-research-agents]]
- **Entities:** [[rlvr]] · [[openai-o3]] · [[claude]] · [[mcts]]
- **Raw:** `raw/blogs/2025-06-04-nathan-lambert-taxonomy-next-gen-reasoners.md`
