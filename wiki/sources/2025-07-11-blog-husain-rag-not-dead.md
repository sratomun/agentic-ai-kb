---
type: source
source_type: blog
title: "Stop Saying RAG Is Dead"
author: Hamel Husain
co_authors: [Ben Clavié]
outlet: hamel.dev
url: https://hamel.dev/notes/llm/rag/not_dead.html
resource: https://hamel.dev/notes/llm/rag/not_dead.html
date: 2025-07-11
stake: Independent ML consultant (Parlance Labs); the post fronts a 7-part series featuring retrieval researchers, and retrieval/eval is part of his consulting and course remit.
ingested: 2026-06-22
tags: [perspective, agentic-rag, retrieval, evaluation]
---

# Stop Saying RAG Is Dead

**Blog (series intro)** · Hamel Husain with Ben Clavié (hamel.dev) · 2025-07-11 · [link](https://hamel.dev/notes/llm/rag/not_dead.html)

**The take (attributed):** Husain and Clavié argue the "RAG is dead" claim conflates *naive single-vector RAG* (which deserved the criticism) with *retrieval itself* (more important than ever). Million-token context windows don't change the economics of stuffing everything into every query, and LLMs are frozen at training time — so the future is **better retrieval**, not bigger context.

**Stake:** Curatorial — Husain fronts a 7-part series of retrieval researchers; the through-position (retrieval matters, measure it properly) overlaps his evals consulting.

## Argument
The 2023 oversimplification — chunk documents into a vector DB, cosine similarity, done — fails because compressing whole documents into single vectors loses critical information. The series' lessons:
- **IR metrics for RAG are different** (Nandan Thakur): traditional IR optimizes for the #1 result; RAG needs coverage (all the facts), diversity (corroboration), and relevance. Models that ace BEIR often fail at real RAG.
- **Retrieval can reason** (Orion Weller): instruction-following retrievers (Rank1) generate explicit relevance-reasoning traces, surfacing documents naive systems miss.
- **Late interaction beats single vectors** (Antoine Chaffin): ColBERT-style token-level representations preserve detail — a 150M-param model outperforming 7B alternatives on reasoning tasks.
- **Multiple representations + routing** (Bryan Bischof, Ayush Chaurasia): stop seeking the perfect embedding; build specialized indices and route.
- **Context Rot** (Kelly Hong): LLM performance degrades significantly as input length grows, even on simple tasks — "needle in a haystack" benchmarks miss this; thoughtful retrieval/context engineering beats dumping everything in the prompt.
- **You don't need a graph DB** (Jo Kristian Bergum): a CSV or Postgres works for GraphRAG; vector search already uses graphs (HNSW).

## Why it matters / where it cuts
The radar's clearest practitioner rebuttal to the "long context kills RAG" narrative, and it's an **eval argument in disguise**: most "RAG is dead" claims come from measuring retrieval with the wrong metrics (BEIR-style #1-result optimization) and ignoring context rot. It connects [[agentic-rag]] to [[agent-evaluation]] — evaluate retrieval and generation separately, with coverage/diversity metrics, and beware long-context degradation. So what: a credible counter to anyone proposing to delete the retrieval layer because the context window grew; the failure modes (context rot, single-vector information loss) are real and measured.

## Graph
- **Author:** [[hamel-husain]] (with Ben Clavié)
- **Concepts:** [[agentic-rag]] · [[agent-evaluation]]
- **Entities:** model-agnostic (retrieval methods)
- **Raw:** `raw/blogs/2025-07-11-husain-rag-not-dead.md`
