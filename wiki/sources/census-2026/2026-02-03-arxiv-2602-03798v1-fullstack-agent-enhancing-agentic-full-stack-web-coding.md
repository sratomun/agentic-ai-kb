---
type: source
source_type: arxiv
title: "FullStack-Agent: Enhancing Agentic Full-Stack Web Coding via Development-Oriented Testing and Repository Back-Translation"
authors: Zimu Lu, Houxing Ren, Yunqiao Yang, Ke Wang et al.
url: https://arxiv.org/abs/2602.03798v1
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.SE
tags: [coding-agents, embodied-agents, self-evolving-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# FullStack-Agent: Enhancing Agentic Full-Stack Web Coding via Development-Oriented Testing and Repository Back-Translation

**arXiv:** [2602.03798v1](https://arxiv.org/abs/2602.03798v1) · 2026-02-03 · cs.SE
**Authors:** Zimu Lu, Houxing Ren, Yunqiao Yang, Ke Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Assisting non-expert users to develop complex interactive websites has become a popular task for LLM-powered code agents. However, existing code agents tend to only generate frontend web pages, masking the lack of real full-stack data processing and storage with fancy visual effects. Notably, constructing production-level full-stack web applications is far more challenging than only generating frontend web pages, demanding careful control of data flow, comprehensive understanding of constantly updating packages and dependencies, and accurate localization of obscure bugs in the codebase. To address these difficulties, we introduce FullStack-Agent, a unified agent system for full-stack agentic coding that consists of three parts: (1) FullStack-Dev, a multi-agent framework with strong planning, code editing, codebase navigation, and bug localization abilities. (2) FullStack-Learn, an innovative data-scaling and self-improving method that back-translates crawled and synthesized website repositories to improve the backbone LLM of FullStack-Dev. (3) FullStack-Bench, a comprehensive benchmark that systematically tests the frontend, backend and database functionalities of the generated website. Our FullStack-Dev outperforms the previous state-of-the-art method by 8.7%, 38.2%, and 15.9% on the frontend, backend, and database test cases respectively. Additionally, FullStack-Learn raises the performance of a 30B model by 9.7%, 9.5%, and 2.8% on the three sets of test cases through self-improvement, demonstrating the effectiveness of our approach. The code is released at https://github.com/mnluzimu/FullStack-Agent.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[embodied-agents|Embodied agents]] · [[self-evolving-agents|Self-evolving agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03798v1)
