---
type: source
source_type: blog
title: "Life lessons from reinforcement learning"
author: Jason Wei
outlet: jasonwei.net
url: https://www.jasonwei.net/blog/life-lessons-from-reinforcement-learning
resource: https://www.jasonwei.net/blog/life-lessons-from-reinforcement-learning
date: 2025-07-15
stake: Frontier-lab reasoning/RL researcher (OpenAI → Meta Superintelligence Labs) — RL practitioner reflecting on his own craft
ingested: 2026-06-22
tags: [perspective, agentic-rl]
---

# Life lessons from reinforcement learning

**Blog** · Jason Wei (jasonwei.net) · 2025-07-15 · [link](https://www.jasonwei.net/blog/life-lessons-from-reinforcement-learning)

**The take (attributed):** Wei argues the core RL principle of staying **"on-policy"** — learning from your own trajectories rather than imitating others — is both why RL beats supervised finetuning on reasoning *and* a personal operating principle: imitate to bootstrap, then play to your own strengths to surpass the teacher.

**Stake:** OpenAI/Meta RL researcher; this is a craft-and-mindset essay, low direct commercial stake, but it doubles as a clear lay explanation of *why* on-policy RL is preferred — useful as primary-source intuition.

## Argument
- In RL you want to be **on-policy**: imitation learning bootstraps to nonzero pass rate, but once trajectories are reasonable you avoid imitation, "because the best way to leverage the model's own strengths (which are different from humans) is to only learn from its own trajectories." Canonical instantiation: RL beats SFT-on-human-chains-of-thought for math word problems.
- Life analogy: school is imitation learning (fine). But copying others' success caps you — "I would never surpass the full ability of someone else because they were playing to their strengths which I didn't have."
- "Beating the teacher requires walking your own path and taking risks and rewards from the environment." Wei leans into his own edges (reading lots of data; running ablations) — e.g. spending a month ablating decisions he'd yolo'ed on **deep research** to learn what kind of RL actually works.

## Why it matters / where it cuts
A primary-source, plain-English statement of the **on-policy > imitation** intuition that underwrites the post-training shift from SFT to RL ([[agentic-rl]]). For the exec it's a useful frame for why "copy the frontier lab's recipe" has limits — the leverage is in your own distribution, not someone else's trajectory. Lighter than his verifier's-rule piece but reinforces the same RL-first worldview from [[jason-wei]].

## Graph
- **Author:** [[jason-wei]]
- **Concepts:** [[agentic-rl]] · [[reasoning-models]] · [[deep-research-agents]]
- **Entities:** [[rlvr]]
- **Raw:** `raw/blogs/2025-07-15-jason-wei-life-lessons-from-rl.md`
