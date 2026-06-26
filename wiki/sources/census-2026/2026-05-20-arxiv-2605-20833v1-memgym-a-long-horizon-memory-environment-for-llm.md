---
type: source
source_type: arxiv
title: "MemGym: a Long-Horizon Memory Environment for LLM Agents"
authors: Wujiang Xu, Yu Wang, Kai Mei, Kaiqu Liang et al.
url: https://arxiv.org/abs/2605.20833v1
date: 2026-05-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [computer-use-agents, embodied-agents, agentic-rl, agent-memory, tool-use, arxiv, auto-ingested]
---

# MemGym: a Long-Horizon Memory Environment for LLM Agents

**arXiv:** [2605.20833v1](https://arxiv.org/abs/2605.20833v1) · 2026-05-20 · cs.CL
**Authors:** Wujiang Xu, Yu Wang, Kai Mei, Kaiqu Liang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Memory is a central capability for LLM agents operating across long-horizon tasks. Existing memory benchmarks predominantly evaluate retention of personalized information in multi-turn chat scenarios, overlooking the dynamic memory formation that occurs during extended agent execution. Consequently, the memory systems they produce transfer poorly to realistic agentic environments, such as coding and web navigation. We present MemGym, a benchmark for agentic memory that unifies existing agent gyms and in-house memory-grounded pipelines behind one memory-reasoning interface. MemGym spans five evaluation tracks grouped into four agentic regimes: tool-use dialogue (tau2-bench), multi-turn deep-research search (MEMGYM-DR), coding (SWE-Gym and MEMGYM-CODEQA), and computer use (WebArena-Infinity). MemGym reports memory-isolated scores that decouple memory performance from reasoning, retrieval, and tool-use ability, so memory strategies can be ranked without those confounders. Our synthetic pipelines for MEMGYM-CODEQA and MEMGYM-DR are length-controllable, ablation-verified at every stage, and tightly aligned with downstream scenarios. To make evaluation on coding environments academically tractable, we train MemRM, a lightweight reward model (Qwen3-1.7B fine-tuned with QLoRA) that scores compression quality as a fast scalar read in place of full Docker rollouts.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]] · [[webarena]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.20833v1)
