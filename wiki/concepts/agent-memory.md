---
type: concept
tags: [agents, memory, self-improvement, long-horizon]
created: 2026-06-21
updated: 2026-06-22
source_count: 2
---

# Agent memory

*How agents carry state beyond a single context window — storing experience, distilling it, and reusing it to stay coherent over long horizons.*

## What it is
The machinery that lets an agent remember across turns, sessions, and tasks: raw trajectory stores, distilled "experience," graph/temporal memory, and increasingly RL-trained policies that decide *what* to keep. It spans bolt-on vector stores through to memory baked into model weights.

## Why it matters
Durable memory is the precondition for agents that **compound in value** rather than resetting every session — the difference between a clever demo and a colleague that gets better over time. It's also one of the most active and best-cited 2025 areas (A-MEM and Mem0 are among the year's most-cited agent papers) and, crucially, an attack surface: poisoned memory persists across steps.

## What the evidence shows
**2025 foundations** (the architectures everything else builds on). Three reference designs defined the year: **A-MEM** made memory *agentic* — Zettelkasten-style interlinked notes the agent itself writes and links, beating prior SOTA across six base models (→ [[2025-02-17-arxiv-2502-12110v11-a-mem-agentic-memory-for-llm-agents]]); **Mem0** made it *production-scale* — dynamically extracting and consolidating salient facts for **+26% over OpenAI's memory on LOCOMO at lower compute**, with a graph variant for relational structure (→ [[2025-04-28-arxiv-2504-19413v1-mem0-building-production-ready-ai-agents-with-scalable]]); and **Zep** (Graphiti) made it *temporal* — a knowledge-graph memory beating MemGPT on DMR with **~18% higher accuracy and ~90% lower latency** on enterprise tasks (→ [[2025-01-20-arxiv-2501-13956v1-zep-a-temporal-knowledge-graph-architecture-for-agent]]; cf. [[knowledge-graph]]). By year-end the consensus was that long/short-term taxonomies are insufficient and the frontier is **RL-trained memory** — agents that *learn* what to store/update/retrieve (MemAgent extends DAPO to extrapolate 8K→3.5M-token tasks; MEM1 keeps memory constant-size; Memory-R1 learns ADD/UPDATE operations).

**2026 developments.** The question shifted from *what to store* to *what to keep*: filtering durable lessons from lucky one-offs (MAA — signed-evidence accumulation, best in 14/16 settings, ~75% lower optimization cost → [[2026-06-18-arxiv-2606-20475v1-memory-driven-agent-self-evolution]]), and showing most of memory's value is the *meta-skill* of building and reusing it (CoD — self-updated context jumped 0.28→0.76 and transferred across domains → [[2026-06-18-arxiv-2606-20002v1-long-lifecycle-agents-cross-domain]]). Elastic orchestration (AutoAgent → [[2026-03-10-arxiv-2603-09716v1-autoagent-evolving-cognition-elastic-memory]]) and tool-graph experience memory as RL state (SEARL → [[2026-04-09-arxiv-2604-07791v3-searl-policy-tool-graph-memory]]) are the current engineering frontier.

**Caveat.** Memory is an attack surface — backdoor triggers persist most strongly through the memory stage (~78%) → [[2026-01-08-arxiv-2601-04566v2-backdooragent-unified-backdoor-attacks]] and [[agent-security]]. The training-loop side now has its own hub, [[self-evolving-agents]].

## Relationships
- methods: [[grpo]]
- structure: [[knowledge-graph]] (graph/temporal memory)
- training loop: [[self-evolving-agents]], [[agentic-rl]]
- security: [[agent-security]] (memory-stage backdoors)
- relates to [[mistral]]
- capability of [[agentic-ai]]
- a hard case for [[small-language-models]] agents (lightweight memory on small models)
- small-model variant: [[slm-agent-memory]]

## Key 2025 papers (citation-ranked)
- **651** · [[2025-02-17-arxiv-2502-12110v11-a-mem-agentic-memory-for-llm-agents|A-MEM: Agentic Memory for LLM Agents]]
- **412** · [[2025-04-28-arxiv-2504-19413v1-mem0-building-production-ready-ai-agents-with-scalable|Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory]]
- **213** · [[2025-01-20-arxiv-2501-13956v1-zep-a-temporal-knowledge-graph-architecture-for-agent|Zep: A Temporal Knowledge Graph Architecture for Agent Memory]]
- **185** · [[2025-10-06-arxiv-2510-04618v3-agentic-context-engineering-evolving-contexts-for-self-improving|Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models]]
- **179** · [[2025-12-15-arxiv-2512-13564v2-memory-in-the-age-of-ai-agents|Memory in the Age of AI Agents]]
- **166** · [[2025-07-03-arxiv-2507-02259v1-memagent-reshaping-long-context-llm-with-multi-conv|MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent]]
- **150** · [[2025-06-18-arxiv-2506-15841v2-mem1-learning-to-synergize-memory-and-reasoning-for|MEM1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents]]
- **127** · [[2025-08-27-arxiv-2508-19828v5-memory-r1-enhancing-large-language-model-agents-to|Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories...]]
