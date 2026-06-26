---
type: concept
tags: [agents, multi-agent, orchestration, evaluation]
created: 2026-06-21
updated: 2026-06-22
source_count: 3
---

# Multi-agent systems

*Coordinating several agents toward a shared goal — orchestration, communication, and the failure modes that emerge when agents work together.*

## What it is
Systems where multiple agents (or one orchestrator plus specialist sub-agents) divide work, communicate, and combine results. It covers orchestration patterns (plan-execute, hierarchical control, role-based crews), the protocols that connect them, and the distinctive ways multi-agent setups break.

## Why it matters
Multi-agent is the default architecture vendors reach for, but more agents is not free: coordination overhead, discovery failures, and bias that propagates between agents can make a multi-agent system *worse* than a single well-prompted one. Knowing when collaboration helps — and how it fails at scale — is the practical question this hub answers.

## What the evidence shows
**2025 foundations.** The defining result was sobering: multi-agent systems often gain little over a single agent, and the **"Why Do MAS Fail?"** study built the first failure taxonomy (MAST) from 1,600+ annotated traces across 7 SOTA frameworks — finding most failures are coordination/specification problems, and that isolated fixes (e.g. "give the CEO agent final say," +9%) help but rarely suffice (→ [[2025-03-17-arxiv-2503-13657v3-why-do-multi-agent-llm-systems-fail]]; the reliability angle is [[agent-reliability]]). The collaboration-mechanisms survey gave the field its vocabulary (actors × types × structures → [[2025-01-10-arxiv-2501-06322v1-multi-agent-collaboration-mechanisms-a-survey-of-llms]]); **agentic-supernet** showed architectures can be *searched* and allocated per-query rather than hand-built (→ [[2025-02-06-arxiv-2502-04180v2-multi-agent-architecture-search-via-agentic-supernet]]); and a structured **risk taxonomy** named the three multi-agent failure modes — miscoordination, conflict, collusion (→ [[2025-02-19-arxiv-2502-14143v1-multi-agent-risks-from-advanced-ai]]). Evaluation moved to collaboration-quality metrics and topology comparisons (MultiAgentBench → [[2025-03-03-arxiv-2503-01935v1-multiagentbench-evaluating-the-collaboration-and-competition-of-llm]]) and society-scale simulation (AgentSociety → [[2025-02-12-arxiv-2502-08691v2-agentsociety-large-scale-simulation-of-llm-driven-generative]]).

**2026 developments.**
- **Scale, not task complexity, is the orchestration bottleneck.** Across 208 enterprise scenarios, correctness held at small registries (74–98%) but degraded at 200 agents (32–83%) — *simple* tasks degraded hardest, because finding 1–3 relevant agents among 200 is the failure point. Two-tier discovery is the mitigation (SAP → [[2026-06-18-arxiv-2606-20058v1-event-driven-multi-agent-orchestration-enterprise]]). Match architecture to registry scale, not complexity.
- **Agents judging agents form a contagion network:** evaluator bias propagates across hops; mixing model families amplifies it; ≥3 diverse evaluators cut effective bias ~72% (→ [[2026-06-18-arxiv-2606-20493v1-contagion-networks-evaluator-bias]]).
- **LLM-planner-over-specialist-skills is robust:** a frozen LLM choosing among pretrained RL policies matched a hand-built behavior tree with zero rule authoring (→ [[2026-06-18-arxiv-2606-20014v1-hierarchical-control-multi-agent-games]]). Keep consequential-action safety in the specialists, not the orchestrator.
- **Reliability is a runtime control problem** (self-healing orchestrators: 98.8% success, silent failures → 0% → [[2026-05-31-arxiv-2606-01416v1-self-healing-agentic-orchestrators]]; cf. [[self-healing-orchestrator]]). **Coordination needs protocols, not prompts** → [[agent-protocols]]. Enterprise attack vectors trace to tool orchestration + memory (AgenticCyOps → [[2026-03-10-arxiv-2603-09134v1-agenticcyops-securing-enterprise-mas]]). Orchestration overhead can backfire — a negative ablation (ChromaFlow) in [[agent-evaluation]].

## Includes (sub-themes folded here)
Folds in: **orchestration frameworks** (AutoGen/CrewAI/LangGraph-style, ~1,700 papers), agent-architecture search, and role/communication design.

## Relationships
- Anthropic: orchestrator-worker beat single-agent Opus 4 by 90.2% on research (~15x token cost) → [[2025-06-13-blog-anthropic-multi-agent-research-system]]
- debate: [[debate-agents-vs-workflows]] ([[anthropic]] simplicity vs autonomy)
- methods: [[react]], [[self-healing-orchestrator]]
- protocols: [[mcp]], [[a2a-protocol]], [[acp-protocol]] (see [[agent-protocols]])
- security: [[agent-security]], [[agenticcyops]]
- evaluation: [[agent-evaluation]] ([[enterpriseops-gym]], [[gaia-benchmark]])
- studied by [[sap]]
- a form of [[agentic-ai]]
- default model tier [[small-language-models]] (heterogeneous systems: SLM by default, LLM selectively)
- exemplar: [[google-deepmind]] Co-Scientist → [[2026-05-19-blog-google-deepmind-co-scientist-multi-agent]]

## Key 2025 papers (citation-ranked)
- **473** · [[2025-01-10-arxiv-2501-06322v1-multi-agent-collaboration-mechanisms-a-survey-of-llms|Multi-Agent Collaboration Mechanisms: A Survey of LLMs]]
- **402** · [[2025-03-17-arxiv-2503-13657v3-why-do-multi-agent-llm-systems-fail|Why Do Multi-Agent LLM Systems Fail?]]
- **164** · [[2025-02-12-arxiv-2502-08691v2-agentsociety-large-scale-simulation-of-llm-driven-generative|AgentSociety: Large-Scale Simulation of LLM-Driven Generative Agents Advances U...]]
- **150** · [[2025-02-19-arxiv-2502-14143v1-multi-agent-risks-from-advanced-ai|Multi-Agent Risks from Advanced AI]]
- **125** · [[2025-03-03-arxiv-2503-01935v1-multiagentbench-evaluating-the-collaboration-and-competition-of-llm|MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents]]
- **125** · [[2025-02-06-arxiv-2502-04180v2-multi-agent-architecture-search-via-agentic-supernet|Multi-agent Architecture Search via Agentic Supernet]]
