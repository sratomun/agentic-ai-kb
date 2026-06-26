---
type: concept
tags: [agents, intent-routing, routing, orchestration, harness-engineering]
created: 2026-06-23
updated: 2026-06-23
kind: domain
---

# Intent routing

*Using detected intent as the signal that selects a model, tool, or sub-agent — the systems half of intent understanding.*

## What it is
Once a request's intent is known, routing decides **where it goes**: which model (cheap vs frontier), which tool or skill, which specialized sub-agent, or which workflow. It covers semantic/embedding routers, preference-aligned routers, hybrid local-vs-cloud cascades, and intent-based networking. It is the downstream sibling of [[intent-understanding]] and a core concern of [[harness-engineering]].

## Why it matters
Sending every prompt to one frontier model is slow, costly, and usually unnecessary — routing is the lever that turns intent into spend control. The same hybrid logic that governs intent detection governs routing: **a small fast router handles the common case; escalate only the hard tail.** [[2025-06-19-arxiv-2506-16655-arch-router-aligning-llm-routing-with-human-preferences|Arch-Router]] is the proof that this can be both accurate and cheap — a **1.5B** router **beats GPT-4o and Claude-3.7 at routing (93.17%) while running ~28× faster (~51ms)**.

## What the evidence shows
**Foundations.** Routing splits into *task-based* (classify the query, send to a specialized handler) and *performance-based* (predict which model is good-enough-and-cheapest). Arch-Router reframes it as **preference alignment**: match the query to a natural-language **Domain-Action** policy, then map policy→model in a separate table — so models swap without retraining and decisions are auditable. A compact 1.5B model **out-routes frontier LLMs (93.17%, +7.71%)** at **~51ms, ~28× faster** ([[2025-06-19-arxiv-2506-16655-arch-router-aligning-llm-routing-with-human-preferences|Arch-Router]]). The pattern also lives in open source — see [[semantic-router]] (embedding nearest-neighbor over example utterances) and [[vllm-semantic-router]] (system-level routing for mixture-of-models).

**Recent developments.** Routing is converging on **hybrid cascades** keyed to intent: a large model distills intent into a "soft token" that steers a lightweight retriever + small generator, hitting **0.83s latency at 80.1%** on BFCL ([[2026-02-14-arxiv-2602-13665v1-hyfunc-hybrid-model-cascade-function-calls|HyFunc]]); position work lays out **on-device super-agents** that detect intent locally and escalate to cloud only on complex tasks ([[2025-04-11-arxiv-2504-10519v2-super-agent-system-hybrid-ai-routers|Super Agent / Hybrid AI Routers]]); and e-commerce pushes intent understanding onto the **device itself** ([[2026-05-06-arxiv-2605-04726v1-recgpt-mobile-on-device-intent-understanding|RecGPT-Mobile]]). The retrieval-grounded classifier of [[2025-05-30-arxiv-2506-00210-reic-rag-enhanced-intent-classification-at-scale|REIC]] is itself a routing engine (intent → service queue). Production conversational stacks increasingly wrap all this in constrained **workflow graphs** to keep flexible intent handling inside hard service rules ([[2025-05-29-arxiv-2505-23006v1-production-conversational-agents-workflow-graphs|Workflow Graphs]]).

**Caveat.** The most-used routers in production are open-source libraries ([[semantic-router]], [[vllm-semantic-router]]) and vendor systems that never publish to arXiv — the literature lags the deployment reality here.

## Relationships
- consumes output of [[intent-understanding]]
- part of [[harness-engineering]] and [[multi-agent-systems]] (orchestration)
- cost/latency sibling of [[distillation]] and [[mixture-of-experts]]
- systems/entities: [[arch-router]] · [[semantic-router]] · [[vllm-semantic-router]] · [[katanemo]]
- generalizes to data-source selection in [[mediated-semantic-architecture]]
- routes among [[small-language-models]] and LLMs (local↔cloud, cheap tier vs. fallback)
- the spend-control half is [[agent-finops]] (cost-aware routing)

## Key papers (citation-ranked)
<!-- Auto-maintained by kg-curator enrich. Citations from census/source-note frontmatter. -->
- **5** · 0.6/mo · [[2025-09-24-arxiv-2509-20175-federation-of-agents-capability-fabric|Federation of Agents: A Semantics-Aware Communication Fabric for L…]]
- **5** · 0.3/mo · [[2025-04-11-arxiv-2504-10519v2-super-agent-system-hybrid-ai-routers|Toward Super Agent System with Hybrid AI Routers]]
- **2** · 0.2/mo · [[2025-05-29-arxiv-2505-23006v1-production-conversational-agents-workflow-graphs|A Practical Approach for Building Production-Grade Conversational …]]
- **1** · 0.1/mo · [[2025-07-14-arxiv-2507-10000v1-on-the-role-of-intentionality-in-knowledge-representation-analyzing-sc|On The Role of Intentionality in Knowledge Representation: Analyzi…]]
- **0** · [[2024-10-02-arxiv-2410-01627-intent-detection-in-the-age-of-llms|Intent Detection in the Age of LLMs]]
- **0** · [[2025-06-19-arxiv-2506-16655-arch-router-aligning-llm-routing-with-human-preferences|Arch-Router: Aligning LLM Routing with Human Preferences]]
- **0** · [[2025-05-30-arxiv-2506-00210-reic-rag-enhanced-intent-classification-at-scale|REIC: RAG-Enhanced Intent Classification at Scale]]
