---
type: concept
tags: [agents, knowledge-graph, retrieval, memory]
created: 2026-06-21
updated: 2026-06-22
census_count: 172
kind: crosscutting
---

# Knowledge graphs (for agents)

*Structured, relational knowledge — knowledge graphs, ontologies, GraphRAG — as agent memory and retrieval infrastructure.*

## What it is
The use of graph-structured knowledge (entities + relations + hierarchy) as the substrate an agent reads from and writes to, instead of flat vector chunks. It spans temporal knowledge-graph memory, ontology-grounded reasoning, and [[graphrag|GraphRAG]]-style retrieval. ~172 KG papers, ~30 GraphRAG, ~75 ontology in the census.

## Why it matters
For agents that must reason over *your* organization's structured knowledge — entities, relationships, a semantic-layer contract — graphs give relational dependencies and multi-hop retrieval that flat vector stores can't. This is where [[agent-memory]], [[agentic-rag]], and [[data-query-agents|data querying]] converge, and it's the most direct path from "agent that searches documents" to "agent that reasons over a knowledge base." Notably there is **no dedicated knowledge-graph-agent survey yet** — a genuine white space worth watching.

## What the evidence shows
**2025 foundations.** Graphs went from a research curiosity to a **production agent-memory architecture**. The landmark is **Zep/Graphiti** — a temporally-aware knowledge-graph memory that beats MemGPT on the DMR benchmark and, on harder enterprise tasks (cross-session synthesis, long-term context), delivers **~18% higher accuracy and ~90% lower latency** than flat-retrieval baselines; notably it builds the graph deterministically rather than via LLM-generated queries, to avoid schema drift and hallucination (→ [[2025-01-20-arxiv-2501-13956v1-zep-a-temporal-knowledge-graph-architecture-for-agent]]). [[mem0|Mem0]]'s graph variant independently confirmed the pattern — relational structure on top of semantic embeddings improves complex reasoning. This is why graph memory keeps surfacing in [[agent-memory]].

**State of play.** Graph-structured memory now has its own taxonomy and lifecycle — extraction → storage → retrieval → evolution — captured in the 2026 graph-based agent-memory survey below. **GraphRAG** is the retrieval counterpart: graph traversal for multi-hop and global-sensemaking queries where flat RAG fails → [[graphrag]]. The open gap: there is still **no dedicated knowledge-graph-agent survey** — a white space worth watching.

## Key survey
- [[2026-02-05-arxiv-2602-05665v1-survey-graph-based-agent-memory|Graph-based Agent Memory: taxonomy, techniques, applications]]

## Relationships
- key method: [[graphrag|GraphRAG]]
- structures [[agent-memory]] and [[agentic-rag]]
- queried by [[data-query-agents]]
- grounds user intent via [[intent-grounding]] (ontology / entity linking)
- queried in natural language via [[text-to-cypher]] ([[cypher]])
- exposed over live sources as a [[virtual-knowledge-graph]] in [[mediated-semantic-architecture]]
- contrast with flat retrieval in [[tool-use]]
- a capability layer of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **213** · [[2025-01-20-arxiv-2501-13956v1-zep-a-temporal-knowledge-graph-architecture-for-agent|Zep: A Temporal Knowledge Graph Architecture for Agent Memory]]
