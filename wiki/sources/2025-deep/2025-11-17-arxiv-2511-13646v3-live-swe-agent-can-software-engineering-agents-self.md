---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Live-SWE-agent: Can Software Engineering Agents Self-Evolve on the Fly?"
authors: Chunqiu Steven Xia, Zhe Wang, Yan Yang, Yuxiang Wei et al.
url: https://arxiv.org/abs/2511.13646v3
date: 2025-11-17
citationCount: 51
influentialCitationCount: 8
velocity: 7.15
ingested: 2026-06-22
tags: [coding-agents, self-evolving-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Live-SWE-agent: Can Software Engineering Agents Self-Evolve on the Fly?

**arXiv [2511.13646v3](https://arxiv.org/abs/2511.13646v3)** · 2025-11-17 · **51 citations** (8 influential · 7.15/mo) · Chunqiu Steven Xia, Zhe Wang, Yan Yang, Yuxiang Wei et al.

## Abstract
Large Language Models (LLMs) are reshaping almost all industries, including software engineering. In recent years, a number of LLM agents have been proposed to solve real-world software problems. Such software agents are typically equipped with a suite of coding tools and can autonomously decide the next actions to form complete trajectories to solve end-to-end software tasks. While promising, they typically require dedicated design and may still be suboptimal, since it can be extremely challenging and costly to exhaust the entire agent scaffold design space. Recognizing that software agents are inherently software themselves that can be further refined/modified, researchers have proposed a number of self-improving software agents recently, including the Darwin-Gödel Machine (DGM). Meanwhile, such self-improving agents require costly offline training on specific benchmarks and may not generalize well across different LLMs or benchmarks. In this paper, we propose Live-SWE-agent, the first live software agent that can autonomously and continuously evolve itself on-the-fly during runtime when solving real-world software problems. More specifically, Live-SWE-agent starts with the most basic agent scaffold with only access to bash tools (e.g., mini-SWE-agent), and autonomously evolves its own scaffold implementation while solving real-world software problems. Our evaluation on the widely studied SWE-bench Verified benchmark shows that LIVE-SWE-AGENT can achieve an impressive solve rate of 77.4% without test-time scaling, outperforming all existing software agents, including the best proprietary solution. Moreover, Live-SWE-agent outperforms state-of-the-art manually crafted software agents on the recent SWE-Bench Pro benchmark, achieving the best-known solve rate of 45.8%.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Approach 2.1 On-the-fly Self Evolution 2.2 Custom Tool Synthesis 3 Experimental Setup 4 Evaluation 4.1 Main Results 4.2 Tools Analysis 4.3 Ablation 4.4 Discussion and Future Work 5 Related Work 5.1 Software Engineering Agents 5.2 Benchmarks for Software Engineering Agents 6 Conclusion A Additional experimental settings B Additional tool analysis C Ablation problems C.1 SWE-bench Verified ablation subset C.2 SWE-bench Multilingual ablation subset D Prompts Used D.1 Initial prompt D.2 Feedback message Live-SWE-agent : Can Software Engineering Agents Self-Evolve on the Fly? Chunqiu Steven Xia Zhe Wang Yan Yang † Yuxiang Wei Lingming Zhang University of Illinois Urbana-Champaign {chunqiu2, zhe36, ywei40, lingming}@illinois.edu † yanyang826@outlook.com Abstract Large Language Models (LLMs) are reshaping almost all industries, including software engineering. In recent years, a number of LLM agents have been proposed to solve real-world software problems. Such software agents are typically equi…

**Method / approach.** methods. Notably, compared to existing self-improving agents, we achieve much better performance (65.0% solve rate on the SWE-bench Verified-60 subset vs. DGM’s 53.3%) while being significantly less costly (no offline cost). • Unified leaderboard. For software tasks, recent LLMs are often benchmarked using manually engineered, proprietary agent scaffolds, making fair model comparison hard. Live-SWE-agent offers an open, unified, and powerful scaffold that enables genuinely fair, apples-to-apples comparison for future model releases. We are maintaining a leaderboard of recent models evaluated on real-world software tasks using Live-SWE-agent at: http://live-swe-agent.github.io 2 Approach Figure 2 : Overview of Live-SWE-agent Live-SWE-agent is a live, self-evolving agent that improves and expands its capabilities on the fly while solving an issue. Our key insight is recognizing that agents themselves can be iteratively improved, just like the software issues they are d…

**Results.** Experimental Setup 4 Evaluation 4.1 Main Results 4.2 Tools Analysis 4.3 Ablation 4.4 Discussion and Future Work 5 Related Work 5.1 Software Engineering Agents 5.2 Benchmarks for Software Engineering Agents 6 Conclusion A Additional experimental settings B Additional tool analysis C Ablation problems C.1 SWE-bench Verified ablation subset C.2 SWE-bench Multilingual ablation subset D Prompts Used D.1 Initial prompt D.2 Feedback message Live-SWE-agent : Can Software Engineering Agents Self-Evolve on the Fly? Chunqiu Steven Xia Zhe Wang Yan Yang † Yuxiang Wei Lingming Zhang University of Illinois Urbana-Champaign {chunqiu2, zhe36, ywei40, lingming}@illinois.edu † yanyang826@outlook.com Abstract Large Language Models (LLMs) are reshaping almost all industries, including software engineering. In recent years, a number of LLM agents have been proposed to solve real-world sof…

**Conclusion.** Conclusion A Additional experimental settings B Additional tool analysis C Ablation problems C.1 SWE-bench Verified ablation subset C.2 SWE-bench Multilingual ablation subset D Prompts Used D.1 Initial prompt D.2 Feedback message Live-SWE-agent : Can Software Engineering Agents Self-Evolve on the Fly? Chunqiu Steven Xia Zhe Wang Yan Yang † Yuxiang Wei Lingming Zhang University of Illinois Urbana-Champaign {chunqiu2, zhe36, ywei40, lingming}@illinois.edu † yanyang826@outlook.com Abstract Large Language Models (LLMs) are reshaping almost all industries, including software engineering. In recent years, a number of LLM agents have been proposed to solve real-world software problems. Such software agen…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2511.13646v3.md` · `raw/arxiv/2511.13646v3.fulltext.md`
