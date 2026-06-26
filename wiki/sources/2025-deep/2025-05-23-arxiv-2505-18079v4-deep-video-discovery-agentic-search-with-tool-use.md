---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Deep Video Discovery: Agentic Search with Tool Use for Long-form Video Understanding"
authors: Xiaoyi Zhang, Zhaoyang Jia, Zongyu Guo, Jiahao Li et al.
url: https://arxiv.org/abs/2505.18079v4
date: 2025-05-23
citationCount: 50
influentialCitationCount: 10
velocity: 3.85
ingested: 2026-06-22
tags: [tool-use, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Deep Video Discovery: Agentic Search with Tool Use for Long-form Video Understanding

**arXiv [2505.18079v4](https://arxiv.org/abs/2505.18079v4)** · 2025-05-23 · **50 citations** (10 influential · 3.85/mo) · Xiaoyi Zhang, Zhaoyang Jia, Zongyu Guo, Jiahao Li et al.

## Abstract
Long-form video understanding presents significant challenges due to extensive temporal-spatial complexity and the difficulty of question answering under such extended contexts. While Large Language Models (LLMs) have demonstrated considerable advancements in video analysis capabilities and long context handling, they continue to exhibit limitations when processing information-dense hour-long videos. To overcome such limitations, we propose the Deep Video Discovery (DVD) agent to leverage an agentic search strategy over segmented video clips. Unlike previous video agents that rely on predefined workflows applied uniformly across different queries, our approach emphasizes the autonomous and adaptive nature of agents. By providing a set of search-centric tools on multi-granular video database, our DVD agent leverages the advanced reasoning capability of LLM to plan on its current observation state, strategically selects tools to orchestrate adaptive workflow for different queries in light of the gathered information. We perform comprehensive evaluation on multiple long video understanding benchmarks that demonstrates our advantage. Our DVD agent achieves state-of-the-art performance on the challenging LVBench dataset, reaching an accuracy of 74.2%, which substantially surpasses all prior works, and further improves to 76.0% with transcripts. The code has been released at https://github.com/microsoft/DeepVideoDiscovery.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Long Video Understanding. Agent and tool use. 3 Deep Video Discovery Overview. 3.1 Multi-granular Video Database Construction Temporal segmentation. Multi-granular information extraction. Outcome. 3.2 Agentic Search and Answer with Tool Use 3.2.1 Search-centric Tool Preparation Tool: Global Browse. Tool: Clip Search. Tool: Frame Inspect. 3.2.2 Agentic Design 4 Experiment 4.1 Benchmarks 4.2 Implementation Details 4.3 Main Results 4.4 Ablation Study 4.5 Analysis on Efficiency 4.6 Analysis on Agentic Reasoning Behavior 5 Conclusion A Evaluation Details A.1 Prompts A.2 Cost A.3 Azure OpenAI Service A.3.1 Maximum Image Count Limitation A.3.2 API Content Filtering B More Results B.1 Statistical Significance B.2 Case Study C Broader Impacts C.1 Positive Impacts C.2 Negative Impacts Deep Video Discovery : Agentic Search with Tool Use for Long-form Video Understanding Xiaoyi Zhang 1 Zhaoyang Jia ∗2 Zongyu Guo 1 Jiahao Li 1 Bin Li 1 Houqiang Li 2…

**Method / approach.** methods. Most critically, these existing frameworks prescribe fixed workflows that are uniformly applied across all query types, failing to adapt to the diverse information needs and optimal search strategies required by different questions. In contrast to existing systems that typically rely on manually defined, rigid workflows, our approach is distinctly designed around an autonomous and adaptive agentic search paradigm for different queries. Instead of explicitly prescribing task workflows or search behaviors, we develop modular search tools that operate at multiple granularities, including (1) Global Browse , (2) Clip Search , and (3) Frame Inspect . Global Browse enables global summarization and indexing of subjects and global contexts across the entire video. Clip Search implements efficient semantic retrieval of relevant events within segmented clips. Specifically, Frame Inspection empowers the agent to extract fine-grained details directly from pixel-level information in a…

**Results.** Experiment 4.1 Benchmarks 4.2 Implementation Details 4.3 Main Results 4.4 Ablation Study 4.5 Analysis on Efficiency 4.6 Analysis on Agentic Reasoning Behavior 5 Conclusion A Evaluation Details A.1 Prompts A.2 Cost A.3 Azure OpenAI Service A.3.1 Maximum Image Count Limitation A.3.2 API Content Filtering B More Results B.1 Statistical Significance B.2 Case Study C Broader Impacts C.1 Positive Impacts C.2 Negative Impacts Deep Video Discovery : Agentic Search with Tool Use for Long-form Video Understanding Xiaoyi Zhang 1 Zhaoyang Jia ∗2 Zongyu Guo 1 Jiahao Li 1 Bin Li 1 Houqiang Li 2 Yan Lu 1 1 Microsoft Research Asia 2 University of Science and Technology of China {xiaoyizhang, zongyuguo, jiahaoli, binli, yanlu}@microsoft.com {jzy_ustc, lihq}@ustc.edu.cn Equal contribution. This work was done during the internship at Microsoft Research Asia as an open-sour…

**Conclusion.** Conclusion A Evaluation Details A.1 Prompts A.2 Cost A.3 Azure OpenAI Service A.3.1 Maximum Image Count Limitation A.3.2 API Content Filtering B More Results B.1 Statistical Significance B.2 Case Study C Broader Impacts C.1 Positive Impacts C.2 Negative Impacts Deep Video Discovery : Agentic Search with Tool Use for Long-form Video Understanding Xiaoyi Zhang 1 Zhaoyang Jia ∗2 Zongyu Guo 1 Jiahao Li 1 Bin Li 1 Houqiang Li 2 Yan Lu 1 1 Microsoft Research Asia 2 University of Science and Technology of China {xiaoyizhang, zongyuguo, jiahaoli, binli, yanlu}@microsoft.com {jzy_ustc, lihq}@ustc.edu.cn Equal contribution. This work was done during the internship at Microsoft Researc…

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.18079v4.md` · `raw/arxiv/2505.18079v4.fulltext.md`
