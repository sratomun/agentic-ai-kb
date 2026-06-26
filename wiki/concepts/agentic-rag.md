---
type: concept
tags: [agents, rag, retrieval, reliability]
created: 2026-06-21
updated: 2026-06-22
source_count: 1
---

# Agentic RAG

*Retrieval-Augmented Generation turned into an autonomous loop — the agent decides what to retrieve, when, and how to use it.*

## What it is
RAG that has become a sequential decision process rather than a one-shot fetch-then-generate: the LLM coordinates multi-step reasoning, dynamic memory, and iterative retrieval, choosing queries and stopping conditions as it goes. It's the engine under [[deep-research-agents|deep-research agents]] and a specialization of [[tool-use]] (retrieval as a tool, in a loop).

## Why it matters
The moment retrieval runs inside an autonomous loop, the failure modes change — and get worse: errors compound across hops, memory can be poisoned, and retrieval can drift off-target. Before you point a RAG agent at consequential data, the 2025–26 framing worth adopting is to treat it as a **control problem** (policies, state, oversight), not a search box. This is also the highest-traffic enterprise pattern, so the reliability stakes are real.

## What the evidence shows
**2025 foundations.** The idea crystallized that reasoning models stall on **knowledge insufficiency** — they reason confidently past what they know. **Search-o1** fixed this by inserting an agentic-RAG step plus a "Reason-in-Documents" module that refines retrieved passages before they re-enter the reasoning chain, the first framework to fold autonomous search into o1-style reasoning (→ [[2025-01-09-arxiv-2501-05366v1-search-o1-agentic-search-enhanced-large-reasoning-models]]). The **Agentic RAG survey** then formalized the shift from static fetch-then-generate to adaptive multi-step retrieval (→ [[2025-01-15-arxiv-2501-09136v4-agentic-retrieval-augmented-generation-a-survey-on-agentic]]). By spring this matured into *trained* deep research: **WebThinker** gave reasoning models autonomous search + report-drafting, trained with iterative online DPO, beating proprietary systems on GPQA/GAIA/HLE (→ [[2025-04-30-arxiv-2504-21776v2-webthinker-empowering-large-reasoning-models-with-deep-research]]) — the lineage that became [[deep-research-agents]].

**2026 developments.** The framing turned to control and reliability: the SoK formalizes agentic RAG as a finite-horizon POMDP with explicit control policies and state transitions, taxonomized over planning, retrieval orchestration, memory, and tool invocation (→ [[2026-03-07-arxiv-2603-07379v1-sok-agentic-rag-taxonomy]]). It names the systemic risks of running retrieval inside an autonomous loop — compounding hallucination propagation, memory poisoning, retrieval misalignment, cascading tool-execution vulnerabilities — and shows static evaluation underspecifies these systems, tying directly to [[agent-evaluation]].

## Relationships
- related 2025 theme: [[deep-research-agents]]
- structured by [[knowledge-graph]] ([[graphrag|GraphRAG]])
- a specialization of [[tool-use]] + [[agentic-ai]]
- shares risks with [[agent-security]], [[agent-memory]]
- evaluation caveats in [[agent-evaluation]]
- used as external memory in [[slm-agent-memory]] (retrieval compensates for small context)

## Key 2025 papers (citation-ranked)
- **429** · [[2025-01-09-arxiv-2501-05366v1-search-o1-agentic-search-enhanced-large-reasoning-models|Search-o1: Agentic Search-Enhanced Large Reasoning Models]]
- **318** · [[2025-01-15-arxiv-2501-09136v4-agentic-retrieval-augmented-generation-a-survey-on-agentic|Agentic Retrieval-Augmented Generation: A Survey on Agentic RAG]]
- **279** · [[2025-04-30-arxiv-2504-21776v2-webthinker-empowering-large-reasoning-models-with-deep-research|WebThinker: Empowering Large Reasoning Models with Deep Research Capability]]
