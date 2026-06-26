---
type: source
source_type: arxiv
title: "Interpretable Context Methodology: Folder Structure as Agentic Architecture"
authors: Jake Van Clief, David McDermott
url: https://arxiv.org/abs/2603.16021v2
date: 2026-03-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-protocols, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Interpretable Context Methodology: Folder Structure as Agentic Architecture

**arXiv:** [2603.16021v2](https://arxiv.org/abs/2603.16021v2) · 2026-03-17 · cs.AI
**Authors:** Jake Van Clief, David McDermott

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current approaches to AI agent orchestration typically involve building multi-agent frameworks that manage context passing, memory, error handling, and step coordination through code. These frameworks work well for complex, concurrent systems. But for sequential workflows where a human reviews output at each step, they introduce engineering overhead that the problem does not require. This paper presents Model Workspace Protocol (MWP), a method that replaces framework-level orchestration with filesystem structure. Numbered folders represent stages. Plain markdown files carry the prompts and context that tell a single AI agent what role to play at each step. Local scripts handle the mechanical work that does not need AI at all. The result is a system where one agent, reading the right files at the right moment, does the work that would otherwise require a multi-agent framework. This approach applies ideas from Unix pipeline design, modular decomposition, multi-pass compilation, and literate programming to the specific problem of structuring context for AI agents. The protocol is open source under the MIT license.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.16021v2)
