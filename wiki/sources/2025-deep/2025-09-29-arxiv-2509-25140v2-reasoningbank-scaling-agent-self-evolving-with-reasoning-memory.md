---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory"
authors: Siru Ouyang, Jun Yan, I-Hung Hsu, Yanfei Chen et al.
url: https://arxiv.org/abs/2509.25140v2
date: 2025-09-29
citationCount: 126
influentialCitationCount: 26
velocity: 14.42
ingested: 2026-06-22
tags: [coding-agents, computer-use-agents, agent-reliability, self-evolving-agents, agent-memory, arxiv, 2025, cited]
---

# ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory

**arXiv [2509.25140v2](https://arxiv.org/abs/2509.25140v2)** · 2025-09-29 · **126 citations** (26 influential · 14.42/mo) · Siru Ouyang, Jun Yan, I-Hung Hsu, Yanfei Chen et al.

## Abstract
With the growing adoption of large language model agents in persistent real-world roles, they naturally encounter continuous streams of tasks. A key limitation, however, is their failure to learn from the accumulated interaction history, forcing them to discard valuable insights and repeat past errors. We propose ReasoningBank, a novel memory framework that distills generalizable reasoning strategies from an agent's self-judged successful and failed experiences. At test time, an agent retrieves relevant memories from ReasoningBank to inform its interaction and then integrates new learnings back, enabling it to become more capable over time. Building on this powerful experience learner, we further introduce memory-aware test-time scaling (MaTTS), which accelerates and diversifies this learning process by scaling up the agent's interaction experience. By allocating more compute to each task, the agent generates abundant, diverse experiences that provide rich contrastive signals for synthesizing higher-quality memory. The better memory in turn guides more effective scaling, establishing a powerful synergy between memory and test-time scaling. Across web browsing and software engineering benchmarks, ReasoningBank consistently outperforms existing memory mechanisms that store raw trajectories or only successful task routines, improving both effectiveness and efficiency; MaTTS further amplifies these gains. These findings establish memory-driven experience scaling as a new scaling dimension, enabling agents to self-evolve with emergent behaviors naturally arise. Our code can be found at https://github.com/google-research/reasoning-bank.

## From the paper (full-text excerpts)
**Introduction.** Introduction The rapid advancement of large language models (LLMs) has significantly accelerated the development of interactive LLM agents (Liu et al., 2025a; Wang et al., 2024), which are crucial in tackling complex real-world tasks that require multi-turn interactions with environments. These agents have demonstrated great potential across diverse scenarios, including web browsing (Gur et al., 2024), computer use (Xie et al., 2024; Yang et al., 2024), and scientific discovery (Ghafarollahi and Buehler, 2025). As these agents are increasingly deployed in persistent, long-running roles, they naturally encounter a continuous stream of tasks and interactions. However, a critical limitation persists: they largely fail to learn from this accumulated experience. By approaching each new task in isolation, they are doomed to (i) repeat similar errors observed in the past (Yin et al., 2025), (ii) discard valuable insights gained from related problems, and, most importantly, (iii) lack self-evolving capabilities that make the agent system more capable over time (Gao et al., 2026). This phenom…

**Method / approach.** methods usually involve retrieval mechanisms (e.g., semantic search) with memory management strategies (e.g., updating) (Hu et al., 2025a; Tan et al., 2025). More recently, with the growing development of reinforcement learning (RL) in LLM agents, RL has also been leveraged for memory management in agent systems (Yu et al., 2025a; Zhou et al., 2025). While most efforts primarily emphasize personalization (Zhang et al., 2025a; Zhong et al., 2024) and long-context management (Hu et al., 2025c; Maharana et al., 2024; Wu et al., 2025), this paper falls in the research line of learning from past experiences as memory (Su et al., 2025; Zhao et al., 2024), which is a critical aspect for developing self-evolving agent systems (Gao et al., 2026; Liang et al., 2024). Different from previous works that emphasize reusing successful trajectories (Tang et al., 2025a; Zheng et al., 2024), procedural workflows (Fang et al., 2025; Liu et al., 2025b; Nottingham et al., 2024; Qian et al., 2024; Wang et…

**Results.** experiments on challenging benchmarks for web browsing (WebArena, Mind2Web) and software engineering (SWE-Bench-Verified). We demonstrate that Re as on i ng Ban k outperforms baselines in both effectiveness (up to 20% relative improvement, Table 1) and efficiency (up to 16% fewer interaction steps, Table 1). Additionally, Re as on i ng Ban k synergizes best with MaT T S, making it an essential component for memory-driven experience scaling. Our contributions are threefold: (1) We propose ReasoningBank, a novel memory framework that distills generalizable reasoning strategies from both successful and failed experiences, beyond prior work that primarily stores raw trajectories or success-only routines. (2) We introduce MaT TS 2 Re as on i ng Ban k: Scaling Agent Self-Evolving with Reasoning Memory that establishes a powerful, bidirectional synergy between memory and test-time scaling, with memorydriven experience as a new scaling dimen…

**Conclusion.** Conclusion We introduce ReasoningBank, a memory framework that distills strategy-level reasoning signals from both successes and failures and integrates them into test-time scaling (MaT TS). Extensive experiments show that Re as on i ng Ban k consistently improves performance while reducing redundant exploration. Further results reveal a strong synergy between memory and scaling: ReasoningBank guides scaling toward more promising rollouts, while diverse rollouts enrich memory with valuable contrastive signals. We also provide analyses of individual components and emergent behaviors. Our findings suggest a practical pathway toward building adaptive and lifelong-learning agents, with additional future directions and limitations in Appendix D…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]]
- **Raw:** `raw/arxiv/2509.25140v2.md` · `raw/arxiv/2509.25140v2.fulltext.md`
