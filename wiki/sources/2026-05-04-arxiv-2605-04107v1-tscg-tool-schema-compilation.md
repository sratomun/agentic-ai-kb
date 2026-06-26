---
type: source
source_type: arxiv
title: "TSCG: Deterministic Tool-Schema Compilation for Agentic LLM Deployments"
authors: Furkan Sakizli
url: https://arxiv.org/abs/2605.04107v1
date: 2026-05-04
ingested: 2026-06-21
depth: full-text
tags: [tool-use, arxiv]
---

# TSCG: Deterministic Tool-Schema Compilation for Agentic LLM Deployments

**Why it matters:** Shows JSON tool schemas are a representation problem, not just a size problem — compiling them to token-efficient text restores small models from near-0% to 80%+ tool accuracy. Practical for cheap-model agent deployments.

## Takeaways
- TSCG deterministically compiles JSON tool schemas into token-efficient structured text at the API boundary — no model access, fine-tuning, or runtime search.
- Restores Phi-4 14B from 0%→84.4% accuracy at 20 tools (90.3% at 50); 52–57% token savings; format-vs-compression decomposition (R²=0.88→0.03) shows representation change is the dominant lever.
- Per-model operator profiles (operator-hungry Opus 4.7, operator-sensitive GPT-5.2, operator-robust Sonnet 4); ships as a zero-dependency TypeScript package.

## Graph
- **Concepts:** [[tool-use|Tool use]]
- **Entities:** [[mcp]] · [[bfcl]]
- **Raw:** `raw/arxiv/2605.04107v1.md` · `raw/arxiv/2605.04107v1.fulltext.md`
