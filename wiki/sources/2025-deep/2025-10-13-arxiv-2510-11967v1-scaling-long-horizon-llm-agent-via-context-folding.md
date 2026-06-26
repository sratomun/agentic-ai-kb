---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Scaling Long-Horizon LLM Agent via Context-Folding"
authors: Weiwei Sun, Miao Lu, Zhan Ling, Kang Liu et al.
url: https://arxiv.org/abs/2510.11967v1
date: 2025-10-13
citationCount: 77
influentialCitationCount: 7
velocity: 9.3
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Scaling Long-Horizon LLM Agent via Context-Folding

**arXiv [2510.11967v1](https://arxiv.org/abs/2510.11967v1)** · 2025-10-13 · **77 citations** (7 influential · 9.3/mo) · Weiwei Sun, Miao Lu, Zhan Ling, Kang Liu et al.

## Abstract
Large language model (LLM) agents are fundamentally constrained by context length on long-horizon tasks. We introduce Context-Folding, a framework that empowers agents to actively manage their working context. An agent can procedurally branch into a sub-trajectory to handle a subtask and then fold it upon completion, collapsing the intermediate steps while retaining a concise summary of the outcome. To make this behavior learnable, we develop an end-to-end reinforcement learning framework FoldGRPO with specific process rewards to encourage effective task decomposition and context management. On complex long-horizon tasks (Deep Research and SWE), our folding agent matches or outperforms the ReAct baselines while using an active context 10$\times$ smaller and significantly outperforms models that rely on summarization-based context management.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large language model (LLM) agents have shown remarkable capabilities in tackling complex, long-horizon problems that require extensive interaction with an environment, such as deep research [8, 12, 17, 21, 32] and agentic coding [3, 11, 31]. The length of tasks agents can complete is argued to be growing exponentially, with a doubling time of about 7 months [20]. However, scaling LLM agents to even longer horizons is fundamentally constrained by the design of agentic frameworks [35]. These frameworks linearly accumulate the entire interaction history (reasoning, tool calls, and observations) into a single, ever-expanding context, which incurs long-context challenges as horizons scale: (1) degraded performance, as LLMs struggle to utilize relevant information in exceedingly long contexts [14, 18, 28]; and (2) poor efficiency, stemming from the quadratic scaling of attention mechanisms and the growing overhead of managing the KV-cache [13]. Existing approaches to scale long-horizon LLM agents largely fall into two classes: (1) Summary-based methods, which trigger a post-h…

**Method / approach.** methods, which trigger a post-hoc summarization stage when the working context is full [1, 19, 24, 34, 38, 43]. While this compresses the context, it can abruptly disrupt the agent’s working context and reasoning flow, which may lead to sub-optimal results. (2) Multi-agent systems, which distribute tasks across specialized agents to manage context length [2, 33, 40, 41]. Yet, these systems typically depend on handcrafted, problem-specific workflows that are difficult to generalize and resist end-to-end optimization. 1 Figure 1 Examples of context folding in long-horizon tasks: deep research (left) and agentic coding (right). In this paper, we propose Context Folding: an agentic mechanism that allows the model to actively manage its working context. Specifically, the agent manages its context using two special actions: (i) a branch action to create a temporary sub-trajectory for a localized subtask; and (ii) a return action to summarize the outcome and rejoin the main thread, after…

**Results.** Experiment 3.1 Datasets We conduct experiment on two representative long-horizon agent tasks: deep research, and agentic software engineering: Deep Research. We use BrowseComp-Plus (BC-Plus) [6], which supplements the original BrowseComp data with a verified corpus. We use Qwen3-Embed-8B as the retriever. Since the quality of training data is crucial for the BrowseComp task but existing datasets are typically not open-sourced [15, 24], we split BrowseComp-Plus into training and evaluation sets to decouple the effect of data distribution. Our split includes 680 instances for training and 150 for evaluation. For deep research, the tools are search(query, topk) and open_page(url), and the reward is based on official LLM-based judger [6]. Agentic SWE. We use SWE-Bench Verified (SWEB-V) [11] as the evaluation set. To collect training data, we roll out the baseline agent1 eight times on a subset of the open-source datasets SWE-Gym [23] an…

**Conclusion.** Conclusions and Future Work In this paper, we introduced context folding, an agentic mechanism for managing long-horizon trajectories by selectively folding ephemeral sub-trajectories while preserving only essential decision-relevant information. Coupled with our reinforcement learning framework, context folding enables efficient credit assignment across tree-structured trajectories and achieves significant improvements in long-horizon coding and deep-research tasks. Empirical results on two long-context tasks demonstrate that folding allows agents to match or exceed the performance of baselines with larger context windows, while improving efficiency and stability relative to summary-based condensation. Several promising future directions…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2510.11967v1.md` · `raw/arxiv/2510.11967v1.fulltext.md`
