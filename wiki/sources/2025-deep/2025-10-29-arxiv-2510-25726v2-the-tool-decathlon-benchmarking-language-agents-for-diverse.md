---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The Tool Decathlon: Benchmarking Language Agents for Diverse, Realistic, and Long-Horizon Task Execution"
authors: Junlong Li, Wenshuo Zhao, Jian Zhao, Weihao Zeng et al.
url: https://arxiv.org/abs/2510.25726v2
date: 2025-10-29
citationCount: 42
influentialCitationCount: 4
velocity: 5.42
ingested: 2026-06-22
tags: [finance-agents, agent-reliability, agent-protocols, agent-memory, tool-use, arxiv, 2025, cited]
---

# The Tool Decathlon: Benchmarking Language Agents for Diverse, Realistic, and Long-Horizon Task Execution

**arXiv [2510.25726v2](https://arxiv.org/abs/2510.25726v2)** · 2025-10-29 · **42 citations** (4 influential · 5.42/mo) · Junlong Li, Wenshuo Zhao, Jian Zhao, Weihao Zeng et al.

## Abstract
Real-world language agents must handle complex, multi-step workflows across diverse Apps. For instance, an agent may manage emails by coordinating with calendars and file systems, or monitor a production database to detect anomalies and generate reports following an operating manual. However, existing language agent benchmarks often focus on narrow domains or simplified tasks that lack the diversity, realism, and long-horizon complexity required to evaluate agents' real-world performance. To address this gap, we introduce the Tool Decathlon (dubbed as Toolathlon), a benchmark for language agents offering diverse Apps and tools, realistic environment setup, and reliable execution-based evaluation. Toolathlon spans 32 software applications and 604 tools, ranging from everyday platforms such as Google Calendar and Notion to professional ones like WooCommerce, Kubernetes, and BigQuery. Most of the tools are based on a high-quality set of Model Context Protocol (MCP) servers that we may have revised or implemented ourselves. Unlike prior works, which primarily ensure functional realism but offer limited environment state diversity, we provide realistic initial environment states from real software, such as Canvas courses with dozens of students or real financial spreadsheets. This benchmark includes 108 manually sourced or crafted tasks in total, requiring interacting with multiple Apps over around 20 turns on average to complete. Each task is strictly verifiable through dedicated evaluation scripts. Comprehensive evaluation of SOTA models highlights their significant shortcomings: the best-performing model, Claude-4.5-Sonnet, achieves only a 38.6% success rate with 20.2 tool calling turns on average, while the top open-weights model DeepSeek-V3.2-Exp reaches 20.1%. We expect Toolathlon to drive the development of more capable language agents for real-world, long-horizon task execution.

## From the paper (full-text excerpts)
**Method / approach.** approaches drastically reduce realism and fail to reflect the complexity of real software environments. In contrast, in T OOLATHLON we leverage both remote environments and locally containerized, open-source applications. Specifically, we deploy the open-source Poste.io for email management, Canvas for course administration, Kubernetes for cluster orchestration, and WooCommerce for e-commerce management. By hosting these realistic applications locally within containers, we can efficiently set up dozens of accounts and initialize complex environment states during evaluation. Compared with existing dedicated agent sandboxes such as SWE-Bench (Jimenez et al., 2024), our environments are more diverse and encompass a wider range of software. Agent Framework: We implement a simple agent framework based on the OpenAI Agents SDK (v0.0.15) 1 to conduct the agent action loop – at each turn, the model is expected to (optionally) reason explicitly and make tool calls. We make several enhancements…

**Results.** experiments on T OOLATHLON, the best-performing models, Claude-4.5-Sonnet, achieve only 38.6% accuracy, highlighting the unique challenges posed by T OOLATHLON. DeepSeek-V3.2-Exp (DeepSeek-AI, 2025) achieves 20.1% success rate as the best performer among open-source models. Further analysis reveals that weaknesses in long-context modeling and robust tool calling error tracking are major challenges for all evaluated models. We have fully open-sourced the benchmark and the T OOLATHLON environment, aiming for T OOLATHLON to accelerate the development of practical language agents. 2 T HE T OOLATHLON E NVIRONMENT AND E VALUATION F RAMEWORK 2.1 TASK D EFINITION Each task in T OOLATHLON can be formulated as a partially observable Markov decision process (POMDP) (S, A, O, T , R, U) with state space S, action space A, observation space O, transition function T : S × A → S × O, reward function R : S → [0, 1], and instruction space U. The env…

**Conclusion.** discussion of these related works is in §6. Benchmark # Tasks # Apps Avg # Turns Real Env States Init Verifiable Execution Cross-App Task Realistic Fuzzy Prompt τ -Bench BFCLv3-MT ACEBench AppWorld MCPWorld MCP-RADAR MCPEval LiveMCPBench MCP-AgentBench LiveMCP-101 MCPAtlas MCPUniverse MCPMark GAIA2 165 800 2000 750 201 507 676 95 600 101 1000 231 127 800 2 – – 9 10 6 19 70 33 41 40+ 11 5 12 – 3.8 1.7 – – – – 5.6 – 5.4 3-6 7.5 18.5 22.5 × × × ✓ ✓ ✓ ✓ ✓ ✓ ✓ ✓ ✓ ✓ × ✓ ✓ Partial∗ ✓ ✓ ✓ × Partial∗ × × ✓ × ✓ ✓ ✓ ✓ ✓ ✓ ✓ ✓ × × × × × ✓ ✓ ✓ × ✓ × ✓ × × ✓ ✓ ✓ ✓ ✓ Partial∗ × ✓ × × × × × × × × × × × × × ✓ T OOLATHLON 108 32 26.8 ✓ ✓ ✓ ✓ ✓ verifiable tasks (Mo et al., 2025; Yin et al., 2025), while others cover few domains or…

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]] · [[claude]] · [[deepseek]]
- **Raw:** `raw/arxiv/2510.25726v2.md` · `raw/arxiv/2510.25726v2.fulltext.md`
