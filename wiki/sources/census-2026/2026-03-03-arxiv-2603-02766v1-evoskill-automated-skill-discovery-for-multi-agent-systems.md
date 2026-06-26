---
type: source
source_type: arxiv
title: "EvoSkill: Automated Skill Discovery for Multi-Agent Systems"
authors: Salaheddin Alzubi, Noah Provenzano, Jaydon Bingham, Weiyuan Chen et al.
url: https://arxiv.org/abs/2603.02766v1
date: 2026-03-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [coding-agents, self-evolving-agents, agent-skills, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# EvoSkill: Automated Skill Discovery for Multi-Agent Systems

**arXiv:** [2603.02766v1](https://arxiv.org/abs/2603.02766v1) · 2026-03-03 · cs.AI
**Authors:** Salaheddin Alzubi, Noah Provenzano, Jaydon Bingham, Weiyuan Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Coding agents are increasingly used as general-purpose problem solvers, but their flexibility does not by itself confer the domain expertise needed for specialized tasks. Recent work addresses this through \textit{agent skills}: reusable workflows, and code, that augment agents with domain-specific capabilities. Most skills today are hand-crafted, and existing evolutionary approaches optimize low-level artifacts (e.g. prompts \& code) that are tightly coupled to specific models and tasks. We introduce \textbf{EvoSkill}, a self-evolving framework that automatically discovers and refines agent skills through iterative failure analysis. EvoSkill analyzes execution failures, proposes new skills or edits to existing ones, and materializes them into structured, reusable skill folders. A Pareto frontier of agent programs governs selection, retaining only skills that improve held-out validation performance while the underlying model remains frozen. We evaluate EvoSkill on two benchmarks: OfficeQA, a grounded reasoning benchmark over U.S.\ Treasury data, where it improves exact-match accuracy by \textbf{7.3\%} (60.6\% $\to$ 67.9\%); and SealQA, a search-augmented QA benchmark with noisy retrieval, where it yields a \textbf{12.1\%} gain (26.6\% $\to$ 38.7\%). We also investigate the zero-shot transfer capabilties of skills evolved on one task to the other; in particular: skills evolved from SealQA transfers zero-shot to BrowseComp, improving accuracy by \textbf{5.3\%} without modification demonstrating that skill-level optimization produces transferable capabilities beyond the training task.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.02766v1)
