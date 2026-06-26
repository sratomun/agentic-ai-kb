---
type: source
source_type: arxiv
title: "MATA: Multi-Agent Framework for Reliable and Flexible Table Question Answering"
authors: Sieun Hyeon, Jusang Oh, Sunghwan Steve Cho, Jaeyoung Do
url: https://arxiv.org/abs/2602.09642v2
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MATA: Multi-Agent Framework for Reliable and Flexible Table Question Answering

**arXiv:** [2602.09642v2](https://arxiv.org/abs/2602.09642v2) · 2026-02-10 · cs.CL
**Authors:** Sieun Hyeon, Jusang Oh, Sunghwan Steve Cho, Jaeyoung Do

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in Large Language Models (LLMs) have significantly improved table understanding tasks such as Table Question Answering (TableQA), yet challenges remain in ensuring reliability, scalability, and efficiency, especially in resource-constrained or privacy-sensitive environments. In this paper, we introduce MATA, a multi-agent TableQA framework that leverages multiple complementary reasoning paths and a set of tools built with small language models. MATA generates candidate answers through diverse reasoning styles for a given table and question, then refines or selects the optimal answer with the help of these tools. Furthermore, it incorporates an algorithm designed to minimize expensive LLM agent calls, enhancing overall efficiency. MATA maintains strong performance with small, open-source models and adapts easily across various LLM types. Extensive experiments on two benchmarks of varying difficulty with ten different LLMs demonstrate that MATA achieves state-of-the-art accuracy and highly efficient reasoning while avoiding excessive LLM inference. Our results highlight that careful orchestration of multiple reasoning pathways yields scalable and reliable TableQA. The code is available at https://github.com/AIDASLab/MATA.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.09642v2)
