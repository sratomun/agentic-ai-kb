---
type: comparison
tags: [agents, evaluation, benchmarks, reliability, state-of-field]
created: 2026-06-22
updated: 2026-06-22
source_count: 8
---

# Agent evals — state of the field (2026 H1)

A synthesized state-of-the-field analysis for AI engineering teams: where agent evaluation is, what advanced, what's still broken, and how to build an eval harness around it. Full write-up lives at `/AI Tech Radar/agent-evals-state-2026.md`.

Full write-ups: `/AI Tech Radar/agent-evals-state-2026.md` (narrative brief) and `/AI Tech Radar/agent-evals-technical-companion-2026.md` (deep dive: 12-tier apparatus + platform metric catalog with default/opt-in split).

## Taxonomy (the spine)
Two axes organize everything:
- **Axis A — layer under test** (what you hold fixed vs vary): **Model** (vary model, fix scaffold), **Agent system** (fix model, vary scaffold — single/multi-agent), **Eval infrastructure** (the judges/guardrails, themselves under test).
- **Axis B — quality dimension** (at every layer): capability/task-success, output quality (faithfulness vs fidelity), consistency (`pass^k`), safety/security, cost/efficiency, selection validity.
- **Functional tasks** specialize *output quality* at the agent-system layer; **benchmarks** are instruments measuring (layer × dimension × task) cells.
- Terminology: the layer-2 scaffold ("reasoning harness") is distinct from the **eval rig** (benchmarks + judges + telemetry). Don't use "harness" unqualified.

## The thesis
2026 evidence converges on one point: **aggregate benchmark scores don't predict deployed agent behavior.** Rankings reshuffle out-of-distribution, the realistic-enterprise ceiling is ~37%, more orchestration can hurt, and LLM-as-judge is a stochastic, model-dependent component — not a measurement. The field's center of gravity moved from *capability* to *dependability* ([[agent-reliability]] is the largest H1 theme after reasoning).

## What advanced
- **Predictive validity** as a selection metric over leaderboards → [[2026-06-18-arxiv-2606-19704v1-predictive-validity-agent-evaluation]]
- **Hard, stateful, side-effect-aware** enterprise envs → [[2026-03-13-arxiv-2603-13594v1-enterpriseops-gym-stateful-agentic-planning]]
- **Cross-paradigm grounding** (RL/LLM/VLM/human on one interface) → [[2026-05-07-arxiv-2605-06869v2-agentick-unified-sequential-decision-benchmark]]
- **Negative results published** (orchestration overhead hurts) → [[2026-05-13-arxiv-2605-14102v2-chromaflow-negative-ablation-orchestration]]
- **Consistency + cost as first-class metrics** (`pass^k`; tool-abuse pricing) → [[2026-06-01-arxiv-2606-02132v2-eapo-learning-when-not-to-act]]
- **Fine-grained + adversarial safety eval** → [[2026-06-02-arxiv-2606-04051v1-rubas-rubric-based-rl-agent-safety]], [[2026-06-18-arxiv-2606-20408v1-llm-agent-safety-red-teaming]]

## What's still broken
- Rankings don't transfer OOD → benchmark choice is load-bearing.
- Enterprise ceiling ~37.4% (Claude Opus 4.5, EnterpriseOps-Gym); agents rarely refuse infeasible tasks.
- LLM-as-judge bias propagates and is model-dependent (30× swing on identical defense code) → [[2026-06-18-arxiv-2606-20493v1-contagion-networks-evaluator-bias]]
- Guardrail stacks can't be certified independently of the model they wrap; failures are disjoint across models.
- Security/privilege are separate eval axes most teams don't run → [[toolprivbench]], [[mcp-tdp-bench]]
- Small-sample noise everywhere — multi-seed before trusting a delta.

## Metrics by task activity
- **Tool/function calling** → selection accuracy, arg validity, redundant-call rate, OPUR@k + PED ([[bfcl]], [[toolprivbench]], [[eapo]])
- **Planning / sequential decision** → human-oracle-plan gap, oracle-normalized return, infeasible-task refusal ([[enterpriseops-gym]], [[agentick]])
- **End-to-end assistant** → task success + orchestration overhead (traceback/timeout/tool-failure rate, cost/task) ([[gaia-benchmark]])
- **Conversational tool use** → `pass^k` consistency, policy adherence ([[tau2-bench]])
- **Coding/SWE** → resolved rate + consistency + cost ([[swe-bench]])
- **Multi-agent orchestration** → success vs single-agent baseline, cost/failure delta ([[gaia-benchmark]])
- **Agent-as-judge** → contagion Γ / spectral radius ρ, strategy entropy, per-model judge-vs-truth agreement ([[2026-06-18-arxiv-2606-20493v1-contagion-networks-evaluator-bias]])
- **Safety-critical autonomy** → ASR_CSF objective harm signal, per model+defense pairing ([[nrt-bench]])
- **Adversarial MCP ecosystem** → tool-description-poisoning ASR by risk category ([[mcp-tdp-bench]])
- **Safety behavior shaping** → per-trajectory rubric scores ([[rubas]])
- **Cross-cutting (all activities):** predictive validity, `pass^k` consistency, refusal/feasibility, cost/latency

## Output-quality metrics by functional task (full-text grounded)
- **Content generation / summarization** → faithfulness (no fabrication) *vs* fidelity (no omission) — two axes; coherence, layout, instruction-following ([[deckbench]])
- **Text2Query (NL2SQL)** → execution accuracy gated on intent-grounding ([[bird-python]]); cost/latency at scale via VES*/VCES/CVQ ([[2026-02-25-arxiv-2602-21480v4-text-to-big-sql-cost-metrics]])
- **Data analyst (analysis/insight/RCA)** → relevance/correctness/completeness + tail latency ([[insight-agents]]); RCA trajectory alignment + A@1/A@3 + ZTDR, not just final cause ([[cloud-opsbench]])
- **Code / tool generation** → execution-grounded Pass Rate + coverage + Syn Pass via deterministic evaluator ([[llm4cov]], [[swe-bench]])
- **RAG / grounded QA** → retrieval precision/recall + faithfulness/groundedness + citation accuracy; agentic-loop drift ([[agentic-rag]])
- **Two rules:** verifiable tasks → execution-based correctness (not BLEU/ROUGE); generative tasks → faithfulness is the headline, judge in cohorts with a consistency score ([[jaf]]) and validate per [[2026-06-18-arxiv-2606-20493v1-contagion-networks-evaluator-bias]].

## Harness guidance (priority order)
1. Rank by predictive validity, not aggregate score.
2. Measure success + consistency (`pass^k`) + refusal/feasibility + cost/latency.
3. Freeze the harness, ablate orchestration separately.
4. Treat LLM judges as validated components (≥3 evaluators, same-family pool, track entropy).
5. Deterministic gates before the LLM, not after.
6. Run security/privilege eval as a separate gate.
7. Multi-seed everything.

## Relationships
- synthesizes [[agent-evaluation]]
- relates to [[agent-reliability]], [[agent-security]], [[governance-gap]], [[data-query-agents]], [[data-analysis-agents]], [[llm-as-judge]], [[agentic-rag]]
- compares [[enterpriseops-gym]], [[agentick]], [[gaia-benchmark]], [[bfcl]], [[tau2-bench]], [[swe-bench]], [[livecodebench]], [[mle-bench]], [[bird-benchmark]], [[bird-python]], [[spider-benchmark]], [[cloud-opsbench]], [[deckbench]], [[llm4cov]], [[insight-agents]], [[jaf]], [[nrt-bench]], [[toolprivbench]], [[mcp-tdp-bench]]
