---
type: source
source_type: arxiv
title: "RepoDoc: A Knowledge Graph-Based Framework to Automatic Documentation Generation and Incremental Updates"
authors: Dong Xu, Mingwei Liu, Xiwen Wang, Jianfeng Zhong et al.
url: https://arxiv.org/abs/2604.26523v1
date: 2026-04-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 1
primary: cs.SE
tags: [coding-agents, knowledge-graph, agent-skills, arxiv, auto-ingested]
---

# RepoDoc: A Knowledge Graph-Based Framework to Automatic Documentation Generation and Incremental Updates

**arXiv:** [2604.26523v1](https://arxiv.org/abs/2604.26523v1) · 2026-04-29 · cs.SE
**Authors:** Dong Xu, Mingwei Liu, Xiwen Wang, Jianfeng Zhong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Maintaining up-to-date, comprehensive documentation for large codebases is a persistent challenge. Recent progress in automated documentation has moved from template-based rules to large language models (LLMs), yet existing tools still process source code as flat fragments, producing isolated documents that lack semantic structure. This design also leads to excessive token consumption and slow generation, while failing to capture how code changes propagate across dependencies. We propose RepoDoc, a system that uses a repository knowledge graph (RepoKG) as the semantic foundation for the entire documentation lifecycle. Our framework consists of three stages: (1) RepoKG construction, which extracts code entities and their relationships; (2) module clustering, which groups code into functionally cohesive, hierarchical units; and (3) skillful agent-based generation, which queries the graph to create modular, cross-referenced documentation with auto-generated Mermaid diagrams. For incremental maintenance, a semantic impact propagation mechanism navigates the RepoKG bidirectionally to pinpoint all affected parts, allowing selective, targeted regeneration. Evaluated on 24 repositories across 8 programming languages, RepoDoc substantially outperforms state-of-the-art alternatives. It improves API coverage by 32.5% and completeness by 10.4%, while generating documentation 3x faster with 85% fewer tokens. For incremental updates, it cuts update time by 73% and token usage by 77%, and achieves 10.2% higher update recall, more accurately reflecting code changes in the regenerated documentation. The source code and experimental artifacts are available at https://github.com/SYSUSELab/RepoDoc.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-skills|Agent skills]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.26523v1)
