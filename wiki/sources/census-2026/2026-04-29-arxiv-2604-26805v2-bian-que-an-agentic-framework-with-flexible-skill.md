---
type: source
source_type: arxiv
title: "Bian Que: An Agentic Framework with Flexible Skill Arrangement for Online System Operations"
authors: Bochao Liu, Zhipeng Qian, Yang Zhao, Xinyuan Jiang et al.
url: https://arxiv.org/abs/2604.26805v2
date: 2026-04-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [recommendation-agents, self-evolving-agents, agent-skills, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Bian Que: An Agentic Framework with Flexible Skill Arrangement for Online System Operations

**arXiv:** [2604.26805v2](https://arxiv.org/abs/2604.26805v2) · 2026-04-29 · cs.AI
**Authors:** Bochao Liu, Zhipeng Qian, Yang Zhao, Xinyuan Jiang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Operating and maintaining (O&M) large-scale online engine systems (eg, search, recommendation and advertising) demands substantial human effort for release monitoring, alert response, and root cause analysis. Despite the inherent suitability of LLM-based agents for such operational scenarios, the critical bottleneck impeding their practical deployment lies not in reasoning, but in orchestration capability - specifically, the precise selection of relevant data (encompassing metrics, logs, and change events) and applicable knowledge (including handbook-defined rules and empirically derived practitioner experience) tailored to each individual operational event. Feeding all signals indiscriminately causes dilution and hallucination, while manually curating the event-to-(data, knowledge) mapping is intractable under dozens of daily releases. Here we present Bian Que, an agentic operating framework with three contributions: (i) The unified operational paradigm, which abstracts routine daily O&M actions into three canonical patterns: release interception, proactive inspection, and alert root cause analysis; (ii) The flexible Skill Arrangement, each predefined Skill explicitly defines the requisite data and operational knowledge for each specific context. Such Skills can be automatically generated and updated by LLM agents, and can also be iteratively optimized by on-call engineers via natural language instructions. (iii) The unified self-evolving mechanism, where each correction signal enables two parallel evolutionary pathways: distilling event memory into knowledge, and targeted refinement of Skills. Deployed on the e-commerce search engine of KuaiShou, Bian Que reduces alert volume by 75%, achieves 80% root-cause analysis accuracy, cuts mean time to resolution by over 50%, and attains a 99.0% pass rate on offline evaluations. Codes are at https://github.com/benchen4395/BianQue_Assistant.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.26805v2)
