---
type: source
source_type: arxiv
title: Autonomous Event-Driven Multi-Agent Orchestration for Enterprise AI at Scale
authors: Harsh Rao Dhanyamraju, Leonidas Raghav, Aaron Lee (SAP SE)
url: http://arxiv.org/abs/2606.20058v1
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [agentic-ai, arxiv, multi-agent-systems, orchestration, enterprise-scale]
---

# Autonomous Event-Driven Multi-Agent Orchestration for Enterprise AI at Scale

**Why it matters:** This is the production-deployment playbook for the exact
thing ADP would build — hundreds of specialist agents (HR, payroll, finance)
coordinated over continuous event streams, not one-shot chat. From SAP's
applied team, with hard numbers on *what breaks at enterprise scale* (it's agent
discovery, not task complexity) and a scheduler pattern that fixes it.

## The problem they target
Enterprise AI's real goal isn't answering questions on request — it's
continuously monitoring, detecting, and acting on events (alerts, scheduled
jobs, user requests, follow-up signals) across many specialist agents. But
existing multi-agent systems assume discrete request-response workflows and are
barely tested at enterprise scale. Two gaps: (1) no one measures how
orchestration degrades as the agent *registry* grows (finding the right 1–3
agents among 200), and (2) nothing handles continuous event streams — merging
related events, inferring priority, preempting routine work for critical events.

## Method
Two orchestration architectures compared, plus a new scheduling layer:
- **ReAct** — single reasoning loop interleaving reason/act (PydanticAI, with
  parallel A2A tool calls), no upfront planning. Exposes deterministic stoppage
  points between iterations for preemption.
- **DAG Plan & Execute** — a Planner builds a typed, validated execution graph
  upfront; an Executor dispatches nodes to specialist agents over **A2A** in
  parallel batches; a Replanner adapts on checkpoint/interrupt/resume.
  **Two-tier agent discovery** (inspired by Anthropic Skills): retrieve
  lightweight summaries of all agents to select candidates, then load full agent
  cards only for the selected few — keeping prompt context bounded as the
  registry grows.
- **Task Manager** — the entry point for all work, "like an OS process
  scheduler." Events arrive via a message broker without priority; an LLM decides
  create-new-task / merge-into-existing / ignore, then assigns priority. Every
  LLM decision is **validated against config constraints before mutating the
  deterministic backlog** (re-prompt or safe-default fallback so no event is
  dropped). Tasks ranked by a deterministic composite score
  (`base_priority × (1 + time_bonus) + progress_factor`) preventing starvation.
  Preemption and event-merging happen only at defined stoppage points
  (DAG checkpoints; ReAct between iterations).

Notable design stance: the orchestrator schedules and routes — it should **not**
be the component deciding whether a consequential action is safe. Safety stays
with the workflow-specific specialist agents (e.g. an HR comp agent enforces
pay-equity and manager approval; a finance agent enforces posting thresholds
and segregation of duties). HITL requests pause the task and propagate to the
right human, not silently resolved.

## Evaluation & results
Benchmark: **208 scenarios** derived from real enterprise user stories / 393
events / 1,051 agent calls, across three registry scales — Persona (<10 agents),
Department (20–80), Enterprise (200) — and four task types (Simple, Parallel,
Complex, Failure). 200 mock A2A agents across 7 departments (Finance, HR,
Procurement, Revenue, Supply Chain, IT, Customer Support). LLM-as-judge scoring.

- **Scale dominates, not complexity.** Both architectures do well at Persona
  (74–98% correctness), drop at Department (65–80%), and fall at Enterprise
  (32–83%). Counterintuitively, **Simple tasks degrade harder than Complex** at
  scale: Simple 90–96% → 36–54%; Complex holds 73–83%. Reason: the discovery
  bottleneck — finding 1–3 specific agents among 200 is harder than finding 4–7.
- **ReAct beats DAG at Enterprise scale** on every scenario type. DAG "doesn't
  fail fast": its plan-interrupt-replan cycle re-runs noisy discovery and
  re-validates the graph, compounding errors. DAG's failure handling collapses
  93.7% → 68.3% → 32.4% across the three scales. DAG still wins on Complex/Parallel
  at Persona/Department scale (upfront planning finds parallelism) and achieves
  higher precision at every scale, but its recall degrades worst at 200 agents.
- **Task Manager — related-event merging:** +20 percentage points correctness at
  Enterprise scale (ReAct 34%→57%, DAG 35%→56%).
- **Task Manager — priority preemption:** keeps high-priority queue time stable
  regardless of scale, saving **14–75%** of wait time. Without it (FIFO), DAG
  high-priority events wait 5+ minutes at Department/Enterprise (e.g. DAG
  Department 323s→81s = 75% saved; Enterprise 305s→79s = 74% saved).

## So what
This is the closest thing to a reference architecture for the agent fleet ADP
would actually run. Three takeaways worth internalizing: (1) the binding
constraint at scale is **agent discovery/routing**, not model reasoning — invest
in registry design and two-tier discovery before bigger models; (2) **ReAct's
incremental robustness beats DAG's structured planning once the registry is
large and noisy** — don't over-engineer the planner; (3) keep **safety decisions
in the specialist agents, not the orchestrator** — exactly the governance
boundary an HR/payroll platform needs. The Task Manager (priority + merge +
preempt + deterministic backlog) is a clean, portable pattern for turning a
chat assistant into a continuous event-stream scheduler.

**Connects to:** [[multi-agent-systems]] [[agentic-ai]] [[agent-security]]
**Raw:** `raw/arxiv/2606.20058v1.fulltext.md`

## Relationships
- methods: [[react]]
- authored by [[sap]]
