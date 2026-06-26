---
type: source
source_type: arxiv
title: "Contagion Networks: Evaluator Bias Propagation in Multi-Agent LLM Systems"
authors: Zewen Liu (Qilu Institute of Technology)
url: http://arxiv.org/abs/2606.20493v1
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [arxiv, multi-agent-systems, evaluation, agent-security, reliability]
---

# Contagion Networks: Evaluator Bias Propagation in Multi-Agent LLM Systems

**Why it matters:** When agents grade each other (agent-as-judge, multi-agent
debate, self-evolving systems), one agent's evaluation bias can infect the
others and collapse the cognitive diversity the system was built to exploit.
This paper gives a measurable framework and a concrete, cheap mitigation — both
directly relevant to anyone designing agent eval pipelines or letting agents
critique each other in production.

## The problem they target
In multi-agent systems, agents evaluate each other's outputs to allocate
subtasks and pick responses — a closed feedback loop. A biased judgment from one
agent shapes another's subsequent outputs, which then shapes a third's. The
worry: do evaluator biases *propagate across agents*, and under what conditions
do they *cascade* into system-wide preference collapse (everyone converging to
one strategy)? Prior work (LLM-as-judge, MM-EPC) only studied single-evaluator
or pairwise dynamics — never multi-hop propagation through an agent network.

## Method
Borrows from epidemiology (SIS/SIR network models) to treat evaluator bias as an
infection spreading through an agent interaction graph.
- **Cross-Agent Contagion Matrix `Γ_N`** — an N×N matrix where `γ_{j→i}`
  measures how much agent i's strategy distribution shifts toward agent j's
  preference after rounds of evaluation (L2-norm of the weight shift). Diagonal
  is 1 (self).
- **Adaptation via TTRL** (Test-Time Reinforcement Learning) — parameter-free:
  agents sample two strategies, an evaluator picks winner/loser, and the agent
  multiplicatively bumps the winning strategy's sampling weight (α_win=0.08,
  α_lose=0.04). No model weights change — works with API-only access.
- **Propagation Regime Theorem** — behavior is governed by the spectral radius
  `ρ(Γ_N)`: **suppression** (ρ<1, bias attenuates per hop), **persistence**
  (ρ≈1), **cascade** (ρ>1, bias amplifies → network-wide collapse), proved via
  Perron-Frobenius. For chain topology, cascade requires some link `γ_{i→i+1}>1`.
- **Diversity-Induced Suppression Theorem** — k diverse evaluators reduce
  effective contagion roughly by 1/√k; k≥3 diverse evaluators suffice to break
  cascade for typical values.

**Experiment:** 3 agents, all based on the same model (DeepSeek-chat), differing
only in evaluator-bias prompt (structured / balanced / evidence-based). 5
strategies, 5 task domains (code, math, summarization, logic, creative), 4
phases (baseline → pairwise Γ_3 → chain propagation → mitigation), 840 API calls,
~50 min, <$1 total.

## Evaluation & results
- **Contagion is real but weak within one model family.** All six off-diagonal
  coefficients positive, mean γ ∈ [0.143, 0.304] — biases propagate even with a
  shared base model. All γ < 1.0, so chain topology sits in the **suppression
  regime**. (Notably, the *fully-connected* spectral radius ρ(Γ_3) = 1.402 > 1,
  so the same agents *could* cascade in a denser topology — stability is
  topology-dependent.)
- **Asymmetric:** the evidence-biased agent exerts strongest outward contagion
  (mean 0.241); structured-biased weakest (0.154).
- **Cross-model is 3–5× worse.** Same-model coefficients (0.14–0.30) are 3–5×
  weaker than the cross-model γ ≈ 0.85–1.3 from prior MM-EPC work (which *does*
  cascade). Implication — the **"contagion spectrum"**: shared architecture acts
  as implicit regularization; mixing model families *amplifies* bias spread.
- **Chain attenuates fast:** cumulative β_3 = 0.254 × 0.113 × 0.191 = 0.0055
  after 3 hops — near-complete decay.
- **Mitigation works:** growing the evaluator committee k=1→3 cuts effective
  contagion **72.4%** (γ_eff 0.264 → 0.073); strategy entropy rises toward max
  (ln 5 ≈ 1.609).

Caveats stated by the author: single model family (cross-model gap is
*inferred* from prior work, not directly measured here), only chain topology
tested for propagation, Phase 2 n=2 seeds and Phases 1/3/4 single-run — results
are exploratory.

## So what
If you let agents judge each other — eval committees, agent-as-judge QA, debate
— you're running a contagion network whether you mean to or not. Three actionable
rules from the paper: (1) **measure Γ before deploying** an evaluator config to
see if it'll suppress or cascade; (2) counterintuitively, **homogeneous
(same-model) evaluator pools suppress bias** — mixing GPT/Claude/DeepSeek as
judges can *amplify* it; (3) **use ≥3 diverse evaluators** for defense-in-depth
and **track strategy entropy** as a live health signal (falling entropy = bias
creeping in). Small, cheap framework — but the design principles are the takeaway
for any internal agent-eval pipeline.

**Connects to:** [[multi-agent-systems]] [[agent-security]] [[agentic-ai]]
**Raw:** `raw/arxiv/2606.20493v1.fulltext.md`
