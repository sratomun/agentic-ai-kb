---
type: concept
tags: [agents, tool-use, mcp, interfaces]
created: 2026-06-21
updated: 2026-06-22
source_count: 3
---

# Tool use

*How agents reach the outside world — calling tools, APIs, and services — and the cost, latency, and safety of that interface.*

## What it is
The interface layer between an agent and external systems: function/tool calling, the schemas that describe tools, and the protocols (MCP-adjacent) that carry them. It's where an agent stops "thinking" and starts "doing" — and where most production failures actually happen.

## Why it matters
The tool interface is a cost, latency, and safety lever, not a plumbing detail. Static single-shot endpoints force one round-trip plus one LLM round per step — dominating latency and token spend on multi-step work — and every tool an agent can call is also something it can misuse. Get this layer right before agents touch real systems.

## What the evidence shows
**2025 foundations.** The big shift was from *teaching* tool use by imitation to *training* it with RL. ToolRL showed coarse answer-matching rewards fail and fine-grained reward design is what makes tool selection generalize (+17% over base, +15% over SFT → [[2025-04-16-arxiv-2504-13958v1-toolrl-reward-is-all-tool-learning-needs]]); ReTool interleaved real-time code execution into reasoning for **67% on AIME** (→ [[2025-04-15-arxiv-2504-11536v2-retool-reinforcement-learning-for-strategic-tool-use-in]]; the RL side lives in [[agentic-rl]]). Data scarcity got addressed by synthetic multi-turn pipelines (APIGen-MT → [[2025-04-04-arxiv-2504-03601v4-apigen-mt-agentic-pipeline-for-multi-turn-data]]), and evaluation matured into dual-control settings where the *user* also acts (τ²-Bench → [[2025-06-09-arxiv-2506-07982v1-2-bench-evaluating-conversational-agents-in-a-dual]]; cf. [[tau2-bench]]).

**2026 developments.** Attention turned to the *interface itself* as a cost/latency/safety lever:
- **Tool programs** consolidate a whole workflow into one service-side object: latency cut up to 53.4%, client traffic up to 96.1% (ToolPro → [[2026-06-18-arxiv-2606-19992v1-tool-programs-agentic-web-services]]). The write-safety pattern: READ/WRITE effect typing, exactly-once replay of WRITEs, fail-closed fallback, WebAssembly sandboxing (ties to [[agent-security]]).
- **The "MCP tax" is measurable:** eager schema injection costs ~10k–60k tokens/turn and degrades reasoning near ~70% context use; gated lazy loading cuts per-turn tool tokens ~95% (Tool Attention → [[2026-04-23-arxiv-2604-21816v1-tool-attention-mcp-tax]]). **Schemas are a representation problem, not a size problem:** compiling JSON to token-efficient text (TSCG) restores small models from ~0%→84%+ with 52–57% token savings (→ [[2026-05-04-arxiv-2605-04107v1-tscg-tool-schema-compilation]]; cf. [[tscg]], [[bfcl]]).
- **Reliability/policy:** policy-adherent tool calling via structured state → [[2026-06-18-arxiv-2606-20529v1-ledgeragent-policy-adherent-tool-calling]]; over-privileged tool selection → [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection]]. Skills sit above tool calls → [[agent-skills]]; tool-use-in-a-loop is [[agentic-rag]].

## Relationships
- design tools FOR agents (Anthropic) → [[2025-09-11-blog-anthropic-writing-tools-for-agents]]; built-in tools (OpenAI) → [[2025-03-11-blog-openai-new-tools-for-building-agents]]
- related 2025 theme: [[deep-research-agents]]
- standard: [[mcp]] (+ peer protocols in [[agent-protocols]])
- benchmarks: [[toolprivbench]], [[tau2-bench]], [[bfcl]]
- methods: [[react]], [[dart]], [[eapo]]
- layers above: [[agent-skills]], [[agentic-rag]]
- training: [[agentic-rl]]
- upstream of [[intent-understanding]] (intent → structured tool call)
- capability of [[agentic-ai]]
- the reliability frontier for [[small-language-models]] (small models struggle to emit valid tool calls)

## Key 2025 papers (citation-ranked)
- **309** · [[2025-04-15-arxiv-2504-11536v2-retool-reinforcement-learning-for-strategic-tool-use-in|ReTool: Reinforcement Learning for Strategic Tool Use in LLMs]]
- **280** · [[2025-04-16-arxiv-2504-13958v1-toolrl-reward-is-all-tool-learning-needs|ToolRL: Reward is All Tool Learning Needs]]
- **275** · [[2025-06-09-arxiv-2506-07982v1-2-bench-evaluating-conversational-agents-in-a-dual|$τ^2$-Bench: Evaluating Conversational Agents in a Dual-Control Environment]]
- **130** · [[2025-04-04-arxiv-2504-03601v4-apigen-mt-agentic-pipeline-for-multi-turn-data|APIGen-MT: Agentic Pipeline for Multi-Turn Data Generation via Simulated Agent-...]]
