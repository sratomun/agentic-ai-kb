---
type: source
source_type: arxiv
title: "GeoBrowse: A Geolocation Benchmark for Agentic Tool Use with Expert-Annotated Reasoning Traces"
authors: Xinyu Geng, Yanjing Xiao, Yuyang Zhang, Hanwen Wang et al.
url: https://arxiv.org/abs/2604.04017v1
date: 2026-04-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.CL
tags: [science-agents, agent-reliability, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# GeoBrowse: A Geolocation Benchmark for Agentic Tool Use with Expert-Annotated Reasoning Traces

**arXiv:** [2604.04017v1](https://arxiv.org/abs/2604.04017v1) · 2026-04-05 · cs.CL
**Authors:** Xinyu Geng, Yanjing Xiao, Yuyang Zhang, Hanwen Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Deep research agents integrate fragmented evidence through multi-step tool use. BrowseComp offers a text-only testbed for such agents, but existing multimodal benchmarks rarely require both weak visual cues composition and BrowseComp-style multi-hop verification. Geolocation is a natural testbed because answers depend on combining multiple ambiguous visual cues and validating them with open-web evidence. Thus, we introduce GeoBrowse, a geolocation benchmark that combines visual reasoning with knowledge-intensive multi-hop queries. Level 1 tests extracting and composing fragmented visual cues, and Level 2 increases query difficulty by injecting long-tail knowledge and obfuscating key entities. To support evaluation, we provide an agentic workflow GATE with five think-with-image tools and four knowledge-intensive tools, and release expert-annotated stepwise traces grounded in verifiable evidence for trajectory-level analysis. Experiments show that GATE outperforms direct inference and open-source agents, indicating that no-tool, search-only or image-only setups are insufficient. Gains come from coherent, level-specific tool-use plans rather than more tool calls, as they more reliably reach annotated key evidence steps and make fewer errors when integrating into the final decision. The GeoBrowse bernchmark and codes are provided in https://github.com/ornamentt/GeoBrowse

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.04017v1)
