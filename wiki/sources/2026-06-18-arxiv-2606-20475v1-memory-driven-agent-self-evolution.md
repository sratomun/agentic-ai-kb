---
type: source
source_type: arxiv
title: Marginal Advantage Accumulation for Memory-Driven Agent Self-Evolution
authors: Mingyu Yang, Keye Zheng, Congchao Cheng, Yujie Liu, Xingkang Lu, Fan Jiang et al. (Alibaba International Digital Commerce Group)
url: http://arxiv.org/abs/2606.20475v1
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [agent-memory, agentic-ai, self-evolution, reliability, arxiv]
---

# Marginal Advantage Accumulation for Memory-Driven Agent Self-Evolution

**Why it matters:** A cheap, training-free way to make agents learn from their own
experience and keep only the lessons that *actually* hold up — the practical path to
agents that get better in production without GPU fine-tuning. Directly relevant to any
ADP agent expected to improve over time from its own traces.

## The problem they target
Agents "self-evolve" by distilling their execution traces into a reusable memory bank
(skills, insights, workflow templates, few-shot cases) that gets injected at inference.
In real deployments this distillation runs *offline in batches* — the agent runs a batch
of tasks, then memory is optimized from those traces without re-running the agent
(re-rollout costs an order of magnitude more than distillation). That forces two hard
limits:
- **No forward verification** — you can only judge a memory edit with a cheap, noisy
  proxy (an LLM judge), not by actually re-running the task.
- **One batch at a time** — trace collections exceed any context window, so edits are
  decided from a single batch's local view.
The result is "locally effective, globally unstable" memory: an op that helps one batch
(e.g., "always add axis labels to plotting code") breaks another (heatmaps, 3D plots).
Existing methods (single-shot like ExpeL/Voyager, reactive like A-MEM/MemGPT) can't tell
a *stably effective* operation from an *accidental hit*, because they keep no cross-batch,
per-operation evidence and can't use later batches' reverse signals to undo earlier bad
edits.

## Method
MAA (Marginal Advantage Accumulation) is a **post-processing layer** over a frozen base
LLM and fixed agent scaffold — no weight updates; only the context-injected memory `M` is
optimized. It formalizes two requirements and builds a mechanism for each:
- **Alignability (semantic identity merging)** — memory is an addressable set of items
  with stable, never-reused ids. Each edit ("op") is identified by `(type, anchor,
  content embedding)`; new candidates merge into an existing accumulation unit when type
  and anchor match and embedding cosine similarity ≥ τ (default 0.85, via Qwen3-Embedding-4B).
  This stops the same idea, worded differently across batches, from fragmenting into
  separate units.
- **Comparability (marginal advantage via differencing)** — an LLM "Score channel"
  estimates expected utility `u(M,B) ∈ [0,100]` for the current batch, evaluating
  baseline and all candidate states side-by-side in one shuffled prompt. Per candidate it
  takes a difference `δ_i = u(M_i,B) − u(M,B)`, which cancels batch-difficulty drift. A
  separate "Propose channel" generates candidates without scores, to avoid confirmation
  bias. MAA relies only on the *sign* of δ being right more than half the time
  (directional alignment), not on accurate magnitudes.
- **Cross-batch accumulation (per-op EMA)** — each op's δ across batches is aggregated
  with a bias-corrected exponential moving average. Consistent-sign evidence amplifies;
  alternating signs cancel toward zero. This lets MAA distinguish stably effective
  (EMA high positive), spurious (EMA decays to zero), and scene-specific (EMA oscillates)
  ops. Top-k sparse truncation (decaying ratio, explore early / conserve late) applies
  only positive-EMA ops; best-checkpoint rollback on a validation set guards against
  regressions.

Crucially, if proxy scoring fails entirely (no directional signal), EMA introduces no
systematic bias and MAA degrades to no worse than a reactive-update baseline. It's
orthogonal to RL — the two can be combined in production.

## Evaluation & results
- **Benchmarks:** four covering different complexity — ScienceAgentBench (scientific
  agent, code pass rate), ALFWorld (embodied, success rate), SpreadsheetBench (accuracy),
  HotpotQA (multi-hop QA, exact match). 500 training trajectories each; 5 seeds.
- **Models:** Qwen3.7-Max, Qwen3.6-Flash, DeepSeek-V4-Flash, GPT-5.4 (strong/weak ×
  same-family/cross-family). Score channel always Qwen3.7-Max.
- **Headline:** MAA achieves the **best result in 14 of 16 settings** (4 benchmarks × 4
  models), beating frozen, single-shot (ExpeL-style), reactive update, offline Trace2Skill,
  and matching or beating the *online* SkillOpt baseline in most settings.
- **Example gains (Qwen3.7-Max):** SpreadsheetBench 41.8 (frozen) → 58.5 (MAA);
  ScienceAgentBench 22.1 → 30.7; ALFWorld 81.0 → 89.4; HotpotQA 71.1 → 77.2.
- **Efficiency:** ~**75% less optimization-phase token consumption** (~1/4 the tokens,
  ~1/5 the training time of online methods); optimization time cut from 12–14 hours to
  ~2.5 hours. Ablations confirm both the differencing layer and the EMA accumulation layer
  contribute to the gains.

## So what
This is the offline, no-training answer to "how do agents learn from experience safely."
The signal isn't just that experience-distillation works — it's that the *hard part* is
filtering durable lessons from lucky one-offs, and you can do it with a deterministic
evidence-accumulation layer (identity merging + signed-difference EMA) bolted on top of any
frozen model. For ADP that means agents can self-improve from their own traces without GPU
fine-tuning, with a built-in floor (never worse than no-accumulation) and a 75% cost cut
vs. online alternatives. The control-layer pattern — accumulate evidence, keep only what
repeatedly verifies — generalizes well beyond memory.

**Connects to:** [[agent-memory]] [[agentic-ai]]
**Raw:** `raw/arxiv/2606.20475v1.fulltext.md`
