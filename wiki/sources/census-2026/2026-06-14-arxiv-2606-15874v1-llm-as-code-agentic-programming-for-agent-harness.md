---
type: source
source_type: arxiv
title: "LLM-as-Code Agentic Programming for Agent Harness"
authors: Junjia Qi, Zichuan Fu, Jingtong Gao, Wenlin Zhang et al.
url: https://arxiv.org/abs/2606.15874v1
date: 2026-06-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [coding-agents, computer-use-agents, agent-reliability, multi-agent-systems, arxiv, auto-ingested]
---

# LLM-as-Code Agentic Programming for Agent Harness

**arXiv:** [2606.15874v1](https://arxiv.org/abs/2606.15874v1) · 2026-06-14 · cs.AI
**Authors:** Junjia Qi, Zichuan Fu, Jingtong Gao, Wenlin Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Every major LLM agent framework gives the LLM the role of orchestrator; the model decides what to do next, when to call tools, and when to stop. We argue that token explosion, control-flow hallucination, and unreliable completion are not implementation bugs but architectural consequences of assigning the deterministic work of looping, branching, and sequencing to a probabilistic system. A better prompt or a stronger model cannot guarantee the reliability of the LLM agent. We therefore propose Agentic Programming, in which the program governs all control flow, and the LLM is itself part of it, an adaptive component we call LLM-as-Code and invoke only where a task calls for reasoning or generation. Within each call the model keeps full flexibility, but it cannot alter the program's execution path. With control in the program, the LLM's context is built from the execution history's call tree and forms a directed acyclic graph (DAG). Each call's context length is then determined by its call depth rather than by accumulation over steps. A case study of computer-use agents shows that the design is practical, not just a theoretical stance, substantially improving the stability of long visual operation sequences.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.15874v1)
