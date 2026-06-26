---
type: source
source_type: arxiv
title: "Multi-Sourced, Multi-Agent Evidence Retrieval for Fact-Checking"
authors: Shuzhi Gong, Richard O. Sinnott, Jianzhong Qi, Cecile Paris et al.
url: https://arxiv.org/abs/2603.00267v1
date: 2026-02-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [knowledge-graph, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# Multi-Sourced, Multi-Agent Evidence Retrieval for Fact-Checking

**arXiv:** [2603.00267v1](https://arxiv.org/abs/2603.00267v1) · 2026-02-27 · cs.AI
**Authors:** Shuzhi Gong, Richard O. Sinnott, Jianzhong Qi, Cecile Paris et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Misinformation spreading over the Internet poses a significant threat to both societies and individuals, necessitating robust and scalable fact-checking that relies on retrieving accurate and trustworthy evidence. Previous methods rely on semantic and social-contextual patterns learned from training data, which limits their generalization to new data distributions. Recently, Retrieval Augmented Generation (RAG) based methods have been proposed to utilize the reasoning capability of LLMs with retrieved grounding evidence documents. However, these methods largely rely on textual similarity for evidence retrieval and struggle to retrieve evidence that captures multi-hop semantic relations within rich document contents. These limitations lead to overlooking subtle factual correlations between the evidence and the claims to be fact-checked during evidence retrieval, thus causing inaccurate veracity predictions. To address these issues, we propose WKGFC, which exploits authorized open knowledge graph as a core resource of evidence. LLM-enabled retrieval is designed to assess the claims and retrieve the most relevant knowledge subgraphs, forming structured evidence for fact verification. To augment the knowledge graph evidence, we retrieve web contents for completion. The above process is implemented as an automatic Markov Decision Process (MDP): A reasoning LLM agent decides what actions to take according to the current evidence and the claims. To adapt the MDP for fact-checking, we use prompt optimization to fine-tune the agentic LLM.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00267v1)
