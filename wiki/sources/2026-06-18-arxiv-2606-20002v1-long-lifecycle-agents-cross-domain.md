---
type: source
source_type: arxiv
title: "Connect the Dots: Training LLMs for Long-Lifecycle Agents with Cross-Domain Generalization Via Reinforcement Learning"
authors: Yanxi Chen, Weijie Shi, Yuexiang Xie, Boyi Hu, Yaliang Li, Bolin Ding et al. (Alibaba Group)
url: http://arxiv.org/abs/2606.20002v1
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [agent-memory, agentic-ai, reinforcement-learning, generalization, arxiv]
---

# Connect the Dots: Training LLMs for Long-Lifecycle Agents with Cross-Domain Generalization Via Reinforcement Learning

**Why it matters:** Today's agents lean on hand-crafted scaffolds to stay coherent over
long deployments; this trains the *meta-skill* of learning-from-experience directly into
the model via RL, so the agent itself decides what to remember and improves over a long
run. The early evidence that "continual learning at test time" can be a trained capability,
not just a prompting trick.

## The problem they target
Long-lifecycle agents must solve a sequence of related tasks in one environment while
exploring it, learning from their own experience, and self-updating their context so later
tasks go better. The authors call this meta-capability **CoD ("Connect the Dots")**.
Frontier LLMs fall short: in underspecified environments they get lost, act on confident-
but-wrong priors, and lose coherence over many rounds — so practitioners patch around it
with elaborate human-designed scaffolds. The gap, they argue, is the **absence of dedicated
post-training** for the meta-capability itself. Standard task-by-task RL trains an LLM to
solve each task from scratch, which is misaligned with long-lifecycle deployment.

## Method
A general framework with a matching training and deployment loop:
- **CoD-Deploy** — abstraction of long-lifecycle deployment in an environment `M`,
  interleaving *solve-task* episodes and *update-context* episodes. The agent solves a
  task while exploring, then condenses experience into updated context (gradient-free
  online learning by trial and error).
- **CoD-Train** — RL post-training whose rollout pattern exactly mirrors CoD-Deploy,
  spanning diverse environments for generalization. It sits one level up in the RL
  hierarchy: trajectories evolve from tokens (single-turn) → turns (long-horizon task) →
  **a sequence of tasks** (long-lifecycle deployment).
- **Credit assignment** — the key algorithmic challenge across long solve/update episode
  sequences. They use a GRPO-style algorithm (critic-free) with **fine-grained credit
  assignment**: each episode's return is the mean reward of the current plus future
  solve-task episodes; episodes at the same sequence position form a group, and their
  averaged return is the advantage baseline. A heuristic re-weighting balances positive/
  negative gradients to fix training instability. Solve-task episodes get outcome rewards;
  update-context episodes get only a small format reward. Built on the Trinity-RFT
  framework (code released).
- **Context** is kept minimal in this proof of concept — a single text "hint" appended to
  the system prompt. Persistent memory banks / Agent Skills files are flagged as future work.
- **Dedicated environments** that *require* cross-task knowledge transfer: **FrozenLake-
  Obscure** (FrozenLake where the A/B/C/D→direction mapping is randomly permuted and hidden,
  imposing an information-theoretic ceiling on solving any single task cold), **Alchemy-
  Random** (discover element recipes), and **TerminalSimulator** (OS-flavored file tasks).

## Evaluation & results
- **Base model:** Qwen3-8B-Instruct. Two training settings: (A) FrozenLake-Obscure alone,
  (B) FrozenLake-Obscure + Alchemy-Random mixture, both with length-4 task sequences.
- **Headline (FrozenLake-Obscure, setting A):** mean reward at the *first* task (no context)
  rises only **0.18 → 0.45** (bounded by information-theoretic limits), but at the *fourth*
  task in a sequence — conditioned on the agent's self-updated context — it jumps **0.28 →
  0.76**. The agent learned to connect the dots, not just solve harder.
- **In-domain OOD generalization:** holds on harder instances (larger maps / more elements)
  and longer length-8 sequences.
- **Cross-domain generalization:** gains transfer to Alchemy-Random and TerminalSimulator
  unseen at training, and to **Ralph-loop** settings (repeated attempts at the same task) —
  evidence the meta-capability generalizes beyond its training domains.
- **Algorithm matters:** fine-grained credit assignment enabled effective training where a
  coarse Orbit-style sum-of-rewards approach was not feasible on FrozenLake-Obscure.
  Setting B (mixed domains) showed less stable Alchemy-Random reward curves.

## So what
This reframes "agent memory" as a *trainable meta-skill* rather than a bolt-on store. The
striking number is the gap between solving cold (0.45) and solving with self-built context
(0.76) — the value is almost entirely in the agent learning *how to remember and reuse*.
For ADP, the long-game implication is agents that adapt to a specific client environment or
user over a long deployment and get measurably better, with less hand-built scaffolding. It's
proof-of-concept (8B model, toy environments, single-text-hint context), so treat it as a
research signal of where training is heading, not a production recipe — but the direction
(RL for continual learning, cross-domain transfer) is the one to watch.

**Connects to:** [[agent-memory]] [[agentic-ai]]
**Raw:** `raw/arxiv/2606.20002v1.fulltext.md`

## Relationships
- methods: [[grpo]]
