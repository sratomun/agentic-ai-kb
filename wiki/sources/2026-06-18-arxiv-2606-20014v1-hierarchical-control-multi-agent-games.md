---
type: source
source_type: arxiv
title: "Hierarchical Control in Multi-Agent Games: LLM-based Planning and RL Execution"
authors: Jannik Hösch, Alessandro Sestini, Florian Fuchs, Amir Baghi, Joakim Bergdahl, Konrad Tollmar, Jean-Philippe Barrette-LaPierre, Linus Gisslén (EA / KTH)
url: http://arxiv.org/abs/2606.20014v1
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [arxiv, multi-agent-systems, agentic-ai, reinforcement-learning, planning-execution]
---

# Hierarchical Control in Multi-Agent Games: LLM-based Planning and RL Execution

**Why it matters:** A clean demonstration of the **planning/execution split** —
a pretrained LLM does slow strategic reasoning and picks among pretrained
specialist policies, which handle fast reactive control. No fine-tuning, no
hand-coded rules. The pattern (LLM-as-meta-controller over a library of skills)
generalizes well beyond games to any multi-agent system with reusable tools/skills.

## The problem they target
RL struggles in multi-agent settings — sparse rewards, huge state-action spaces,
non-stationarity from other learning agents, hard credit assignment.
Hierarchical RL helps via reusable skills, but automatic skill discovery and
learning the high-level skill-selecting policy are themselves unstable and
sample-inefficient. LLMs reason and plan well but are too slow and ungrounded
for low-level reactive control. The question: can a pretrained LLM orchestrate
pretrained RL skills to get competitive coordination *and* believable behavior
without manual rule engineering?

## Method
A two-layer hierarchy, both layers pretrained (no end-to-end training of the
hierarchy):
- **Strategic layer (LLM):** a centralized meta-controller (Gemma 3 27B via
  Ollama, temperature 0.1) observes global game state — discretized into
  categorical labels like health HIGH/MEDIUM/LOW for semantic reasoning — and at
  ~2 Hz (0.5s intervals) assigns each agent one of m=4 skills.
- **Execution layer (RL):** each agent runs its assigned skill policy at 12.5 Hz,
  mapping local observations (20-dim vector) to hybrid actions. Four skills
  trained independently via PPO for 10M steps each in Unity ML-Agents, with
  shaped rewards: **Navigate** (toward goal), **Combat** (engage enemies),
  **Secure** (defend zone), **Retreat** (flee to health when low).
- **Environment:** bespoke 2v2 King of the Hill in Unity 6 — two teams race to
  hold a goal zone for 8s; elimination costs 50% goal progress; 60s draw cap.
- **Baselines:** hand-crafted **Behavior Tree** (priority rules, shared
  blackboard for role exclusivity) and **Flat RL** (single PPO policy, no skill
  decomposition, trained 15M self-play + 15M vs heuristic team).

Key design idea: asymmetry — LLM gets global state at low frequency for
coordination; RL gets local state at high frequency for reactivity.

## Evaluation & results
Two evaluations: 3,000 episodes of pairwise matchups (1,000 each) plus a user
study (n=15, within-subjects, 5-point Likert).
- **Win rates:** LLM+RL is **statistically equivalent to the hand-crafted BT**
  (46.4% vs 51.5%, p=0.103) and both **crush Flat RL** (p<0.001). vs Flat RL:
  BT wins 72.2%, LLM+RL 67.0%. So skill decomposition is what matters — Flat RL
  had the *highest* K/D ratio (2.074) but the *lowest* win rate, underlining
  that coordination, not individual combat, wins.
- **Behavioral profile:** Flat RL combat-heavy (87 shots, 56% acc, rarely heals);
  BT cautious-precise (26 shots, 96% acc, dies most); LLM+RL between (81 shots,
  32% acc) and collected the **most health pickups** (0.57/episode) — it learned
  to heal.
- **Human-likeness (user study):** **60% of participants** rated LLM+RL most
  human-like (n=9) vs Flat RL 33.3% and BT 6.7% (chi-square p=0.027, Cramér's
  V=0.69), citing behavioral adaptability and tactical variability. LLM+RL also
  topped 4 of 5 subjective dimensions. Against human teams, LLM+RL won most
  (25.6% AI wins vs BT 13.3%, Flat RL 1.1%).
- **Why:** LLM+RL allocates more time to Combat (36.2% vs BT 24.0%) and has
  higher skill-transition entropy (H=3.19 vs 2.47 bits) — varied, context-driven
  switching rather than stereotyped loops.

Limitations the authors flag: one environment, one LLM (Gemma 3 27B), small
user study (n=15), single hand-tuned prompt with no ablation; LLM+RL didn't
*beat* the BT (premature skill switching, RL policies hitting out-of-distribution
states after transitions).

## So what
The transferable lesson isn't the game — it's the architecture. A frozen
general-purpose LLM, reasoning over a *discretized, semantic* view of state at a
slow cadence, can effectively orchestrate a library of pretrained specialist
policies/skills at high cadence, matching hand-engineered logic *with zero rule
authoring*. That's the same shape as an enterprise agent fleet: an LLM planner
selecting among specialist agents/tools. The believability result also hints
that LLM-driven orchestration produces more adaptive, less brittle behavior than
rigid decision trees — relevant wherever agent behavior faces a human and
predictability reads as "robotic."

**Connects to:** [[multi-agent-systems]] [[agentic-ai]]
**Raw:** `raw/arxiv/2606.20014v1.fulltext.md`

## Relationships
- model: [[google]] (Gemma 3 27B)
