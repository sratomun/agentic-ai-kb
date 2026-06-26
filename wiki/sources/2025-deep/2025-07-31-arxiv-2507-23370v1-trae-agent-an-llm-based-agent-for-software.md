---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Trae Agent: An LLM-based Agent for Software Engineering with Test-time Scaling"
authors: Trae Research Team, Pengfei Gao, Zhao Tian, Xiangxin Meng et al.
url: https://arxiv.org/abs/2507.23370v1
date: 2025-07-31
citationCount: 80
influentialCitationCount: 15
velocity: 7.47
ingested: 2026-06-22
tags: [coding-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Trae Agent: An LLM-based Agent for Software Engineering with Test-time Scaling

**arXiv [2507.23370v1](https://arxiv.org/abs/2507.23370v1)** · 2025-07-31 · **80 citations** (15 influential · 7.47/mo) · Trae Research Team, Pengfei Gao, Zhao Tian, Xiangxin Meng et al.

## Abstract
Software issue resolution is a critical challenge in software engineering and has garnered increasing attention in recent years. With the rapid advancement of large language models (LLMs), substantial progress has been made in addressing real-world software engineering tasks. Recent studies have introduced ensemble reasoning techniques to enhance the performance of LLM-based issue resolution. However, existing prompting-based methods still face limitations in effectively exploring large ensemble spaces and lack the capacity for repository-level understanding, both of which constrain their overall effectiveness. In this paper, we propose Trae Agent, the first agent-based ensemble reasoning approach for repository-level issue resolution. Trae Agent formulates our goal as an optimal solution search problem and addresses two key challenges, i.e., large ensemble spaces and repository-level understanding, through modular agents for generation, pruning, and selection. We conduct extensive experiments using three leading LLMs on the widely-adopted SWE-bench benchmark, comparing Trae Agent against four state-of-the-art ensemble reasoning techniques. Experimental results demonstrate that Trae Agent consistently achieves superior performance, with an average improvement of 10.22% over all baselines in terms of Pass@1. Trae Agent has achieved first place on the SWE-bench Verified leaderboard, with a notable Pass@1 score of 75.20%. We are pleased to release Trae Agent as an open-source project to support the research community, with all resources available at https://github.com/bytedance/trae-agent.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Motivation 3 Approach 3.1 Overview 3.2 Patch Generation 3.3 Patch Pruning 3.4 Patch Selection 4 Evaluation Design 4.1 Benchmarks 4.2 Metrics 4.3 Compared Techniques 4.4 Implementation Details 5 Results and Analysis 5.1 RQ1: Overall Effectiveness of Trae Agent 5.1.1 Process: 5.1.2 Results: 5.2 RQ2: Influence of Hyper-parameter 5.2.1 Setup: 5.2.2 Results: 5.3 RQ3: Contribution of Main Components 5.3.1 Variants: 5.3.2 Results: 5.4 RQ4: Influence of Ensemble Space 5.4.1 Process 5.4.2 Results 6 Discussion 6.1 Practical Impact 6.2 Quality of Regression Tests 6.3 Future Work 7 Threats and Validity 8 Related Work 8.1 Automatic Software Issue Resolution 8.2 Ensemble Techniques for LLM 9 Conclusion Trae Agent: An LLM-based Agent for Software Engineering with Test-time Scaling Trae Research Beijing, China opensource@mail.trae.ai Abstract Software issue resolution is a critical challenge in software engineering and has garnered increasing attention in recent years. With the…

**Method / approach.** methods still face limitations in effectively exploring large ensemble spaces and lack the capacity for repository-level understanding, both of which constrain their overall effectiveness. In this paper, we propose Trae Agent , the first agent-based ensemble reasoning approach for repository-level issue resolution. Trae Agent formulates our goal as an optimal solution search problem and addresses two key challenges, i.e., large ensemble spaces and repository-level understanding, through modular agents for generation, pruning, and selection. We conduct extensive experiments using three leading LLMs on the widely-adopted SWE-bench benchmark, comparing Trae Agent against four state-of-the-art ensemble reasoning techniques. Experimental results demonstrate that Trae Agent consistently achieves superior performance, with an average improvement of 10.22% over all baselines in terms of Pass@1. Trae Agent has achieved first place on the SWE-bench Verified leaderboard, with a notable Pass@1…

**Results.** experiments using three leading LLMs on the widely-adopted SWE-bench benchmark, comparing Trae Agent against four state-of-the-art ensemble reasoning techniques. Experimental results demonstrate that Trae Agent consistently achieves superior performance, with an average improvement of 10.22% over all baselines in terms of Pass@1. Trae Agent has achieved first place on the SWE-bench Verified leaderboard, with a notable Pass@1 score of 75.20%. We are pleased to release Trae Agent as an open-source project to support the research community, with all resources available at https://github.com/bytedance/trae-agent . † † footnotetext: The list of authors is provided at the end of the technical report. 1 Introduction Software issue resolution refers to the automated handling of newly reported bugs or feature requests during software development and maintenance, aiming to ensure correct and reliable system behavior ( Fakhoury et…

**Conclusion.** Conclusion Trae Agent: An LLM-based Agent for Software Engineering with Test-time Scaling Trae Research Beijing, China opensource@mail.trae.ai Abstract Software issue resolution is a critical challenge in software engineering and has garnered increasing attention in recent years. With the rapid advancement of large language models (LLMs), substantial progress has been made in addressing real-world software engineering tasks. Recent studies have introduced ensemble reasoning techniques to enhance the performance of LLM-based issue resolution. However, existing prompting-based methods still face limitations in effectively exploring large ensemble spaces and lack the capacity for repository-level understanding, both of which const…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2507.23370v1.md` · `raw/arxiv/2507.23370v1.fulltext.md`
