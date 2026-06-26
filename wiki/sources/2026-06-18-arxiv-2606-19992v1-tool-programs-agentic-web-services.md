---
type: source
source_type: arxiv
title: "Beyond Static Endpoints: Tool Programs as an Interface for Flexible Agentic Web Services"
authors: Mugeng Liu, Shuoqi Li, Yixuan Zhang, Yun Ma (Peking University)
url: http://arxiv.org/abs/2606.19992v1
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [tool-use, agentic-ai, agent-security, mcp, agentic-web, arxiv]
---

# Beyond Static Endpoints: Tool Programs as an Interface for Flexible Agentic Web Services

**Why it matters:** As agents call more services, the interface itself — one-API-call-at-a-
time — becomes the bottleneck: every step is a network round trip plus an LLM reasoning
round, and partial failures duplicate writes. ToolPro reframes tool use as submitting a
small *program* the service runs as a unit, with exactly-once guarantees on state changes.
A concrete, MCP-adjacent pattern for making agent-to-service calls faster, cheaper, and
safer to retry.

## The problem they target
In the "agentic web," LLM agents orchestrate web services to complete multi-step workflows
with loops, conditionals, joins, and retries — but services still expose **static endpoints
designed for single-shot queries**. To realize control flow, the agent must externalize the
whole workflow into a brittle sequence of endpoint calls interleaved with reasoning. The
authors argue the inefficiency is **representational**: endpoint sequences fragment a
coherent plan into local next-call decisions. As workflows grow, this (i) inflates latency
via repeated round-trip time (RTT) and per-step decision overhead, (ii) over-/under-fetches
because control logic lives outside the service, and (iii) makes recovery brittle — partial
failures trigger retries that **duplicate state-modifying calls and corrupt service state**.

## Method
**ToolPro** makes "tool intent" first-class by representing a workflow as an **executable
tool program**: structured control flow whose only external operations are `Call(e, a)`
endpoint invocations, each annotated with an explicit effect type (**READ** vs **WRITE**).
The agent submits one program; a service-side runtime compiles, optionally repairs, and
executes it as a unit. Four pieces:
- **Constrained surface** — submitted programs allow only structured control flow
  (if/else, loops), external interaction solely through `Call(·)` with effect annotations,
  and no exceptions/threads/dynamic-linking/unsafe-memory or ad-hoc networking/filesystem
  access. This keeps compiler diagnostics and traces analyzable and enforceable.
- **Constraint-guided construction** — a synthesize→project→compile→execute pipeline:
  client-side synthesis with lightweight checks (endpoint coverage, control-flow skeleton,
  value-flow sanity) → server-side deterministic projection `Π(·)` into the canonical
  surface → compile/execute in sandbox with **bounded in-place repair** driven by compiler
  diagnostics and runtime traces (localized edits to the failing call site or block) →
  **safe fallback** to stepwise calling if the attempt budget or constraints are exceeded.
- **Effect-aware replay (exactly-once WRITEs)** — the runtime intercepts every dynamic
  call. READs are always re-issued (safe); completed WRITEs are logged (history `H` +
  working log `W`) and, on repair-driven re-execution, matched to the earliest unused
  entry and **replayed from cache rather than re-emitted**. If a repair changes the
  arguments/order of an already-committed WRITE prefix, ToolPro disables replay and falls
  back — turning silent semantic divergence into an explicit, auditable condition. A
  proposition proves each completed WRITE is emitted at most once. Idempotency keys
  strengthen matching; meaningful nondeterminism without idempotency triggers fallback.
- **Profile-driven consolidation policy** — maintains moving averages of RTT, per-step
  decision cost, and build cost; predicts net benefit `ΔT = (N−1)·(RTT + decision) − build`
  and runs program mode only when `ΔT > 0`, else reverts to stepwise calling.
- **Implementation:** instantiated over MCP-style services with the runtime in
  **WebAssembly** (strong sandbox for untrusted LLM-generated code, capability-style host
  interface exposing only the `Call` stub, low-overhead portable execution). Code released.

## Evaluation & results
- **Benchmarks:** three open-source apps (Memos, Directus, MinIO) exposed as MCP-style
  services, each with a read-only (`.r`) and read-write (`.w`) workflow parameterized by
  procedural length N; plus four supplemental complex workflows (cbench1–4) stressing
  nondeterministic retrieval, branching, coordinated writes, non-idempotent effects, and
  cross-service execution. **Metrics:** end-to-end latency, client-side traffic, and task
  accuracy. **Baselines:** stepwise MCP (MWS), ToolPro-step, ToolPro-prog, full ToolPro.
- **Headline:** up to **53.4% lower end-to-end latency** and up to **96.1% less client-side
  traffic** (paper-wide), with gains growing under higher network latency and workflow
  complexity. Traffic reduction reaches up to 85.3% on the fixed-N procedural workflows,
  driven mainly by fewer client-to-LLM exchanges (one compact program vs. repeatedly
  re-transmitting tool specs and intermediate context across N rounds).
- **Complex realistic workflows (cbench1–3):** latency 30.16s → 17.91s (−40.6%), task
  accuracy 0.60 → 0.93, client-side LLM latency 14.98s → 7.08s (−52.8%). **Cross-service
  (cbench4):** latency 52.68s → 24.54s (−53.4%), traffic −96.1%, accuracy 0.20 → 0.80.
- **Reliability:** program-mode success tracks the LLM's coding ability — on Rust-based
  cbench2, qwen3-coder-flash hit 80% success while gpt-5.1 and gemini-3-flash-preview hit
  100% with no compilation failures. Disabling replay over 15 runs raised average latency
  17.92s → 21.45s (+19.7%) and fallbacks 0/15 → 3/15. ToolPro "fails closed" when replay
  safety can't be guaranteed, and fallback doesn't erase the overall gains.

## So what
Two ideas worth carrying into ADP's agent-platform thinking. First, the *interface* between
agents and services is itself a performance and cost lever — consolidating a workflow into
one submitted program cuts the LLM round-trips that dominate both latency and token spend
(up to ~96% traffic reduction). Second, and more important for anything touching payroll/HR
systems: **effect-typed calls + exactly-once replay + fail-closed fallback** is a clean
safety pattern for the dangerous part of tool use — agents that write. The WebAssembly
sandbox for untrusted LLM-generated code is also the right instinct. This is MCP-adjacent
infrastructure; the design points (READ/WRITE typing, retry-safe semantics, auditable
fallback) are exactly what you'd want any agent-to-service layer to enforce before it's
allowed near production systems.

**Connects to:** [[tool-use]] [[agent-security]]
**Raw:** `raw/arxiv/2606.19992v1.fulltext.md`
