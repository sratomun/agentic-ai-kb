---
type: source
source_type: arxiv
title: "AdapTools: Adaptive Tool-based Indirect Prompt Injection Attacks on Agentic LLMs"
authors: Che Wang, Jiaming Zhang, Ziqi Zhang, Zijie Wang et al.
url: https://arxiv.org/abs/2602.20720v1
date: 2026-02-24
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CR
tags: [agent-security, agent-protocols, arxiv, auto-ingested]
---

# AdapTools: Adaptive Tool-based Indirect Prompt Injection Attacks on Agentic LLMs

**arXiv:** [2602.20720v1](https://arxiv.org/abs/2602.20720v1) · 2026-02-24 · cs.CR
**Authors:** Che Wang, Jiaming Zhang, Ziqi Zhang, Zijie Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The integration of external data services (e.g., Model Context Protocol, MCP) has made large language model-based agents increasingly powerful for complex task execution. However, this advancement introduces critical security vulnerabilities, particularly indirect prompt injection (IPI) attacks. Existing attack methods are limited by their reliance on static patterns and evaluation on simple language models, failing to address the fast-evolving nature of modern AI agents. We introduce AdapTools, a novel adaptive IPI attack framework that selects stealthier attack tools and generates adaptive attack prompts to create a rigorous security evaluation environment. Our approach comprises two key components: (1) Adaptive Attack Strategy Construction, which develops transferable adversarial strategies for prompt optimization, and (2) Attack Enhancement, which identifies stealthy tools capable of circumventing task-relevance defenses. Comprehensive experimental evaluation shows that AdapTools achieves a 2.13 times improvement in attack success rate while degrading system utility by a factor of 1.78. Notably, the framework maintains its effectiveness even against state-of-the-art defense mechanisms. Our method advances the understanding of IPI attacks and provides a useful reference for future research.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.20720v1)
