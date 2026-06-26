---
type: source
source_type: arxiv
title: "AgentCAT: An LLM Agent for Extracting and Analyzing Catalytic Reaction Data from Chemical Engineering Literature"
authors: Wei Yang, Zihao Liu, Tao Tan, Xiao Hu et al.
url: https://arxiv.org/abs/2602.18479v1
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: physics.chem-ph
tags: [knowledge-graph, arxiv, auto-ingested]
---

# AgentCAT: An LLM Agent for Extracting and Analyzing Catalytic Reaction Data from Chemical Engineering Literature

**arXiv:** [2602.18479v1](https://arxiv.org/abs/2602.18479v1) · 2026-02-10 · physics.chem-ph
**Authors:** Wei Yang, Zihao Liu, Tao Tan, Xiao Hu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This paper presents a large language model (LLM) agent named AgentCAT, which extracts and analyzes catalytic reaction data from chemical engineering papers, %and supports natural language based interactive analysis of the extracted data. AgentCAT serves as an alternative to overcome the long-standing data bottleneck in chemical engineering field, and its natural language based interactive data analysis functionality is friendly to the community. AgentCAT also presents a formal abstraction and challenge analysis of the catalytic reaction data extraction task in an artificial intelligence-friendly manner. This abstraction would help the artificial intelligence community understand this problem and in turn would attract more attention to address it. Technically, the complex catalytic process leads to complicated dependency structure in catalytic reaction data with respect to elementary reaction steps, molecular behaviors, measurement evidence, etc. This dependency structure makes it challenging to guarantee the correctness and completeness of data extraction, as well as representing them for analysis. AgentCAT addresses this challenge and it makes four folds of technical contributions: (1) a schema-governed extraction pipeline with progressive schema evolution, enabling robust data extraction from chemical engineering papers; (2) a dependency-aware reaction-network knowledge graph that links catalysts/active sites, synthesis-derived descriptors, mechanistic claims with evidence, and macroscopic outcomes, preserving process coupling and traceability; (3) a general querying module that supports natural-language exploration and visualization over the constructed graph for cross-paper analysis; (4) an evaluation on $\sim$800 peer-reviewed chemical engineering publications demonstrating the effectiveness of AgentCAT.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.18479v1)
