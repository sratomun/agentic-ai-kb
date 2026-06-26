---
type: source
source_type: arxiv
title: "LedgerAgent: Structured State for Policy-Adherent Tool-Calling Agents"
authors: Md Nayem Uddin, Amir Saeidi, Eduardo Blanco, Chitta Baral (ASU / U. Arizona)
url: https://arxiv.org/abs/2606.20529
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [agent-security, tool-use, governance-gap, reliability, arxiv]
---

# LedgerAgent: Structured State for Policy-Adherent Tool-Calling Agents

**Why it matters:** A training-free pattern for stopping agents from taking
disallowed actions — exactly the reliability/governance problem enterprises hit when
agents touch real systems (refunds, orders, accounts). Directly relevant to any
HR/payroll agent (ADP) that must obey policy before it writes.

## The problem they target
Standard tool-calling agents keep task state *implicit* in an ever-growing prompt
(tool outputs, prior actions, policy text all interleaved). Two failure modes follow:
1. **State grounding failures** — the agent retrieved the right record earlier but
   later acts on stale/missing/misreconstructed state.
2. **Policy-boundary failures** — a syntactically valid tool call still violates a
   domain policy whose applicability depends on current state.

## Method (inference-time, model weights unchanged)
Two deterministic components added to the agent loop:
- **Schema-anchored ledger** — a typed dictionary mapping canonical paths
  (`user`, `orders.*`, `products.*`, `reservations.*`) to tool-returned values.
  Built with no extra LLM calls; updated *only* from successful read-tool returns;
  re-injected into the prompt each turn so the model looks state up instead of
  searching transcript history. "Observe-not-assume": after a write, the agent must
  re-read to refresh the ledger.
- **Policy gate** — runs immediately before any *environment-changing* call,
  evaluating it against executable predicates over the ledger. Three verdicts:
  **allow** / **revise** (drop the call, return the violated predicate) / **block**.
  Read-only calls aren't gated. It's a verifier only — it doesn't pick tools or
  repair arguments.

Framed as a *system-level* mechanism, complementary to fine-tuning, RL, or
multi-agent scaffolding (which all keep state prompt-implicit).

## Evaluation & results
- Benchmarks: four customer-service domains from **τ²-bench** and **τ-Trait**, across
  a mixed panel of open- and closed-weight models.
- Metric: **pass^k** (multi-trial consistency). LedgerAgent improves average pass^k
  over standard prompt-based tool calling on the majority of domain–model pairs, with
  the **largest gains at higher k** (where prompt-only agents are least consistent)
  and on **environment-changing tasks**. Ablations attribute the gain to both the
  typed ledger and the policy gate.

## So what
The frontier of "safe agents" isn't only better models — it's external, deterministic
guardrails (typed state + pre-action policy gates). Cheap to bolt on, model-agnostic,
and the kind of control layer enterprises will demand before letting agents write.

**Connects to:** [[agent-security]] [[tool-use]] [[governance-gap]]
**Raw:** `raw/arxiv/2606.20529v1.fulltext.md` (full text, ~59k chars)

## Relationships
- benchmarks: [[tau2-bench]], [[tau-trait]]
