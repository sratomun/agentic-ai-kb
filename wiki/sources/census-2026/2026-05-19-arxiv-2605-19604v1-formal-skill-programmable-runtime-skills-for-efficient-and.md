---
type: source
source_type: arxiv
title: "Formal Skill: Programmable Runtime Skills for Efficient and Accurate LLM Agents"
authors: Xi Zhang, Meijun Gao, Yuntian Zhao, Xinyu Tan et al.
url: https://arxiv.org/abs/2605.19604v1
date: 2026-05-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agent-protocols, agent-skills, tool-use, arxiv, auto-ingested]
---

# Formal Skill: Programmable Runtime Skills for Efficient and Accurate LLM Agents

**arXiv:** [2605.19604v1](https://arxiv.org/abs/2605.19604v1) · 2026-05-19 · cs.AI
**Authors:** Xi Zhang, Meijun Gao, Yuntian Zhao, Xinyu Tan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM) agents increasingly act inside real workspaces, where tools and skills determine whether model reasoning becomes reliable action. Existing skills remain largely informal: Markdown skills and instruction packs encode procedures as long natural-language documents, while function calling, Model Context Protocol (MCP) servers, and framework tools structure individual actions but usually leave workflow state, policy enforcement, and completion discipline outside the skill itself. We introduce Formal Skill, a runtime-native abstraction that represents reusable capability with JSON metadata and action schemas, reliable Python executors, hook-governed control logic, Formal Skill routing, and skill-local runtime state. By moving reusable procedure from repeated prompt text into executable state machines and hook policies, Formal Skill gives agents a token-efficient and enforceable control surface. We implement the abstraction in FairyClaw, an open-source event-driven runtime for executable, observable, and composable Formal Skills. On Harness-Bench, FairyClaw obtains highly competitive average scores while using substantially fewer tokens, with especially strong results on tasks that expose the role of Formal Skill.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.19604v1)
