---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Enhancing Text2Cypher with Schema Filtering"
authors: Makbule Gulcin Ozsoy (Neo4j)
url: https://arxiv.org/abs/2505.05118
date: 2025-05-08
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, text-to-cypher, semantic-parsing, knowledge-graph]
---

# Enhancing Text2Cypher with Schema Filtering

**arXiv [2505.05118](https://arxiv.org/abs/2505.05118)** · 2025-05-08 · Neo4j

**Significance.** The schema-linking cost lever for graph querying: prune the schema to what the question needs and small models get both cheaper and *more* accurate. Grounds the "schema linking dominates" claim in [[semantic-parsing]].

## Abstract
Studies five schema-filtering strategies for Text2Cypher — two static (Enhanced, Base) and three dynamic (Exact-Match pruning; NER-masked + Exact-Match; Similarity pruning) — on a 22,093-train / 2,471-test public subset with Llama-3.1-8B, Qwen2.5-7B, Gemini-1.5-Flash, scored by Google-BLEU and Exact-Match.

## From the paper (full-text, via subagent)
**Contribution / method.** Inserts a schema-filtering stage before Cypher generation, comparing static vs dynamic pruning of the graph schema passed in the prompt.
**Results.** A ~150-token base prompt balloons past 2,700 with full schema; **exact-match pruning cuts P95 tokens 2,697 → 529 (~6×)**. Cost for 20K instances drops Gemini-2.0-Flash **$2.7 → $1.0**, Claude-3.5-Haiku $14.7 → $5.5, self-hosted Llama-3.1-8B $112.5 → $42.0. **Best accuracy comes from exact-match pruning**, especially for small models; large long-context models lose <5% (lexical) / ~2% (execution) with shorter prompts but still save money.
**Takeaway.** Schema linking is the highest-leverage knob in graph parsing: smaller prompt, lower cost, higher small-model accuracy. The same lesson as the "MCP tax" in [[tool-use]] — schema is a representation problem.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[semantic-parsing]] · [[knowledge-graph]]
- **Entities:** [[cypher]] · [[neo4j]] · [[text2cypher-dataset]]
- **Raw:** full-text (alphaXiv, read via subagent) 2026-06-23
