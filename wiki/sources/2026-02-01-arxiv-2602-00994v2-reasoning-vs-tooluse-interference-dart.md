---
type: source
source_type: arxiv
title: "Reasoning and Tool-use Compete in Agentic RL:From Quantifying Interference to Disentangled Tuning"
authors: Yu Li, Mingyang Yi, Xiuyu Li, Ju Fan et al.
url: https://arxiv.org/abs/2602.00994v2
date: 2026-02-01
ingested: 2026-06-21
depth: full-text
tags: [agentic-rl, tool-use, arxiv]
---

# Reasoning and Tool-use Compete in Agentic RL:From Quantifying Interference to Disentangled Tuning

**Why it matters:** Empirically challenges a core Agentic-RL assumption: jointly training reasoning and tool-use in one parameter set causes gradient interference. DART decouples them with separate LoRA modules and beats joint baselines.

## Takeaways
- Capability Effect Attribution (CEA) shows reasoning and tool-use induce misaligned gradients → joint optimization interferes.
- [[dart|DART]] decouples parameter updates via separate low-rank adaptation modules for reasoning vs action.
- Outperforms all joint-optimization baselines and approaches the 2-Agent upper bound across 13 RAG-QA and NL2SQL benchmarks.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[dart]]
- **Raw:** `raw/arxiv/2602.00994v2.md` · `raw/arxiv/2602.00994v2.fulltext.md`
