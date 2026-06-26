---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Mind2Web 2: Evaluating Agentic Search with Agent-as-a-Judge"
authors: Boyu Gou, Zanming Huang, Yuting Ning, Yu Gu et al.
url: https://arxiv.org/abs/2506.21506v2
date: 2025-06-26
citationCount: 51
influentialCitationCount: 4
velocity: 4.3
ingested: 2026-06-22
tags: [computer-use-agents, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Mind2Web 2: Evaluating Agentic Search with Agent-as-a-Judge

**arXiv [2506.21506v2](https://arxiv.org/abs/2506.21506v2)** · 2025-06-26 · **51 citations** (4 influential · 4.3/mo) · Boyu Gou, Zanming Huang, Yuting Ning, Yu Gu et al.

## Abstract
Agentic search such as Deep Research systems-where agents autonomously browse the web, synthesize information, and return comprehensive citation-backed answers-represents a major shift in how users interact with web-scale information. While promising greater efficiency and cognitive offloading, the growing complexity and open-endedness of agentic search have outpaced existing evaluation benchmarks and methodologies, which largely assume short search horizons and static answers. In this paper, we introduce Mind2Web 2, a benchmark of 130 realistic, high-quality, and long-horizon tasks that require real-time web browsing and extensive information synthesis, constructed with over 1000 hours of human labor. To address the challenge of evaluating time-varying and complex answers, we propose a novel Agent-as-a-Judge framework. Our method constructs task-specific judge agents based on a tree-structured rubric design to automatically assess both answer correctness and source attribution. We conduct a comprehensive evaluation of ten frontier agentic search systems and human performance, along with a detailed error analysis to draw insights for future development. The best-performing system, OpenAI Deep Research, can already achieve 50-70% of human performance while spending half the time, highlighting its great potential. Altogether, Mind2Web 2 provides a rigorous foundation for developing and benchmarking the next generation of agentic search systems.

## From the paper (full-text excerpts)
**Introduction.** Introduction Web search has long been the gateway to the world’s knowledge, underpinning everything from everyday fact-checking to frontier scientific discovery. The core techniques supporting web search have undergone constant evolution in the past decades, from TF-IDF [32] for term statistics to PageRank [3] for network analysis and learning to rank [4, 20] for supervised learning. Yet the core interaction model has remained essentially unchanged: users issue a query, receive a ranked list of URLs, and must manually open, read, and synthesize multiple webpages to answer complex questions. Current web search is inherently user-driven: it retrieves pieces of information but relies on users to interpret and assemble those pieces. That places a significant cognitive load on users, especially as the complexity of the digital world grows. Recent advances in large language models (LLMs) have sparked the development of agentic search systems. Rather than taking keyword queries and returning lists of links, agentic search systems decompose and plan for complex queries, iteratively search t…

**Method / approach.** methodologies, which largely assume short search horizons and static answers. In this paper, we introduce Mind2Web 2, a benchmark of 130 realistic, high-quality, and long-horizon tasks that require real-time web browsing and extensive information synthesis, constructed with over 1,000 hours of human labor. To address the challenge of evaluating time-varying and complex answers, we propose a novel Agent-as-a-Judge framework. Our method constructs task-specific judge agents based on a tree-structured rubric design to automatically assess both answer correctness and source attribution. We conduct a comprehensive evaluation of ten frontier agentic search systems and human performance, along with a detailed error analysis to draw insights for future development. The best-performing system, OpenAI Deep Research, can already achieve 50-70% of human performance while spending half the time, highlighting its great potential. Altogether, Mind2Web 2 provides a rigorous foundation for developing…

**Results.** Experiments 4.1 Experimental Setup We evaluate agentic search systems of various types on Mind2Web 2. Given the complexity of our tasks, we focus on frontier systems capable of yielding meaningful results, namely, those exhibit sufficient long-horizon search capability and can consistently provide source attributions. We report two primary metrics: Partial Completion and Success Rate, as defined in §3.3. We run and evaluate each system independently over three runs per task, and we present the averaged metrics along with their standard deviations. Additionally, we introduce Pass@3, indicating whether at least one of the three attempts for a task is successful. To further contextualize system performance, we also report behavioral aspects influencing user experience, including the average task completion time and average answer length.4 We report results on the private test set, reserving the public development set for unrestricted ex…

**Conclusion.** conclusion), frequently exceeding thousands of words. However, despite the apparent comprehensiveness of these reports, our evaluation reveals that their increased length does not necessarily result in better task completion. Moreover, excessively lengthy reports can be cognitively burdensome and suboptimal for users seeking concise and targeted information. Test-Time Scaling. As illustrated in Figure 3, we observe clear performance improvements resulting from increased inference time. The benefit is especially evident when comparing systems within the same family (e.g., Grok and Perplexity), given that they presumably share the same underlying models. This observation aligns intuitively with the complexity of our tasks, which inherently de…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.21506v2.md` · `raw/arxiv/2506.21506v2.fulltext.md`
