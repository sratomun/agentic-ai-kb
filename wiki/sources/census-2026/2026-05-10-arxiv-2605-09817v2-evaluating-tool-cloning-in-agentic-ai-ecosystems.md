---
type: source
source_type: arxiv
title: "Evaluating Tool Cloning in Agentic-AI Ecosystems"
authors: Taein Kim, David Jiang, Yuepeng Hu, Yuqi Jia et al.
url: https://arxiv.org/abs/2605.09817v2
date: 2026-05-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.SE
tags: [coding-agents, agent-economies, agent-security, agent-protocols, agent-skills, arxiv, auto-ingested]
---

# Evaluating Tool Cloning in Agentic-AI Ecosystems

**arXiv:** [2605.09817v2](https://arxiv.org/abs/2605.09817v2) · 2026-05-10 · cs.SE
**Authors:** Taein Kim, David Jiang, Yuepeng Hu, Yuqi Jia et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agent tools are becoming a core interface through which LLM agents access external data, services, and execution environments. As these tools are distributed through public marketplaces, raw tool counts may substantially overstate ecosystem diversity if many repositories are cloned, lightly modified, or derived from shared templates. Such hidden duplication can contaminate benchmark splits, propagate vulnerable implementations, bias measurements of tool-use generalization, and raise provenance, attribution, and intellectual-property concerns. We present, to our knowledge, the first large-scale measurement study of tool cloning in agentic AI ecosystems. We curate a unified dataset from multiple public platforms, covering 7,508 Model Context Protocol (MCP) repositories with 87,564 extracted tools and 1,353 Skills repositories with 12,447 tools, for a total of 8,861 repositories and 100,011 tool entries. To measure implementation-level duplication, we build a repository-level auditing pipeline using complementary lexical and fuzzy-structural similarity metrics, and compute pairwise similarity across MCP-to-MCP, Skills-to-Skills, and MCP-to-Skills repository pairs. We further manually verify 100 sampled pairs per MCP and Skills ecosystem across similarity-score buckets to calibrate how often high similarity reflects true code cloning. Our analysis shows that cloning is not an isolated artifact: high-similarity regions appear across comparison settings, and 60\% of high-Jaccard candidates and 85\% of high-ssdeep candidates in the MCP ecosystem are manually verified as clones. These results indicate that tool cloning is a pervasive and severe source of hidden duplication in agent-tool ecosystems. They further suggest that agent-tool datasets and benchmarks should account for repository provenance and implementation similarity when measuring tool diversity or constructing evaluation splits.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-economies|Agent economies]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.09817v2)
