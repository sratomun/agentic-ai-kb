---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Establishing Best Practices for Building Rigorous Agentic Benchmarks"
authors: Yuxuan Zhu, Tengjun Jin, Yada Pruksachatkun, Andy Zhang et al.
url: https://arxiv.org/abs/2507.02825v5
date: 2025-07-03
citationCount: 52
influentialCitationCount: 3
velocity: 4.47
ingested: 2026-06-22
tags: [coding-agents, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Establishing Best Practices for Building Rigorous Agentic Benchmarks

**arXiv [2507.02825v5](https://arxiv.org/abs/2507.02825v5)** · 2025-07-03 · **52 citations** (3 influential · 4.47/mo) · Yuxuan Zhu, Tengjun Jin, Yada Pruksachatkun, Andy Zhang et al.

## Abstract
Benchmarks are essential for quantitatively tracking progress in AI. As AI agents become increasingly capable, researchers and practitioners have introduced agentic benchmarks to evaluate agents on complex, real-world tasks. These benchmarks typically measure agent capabilities by evaluating task outcomes via specific reward designs. However, we show that many agentic benchmarks have issues in task setup or reward design. For example, SWE-bench Verified uses insufficient test cases, while TAU-bench counts empty responses as successful. Such issues can lead to under- or overestimation of agents' performance by up to 100% in relative terms. To make agentic evaluation rigorous, we introduce the Agentic Benchmark Checklist (ABC), a set of guidelines that we synthesized from our benchmark-building experience, a survey of best practices, and previously reported issues. When applied to CVE-Bench, a benchmark with a particularly complex evaluation design, ABC reduces the performance overestimation by 33%.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Overview 4 ABC: Agentic Benchmark Checklist 4.1 Assessing Task Validity 4.2 Assessing Outcome Validity 4.3 Assessing the Benchmark Reporting 5 Assessment of Agentic Benchmarks 5.1 Assessment Scores 5.2 Assessment Findings 5.3 Revising CVE-Bench 6 Conclusion 7 Acknowledgements A Limitation and Impact Statement B Details of Benchmark Collection and Selection C Sources of the Checks in ABC D Assessment Reports E Case Study E.1 SWE-bench E.2 τ \tau italic_τ -bench E.3 BIRD E.4 SWE-Lancer E.5 WebArena E.6 KernelBench F An Example of Rigorous Benchmark Reporting G NeurIPS Paper Checklist Establishing Best Practices for Building Rigorous Agentic Benchmarks Yuxuan Zhu 1 Tengjun Jin 1 Yada Pruksachatkun Andy Zhang 2 Shu Liu 3 Sasha Cui 4 Sayash Kapoor 5 Shayne Longpre 6 Kevin Meng 7 Rebecca Weiss 8 Fazl Barez 8,11 Rahul Gupta 9 Jwala Dhamala 9 Jacob Merizian 10 Mario Giulianelli 10 Harry Coppock 10 Cozmin Ududec 10 Jasjeet Sekhon 4 Jacob Steinhardt…

**Method / approach.** methods, such as program testing and string matching [ 93 , 86 , 30 , 83 , 11 , 37 , 89 , 59 , 47 ] . Unfortunately, many existing outcome-based evaluation methods of agentic benchmarks introduce issues that can cause under- or overestimation of agent capabilities by up to 100% in relative terms, compromising the validity of their findings [ 87 , 35 , 80 , 62 , 46 ] . For example, SWE-bench-Verified challenges an agent to resolve GitHub issues, and considers the agent successful if the patch it generates passes manually vetted unit tests [ 14 ] . However, recent work has shown that passing these tests does not necessarily indicate that the issue is resolved, because unit tests can fail to capture important edge cases. Consequently, 24% of the top 50 leaderboard positions are incorrect [ 87 , 31 ] . In addition, we find that in τ \tau italic_τ -bench, a trivial agent that returns empty responses is considered successful on intentionally impossible tasks (e.g., changing a non-refund…

**Results.** experiments to validate the issue and obtained quantitative results (Section 5 ). We defer detailed assessment results to Appendix D and case studies to Appendix E . 4 ABC: Agentic Benchmark Checklist In this section, we formulate our assessment framework into an actionable checklist (ABC). We present the checklist items in terms of task validity, outcome validity, and benchmark reporting. 4.1 Assessing Task Validity Figure 2 : Checks in ABC to assess the task validity of an agentic benchmark. We propose guidelines for ensuring task validity. These checks uncover design or implementation flaws that can create shortcuts, which causes false positive evaluation results, or lead to impossible tasks, which causes false negative evaluation results. Tool . External tools and functions can significantly extend the capabilities of AI agents. Existing benchmarks provide two types of tools: self-hosted tools (e.g., Python, comm…

**Conclusion.** Conclusion 7 Acknowledgements A Limitation and Impact Statement B Details of Benchmark Collection and Selection C Sources of the Checks in ABC D Assessment Reports E Case Study E.1 SWE-bench E.2 τ \tau italic_τ -bench E.3 BIRD E.4 SWE-Lancer E.5 WebArena E.6 KernelBench F An Example of Rigorous Benchmark Reporting G NeurIPS Paper Checklist Establishing Best Practices for Building Rigorous Agentic Benchmarks Yuxuan Zhu 1 Tengjun Jin 1 Yada Pruksachatkun Andy Zhang 2 Shu Liu 3 Sasha Cui 4 Sayash Kapoor 5 Shayne Longpre 6 Kevin Meng 7 Rebecca Weiss 8 Fazl Barez 8,11 Rahul Gupta 9 Jwala Dhamala 9 Jacob Merizian 10 Mario Giulianelli 10 Harry Coppock 10 Cozmin Ududec…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2507.02825v5.md` · `raw/arxiv/2507.02825v5.fulltext.md`
