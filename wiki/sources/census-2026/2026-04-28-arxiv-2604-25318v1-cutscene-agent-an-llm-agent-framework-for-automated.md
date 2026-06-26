---
type: source
source_type: arxiv
title: "Cutscene Agent: An LLM Agent Framework for Automated 3D Cutscene Generation"
authors: Lanshan He, Haozhou Pang, Qi Gan, Xin Shen et al.
url: https://arxiv.org/abs/2604.25318v1
date: 2026-04-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 26
primary: cs.GR
tags: [agent-protocols, agent-memory, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Cutscene Agent: An LLM Agent Framework for Automated 3D Cutscene Generation

**arXiv:** [2604.25318v1](https://arxiv.org/abs/2604.25318v1) · 2026-04-28 · cs.GR
**Authors:** Lanshan He, Haozhou Pang, Qi Gan, Xin Shen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Cutscenes are carefully choreographed cinematic sequences embedded in video games and interactive media, serving as the primary vehicle for narrative delivery, character development, and emotional engagement. Producing cutscenes is inherently complex: it demands seamless coordination across screenwriting, cinematography, character animation, voice acting, and technical direction, often requiring days to weeks of collaborative effort from multidisciplinary teams to produce minutes of polished content. In this work, we present Cutscene Agent, an LLM agent framework for automated end-to-end cutscene generation. The framework makes three contributions: (1)~a Cutscene Toolkit built on the Model Context Protocol (MCP) that establishes \emph{bidirectional} integration between LLM agents and the game engine -- agents not only invoke engine operations but continuously observe real-time scene state, enabling closed-loop generation of editable engine-native cinematic assets; (2)~a multi-agent system where a director agent orchestrates specialist subagents for animation, cinematography, and sound design, augmented by a visual reasoning feedback loop for perception-driven refinement; and (3)~CutsceneBench, a hierarchical evaluation benchmark for cutscene generation. Unlike typical tool-use benchmarks that evaluate short, isolated function calls, cutscene generation requires long-horizon, multi-step orchestration of dozens of interdependent tool invocations with strict ordering constraints -- a capability dimension that existing benchmarks do not cover. We evaluate a range of LLMs on CutsceneBench and analyze their performance across this challenging task.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.25318v1)
