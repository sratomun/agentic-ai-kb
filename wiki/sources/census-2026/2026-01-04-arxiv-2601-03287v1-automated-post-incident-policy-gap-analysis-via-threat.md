---
type: source
source_type: arxiv
title: "Automated Post-Incident Policy Gap Analysis via Threat-Informed Evidence Mapping using Large Language Models"
authors: Huan Lin Oh, Jay Yong Jun Jie, Mandy Lee Ling Siu, Jonathan Pan
url: https://arxiv.org/abs/2601.03287v1
date: 2026-01-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CR
tags: [recommendation-agents, human-agent-interaction, agent-security, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# Automated Post-Incident Policy Gap Analysis via Threat-Informed Evidence Mapping using Large Language Models

**arXiv:** [2601.03287v1](https://arxiv.org/abs/2601.03287v1) · 2026-01-04 · cs.CR
**Authors:** Huan Lin Oh, Jay Yong Jun Jie, Mandy Lee Ling Siu, Jonathan Pan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Cybersecurity post-incident reviews are essential for identifying control failures and improving organisational resilience, yet they remain labour-intensive, time-consuming, and heavily reliant on expert judgment. This paper investigates whether Large Language Models (LLMs) can augment post-incident review workflows by autonomously analysing system evidence and identifying security policy gaps. We present a threat-informed, agentic framework that ingests log data, maps observed behaviours to the MITRE ATT&CK framework, and evaluates organisational security policies for adequacy and compliance. Using a simulated brute-force attack scenario against a Windows OpenSSH service (MITRE ATT&CK T1110), the system leverages GPT-4o for reasoning, LangGraph for multi-agent workflow orchestration, and LlamaIndex for traceable policy retrieval. Experimental results indicate that the LLM-based pipeline can interpret log-derived evidence, identify insufficient or missing policy controls, and generate actionable remediation recommendations with explicit evidence-to-policy traceability. Unlike prior work that treats log analysis and policy validation as isolated tasks, this study integrates both into a unified end-to-end proof-of-concept post-incident review framework. The findings suggest that LLM-assisted analysis has the potential to improve the efficiency, consistency, and auditability of post-incident evaluations, while highlighting the continued need for human oversight in high-stakes cybersecurity decision-making.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Entities:** [[gpt-5]] · [[llama]] · [[langgraph]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.03287v1)
