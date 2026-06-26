---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SWE-PolyBench: A multi-language benchmark for repository level evaluation of coding agents"
authors: Muhammad Shihab Rashid, Christian Bock, Yuan Zhuang, Alexander Buchholz et al.
url: https://arxiv.org/abs/2504.08703v3
date: 2025-04-11
citationCount: 58
influentialCitationCount: 4
velocity: 4.04
ingested: 2026-06-22
tags: [coding-agents, agent-evaluation, arxiv, 2025, cited]
---

# SWE-PolyBench: A multi-language benchmark for repository level evaluation of coding agents

**arXiv [2504.08703v3](https://arxiv.org/abs/2504.08703v3)** · 2025-04-11 · **58 citations** (4 influential · 4.04/mo) · Muhammad Shihab Rashid, Christian Bock, Yuan Zhuang, Alexander Buchholz et al.

## Abstract
Coding agents powered by large language models have shown impressive capabilities in software engineering tasks, but evaluating their performance across diverse programming languages and real-world scenarios remains challenging. We introduce SWE-PolyBench, a new multi-language benchmark for repository-level, execution-based evaluation of coding agents. SWE-PolyBench contains 2110 instances from 21 repositories and includes tasks in Java (165), JavaScript (1017), TypeScript (729) and Python (199), covering bug fixes, feature additions, and code refactoring. We provide a task and repository-stratified subsample (SWE-PolyBench500) and release an evaluation harness allowing for fully automated evaluation. To enable a more comprehensive comparison of coding agents, this work also presents a novel set of metrics rooted in syntax tree analysis. We evaluate leading open source coding agents on SWE-PolyBench, revealing their strengths and limitations across languages, task types, and complexity classes. Our experiments show that current agents exhibit uneven performances across languages and struggle with complex problems while showing higher performance on simpler tasks. SWE-PolyBench aims to drive progress in developing more versatile and robust AI coding assistants for real-world software engineering. Our datasets and code are available at: https://github.com/amazon-science/SWE-PolyBench

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related work 3 Building SWE-PolyBench 3.1 Data Collection 3.2 Runtime Setup 4 SWE-PolyBench Characteristics 4.1 Contrasting SWE-PolyBench with SWE-Bench 4.2 LLM-based task classification Development task classification Informativeness of problem statements 4.3 SWE-PolyBench500 5 Evaluating Open-Source Coding Agents 5.1 Coding Agents 5.1.1 Technical Challenges in Making Coding Agents Multi-Lingual Aider Agentless SWE-agent 5.2 Metrics Pass rate Retrieval scores. 5.3 Results 5.3.1 Pass Rates 5.3.2 Retrieval Metrics 6 Limitations Task Diversity Evaluation Metrics Limits of execution-based evaluation Verifiability LLM-based Classifications Data Leakage 7 Conclusions A Appendix A.1 Prompts A.1.1 Prompt for classification of tasks A.1.2 Prompts for classification of problem statements A.2 Details CST retrieval metrics A.3 Task classifications and pass rates A.4 Results on SWE-PolyBench500 A.5 Collected Repositories \NewCommandCopy \ORIcitep , ) \NewCommandCopy…

**Method / approach.** methods to our multi-lingual framework. Lastly, we contrast their performance in terms of pass rate and various retrieval metrics. 5.1 Coding Agents For our comparison, we selected three open-source agents that are widely recognized and appreciated in both the research community and among practitioners. These include: • Aider (Gauthier, 2024 ) , an interactive pair programming agent. The agent suggests different changes to the codebase and the user can select or submit their preferences. To run Aider on the benchmarks, we disable the interactive part and always select the agents’ suggestions. • SWE-agent (Yang et al., 2024a ) which employs an agent-computer interface that can create and edit code files, navigate entire repositories, and execute tests and other programs. • Agentless (Xia et al., 2024 ) which uses a three-phase approach to 1) localize, 2) repair, and 3) validate code. It does not rely on autonomous agent-based interactions or complex to…

**Results.** experiments show that current agents exhibit uneven performances across languages and struggle with complex problems while showing higher performance on simpler tasks. SWE-PolyBench aims to drive progress in developing more versatile and robust AI coding assistants for real-world software engineering. Our datasets and code are available at: https://github.com/amazon-science/SWE-PolyBench Figure 1 : Pass rates of coding agents across programming languages (left) and across subsets of different complexities based on syntax tree nodes. The right plot categorizes changes by type (class or function) and scope (single or multiple), with ”No nodes” indicating no class or function changes and ”Mixed” requiring both. 1 Introduction Coding agents are language model-based, autonomous systems able to create or modify software with limited human inputs. Over the last year, coding agents have garnered substantial attention due to their pote…

**Conclusion.** Conclusions A Appendix A.1 Prompts A.1.1 Prompt for classification of tasks A.1.2 Prompts for classification of problem statements A.2 Details CST retrieval metrics A.3 Task classifications and pass rates A.4 Results on SWE-PolyBench500 A.5 Collected Repositories \NewCommandCopy \ORIcitep , ) \NewCommandCopy \ORIcitet () \AtBeginEnvironment appendices \AtBeginEnvironment appendices SWE-PolyBench: A multi-language benchmark for repository level evaluation of coding agents Muhammad Shihab Rashid Christian Bock 1 1 footnotemark: 1 Yuan Zhuang Alexander Buchholz Tim Esler 2 2 footnotemark: 2 Simon Valentin Luca Franceschi Martin Wistuba Prabhu Teja Sivaprasad Woo Jung Kim Anoop Deoras Giovan…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2504.08703v3.md` · `raw/arxiv/2504.08703v3.fulltext.md`
