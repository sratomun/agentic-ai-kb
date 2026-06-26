---
type: source
source_type: arxiv
title: "PHMForge: Evaluating LLM Agents on Industrial Prognostics through MCP-Native, Algorithm-Grounded Tools"
authors: Tianjun Feng, Yunfeng Chen, Chun-Yi Tsai, Yihan Sun et al.
url: https://arxiv.org/abs/2604.01532v2
date: 2026-04-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 34
primary: cs.AI
tags: [agent-reliability, agent-security, agent-protocols, agentic-rag, tool-use, arxiv, auto-ingested]
---

# PHMForge: Evaluating LLM Agents on Industrial Prognostics through MCP-Native, Algorithm-Grounded Tools

**arXiv:** [2604.01532v2](https://arxiv.org/abs/2604.01532v2) · 2026-04-02 · cs.AI
**Authors:** Tianjun Feng, Yunfeng Chen, Chun-Yi Tsai, Yihan Sun et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM agents are beginning to invoke industrial asset-management tools through the Model Context Protocol (MCP), yet whether they can act reliably on this substrate for safety-critical \emph{Prognostics and Health Management (PHM)} is unanswered. Prior benchmarks conflate protocol fluency with reasoning, instrumentation failures with agent failures, and tool use with tool retrieval. We introduce \textbf{PHMForge}, an evaluation environment that closes each conflation. PHMForge ships 99 SME-authored scenarios across eight industrial asset classes spanning rotating equipment, aero-engines, and lithium-ion cells, on public datasets including NASA PCoE, served through 39 MCP-native tools wrapping published PHM algorithms (C-MAPSS, ISO~10816, Arrhenius capacity-fade models, time-series foundation models). Krippendorff's $α\in [0.74,\,0.82]$ on a 30-scenario stratified rotating-equipment/aero-engine sample; the battery extension is single-rater. Across three agentic frameworks and six LLM backbones, the strongest configuration reaches \textbf{80.8\% pass@1}, with the residual gap concentrated in orchestration and tool-sequencing errors. Crucially, an architectural ablation shows that replacing MCP execution with text-based Retrieval-Augmented Generation (RAG) over telemetry-equivalent evidence collapses Remaining Useful Life \emph{pass-all-3} from \textbf{100\% to 20\%} (5/5 vs.\ 1/5) on the battery class, exposing the structural limits of static retrieval for prognostic computation. Trajectory decomposition shows orchestration errors dominate failures across backbones, while schema-invalid tool calls concentrate in smaller open-weight models. Frontier LLMs are stronger at calling tools than at planning when to call them. PHMForge is open-sourced with deterministic evaluators, a public leaderboard, and a datasheet.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.01532v2)
