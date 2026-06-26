---
type: source
source_type: arxiv
title: "AgentWebBench: Benchmarking Multi-Agent Coordination in Agentic Web"
authors: Shanshan Zhong, Kate Shen, Chenyan Xiong
url: https://arxiv.org/abs/2604.10938v1
date: 2026-04-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.MA
tags: [recommendation-agents, agent-economies, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AgentWebBench: Benchmarking Multi-Agent Coordination in Agentic Web

**arXiv:** [2604.10938v1](https://arxiv.org/abs/2604.10938v1) · 2026-04-13 · cs.MA
**Authors:** Shanshan Zhong, Kate Shen, Chenyan Xiong

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic Web is an emerging paradigm where autonomous agents help users use online information. As the paradigm develops, content providers are also deploying agents to manage their data and serve it through controlled interfaces. This shift moves information access from centralized retrieval to decentralized coordination. To study this setting, we introduce AgentWebBench, a benchmark that evaluates how well a user agent synthesizes answers by interacting with website-specific content agents. We evaluate four tasks that cover common web information needs, spanning ranked retrieval (web search, web recommendation) and open-ended synthesis (question answering, deep research). Across seven advanced LLMs and three coordination strategies, multi-agent coordination generally lags behind centralized retrieval as expected, because user agent cannot directly access the corpus, but the gap shrinks with model scale and can even outperform centralized retrieval on question answering. This benchmark also enables us to study properties of the emerging paradigm of the digital world. We find that decentralized access concentrates traffic toward a small set of websites, test time scaling improves both interaction reliability and task performance, and strong results require sufficient interactions guided by careful planning. Finally, our failure analysis suggests that user agents need better planning and answer synthesis, while content agents need more reliable retrieval and evidence quality. Code, data, and APIs are released on https://github.com/cxcscmu/AgentWebBench.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agent-economies|Agent economies]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.10938v1)
