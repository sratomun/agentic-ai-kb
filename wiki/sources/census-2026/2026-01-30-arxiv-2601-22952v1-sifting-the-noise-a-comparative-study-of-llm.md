---
type: source
source_type: arxiv
title: "Sifting the Noise: A Comparative Study of LLM Agents in Vulnerability False Positive Filtering"
authors: Yunpeng Xiong, Ting Zhang
url: https://arxiv.org/abs/2601.22952v1
date: 2026-01-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.SE
tags: [agent-security, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Sifting the Noise: A Comparative Study of LLM Agents in Vulnerability False Positive Filtering

**arXiv:** [2601.22952v1](https://arxiv.org/abs/2601.22952v1) · 2026-01-30 · cs.SE
**Authors:** Yunpeng Xiong, Ting Zhang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Static Application Security Testing (SAST) tools are essential for identifying software vulnerabilities, but they often produce a high volume of false positives (FPs), imposing a substantial manual triage burden on developers. Recent advances in Large Language Model (LLM) agents offer a promising direction by enabling iterative reasoning, tool use, and environment interaction to refine SAST alerts. However, the comparative effectiveness of different LLM-based agent architectures for FP filtering remains poorly understood. In this paper, we present a comparative study of three state-of-the-art LLM-based agent frameworks, i.e., Aider, OpenHands, and SWE-agent, for vulnerability FP filtering. We evaluate these frameworks using the vulnerabilities from the OWASP Benchmark and real-world open-source Java projects. The experimental results show that LLM-based agents can remove the majority of SAST noise, reducing an initial FP detection rate of over 92% on the OWASP Benchmark to as low as 6.3% in the best configuration. On real-world dataset, the best configuration of LLM-based agents can achieve an FP identification rate of up to 93.3% involving CodeQL alerts. However, the benefits of agents are strongly backbone- and CWE-dependent: agentic frameworks significantly outperform vanilla prompting for stronger models such as Claude Sonnet 4 and GPT-5, but yield limited or inconsistent gains for weaker backbones. Moreover, aggressive FP reduction can come at the cost of suppressing true vulnerabilities, highlighting important trade-offs. Finally, we observe large disparities in computational cost across agent frameworks. Overall, our study demonstrates that LLM-based agents are a powerful but non-uniform solution for SAST FP filtering, and that their practical deployment requires careful consideration of agent design, backbone model choice, vulnerability category, and operational cost.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]] · [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.22952v1)
