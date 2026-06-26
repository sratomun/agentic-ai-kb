---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A-MEM: Agentic Memory for LLM Agents"
authors: Wujiang Xu, Zujie Liang, Kai Mei, Hang Gao et al.
url: https://arxiv.org/abs/2502.12110v11
date: 2025-02-17
citationCount: 651
influentialCitationCount: 101
velocity: 40.44
ingested: 2026-06-22
tags: [agent-memory, agentic-ai, arxiv, 2025, cited]
---

# A-MEM: Agentic Memory for LLM Agents

**arXiv [2502.12110v11](https://arxiv.org/abs/2502.12110v11)** · 2025-02-17 · **651 citations** (101 influential · 40.44/mo) · Wujiang Xu, Zujie Liang, Kai Mei, Hang Gao et al.

**Significance:** Defined the agentic-memory pattern (interlinked, self-organizing notes) that much of 2026 memory work builds on.

## Abstract
While large language model (LLM) agents can effectively use external tools for complex real-world tasks, they require memory systems to leverage historical experiences. Current memory systems enable basic storage and retrieval but lack sophisticated memory organization, despite recent attempts to incorporate graph databases. Moreover, these systems' fixed operations and structures limit their adaptability across diverse tasks. To address this limitation, this paper proposes a novel agentic memory system for LLM agents that can dynamically organize memories in an agentic way. Following the basic principles of the Zettelkasten method, we designed our memory system to create interconnected knowledge networks through dynamic indexing and linking. When a new memory is added, we generate a comprehensive note containing multiple structured attributes, including contextual descriptions, keywords, and tags. The system then analyzes historical memories to identify relevant connections, establishing links where meaningful similarities exist. Additionally, this process enables memory evolution - as new memories are integrated, they can trigger updates to the contextual representations and attributes of existing historical memories, allowing the memory network to continuously refine its understanding. Our approach combines the structured organization principles of Zettelkasten with the flexibility of agent-driven decision making, allowing for more adaptive and context-aware memory management. Empirical experiments on six foundation models show superior improvement against existing SOTA baselines. The source code for evaluating performance is available at https://github.com/WujiangXu/A-mem, while the source code of the agentic memory system is available at https://github.com/WujiangXu/A-mem-sys.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Memory for LLM Agents 2.2 Retrieval-Augmented Generation 3 Methodolodgy 3.1 Note Construction 3.2 Link Generation 3.3 Memory Evolution 3.4 Retrieve Relative Memory 4 Experiment 4.1 Dataset and Evaluation 4.2 Implementation Details 4.3 Empricial Results 4.4 Ablation Study 4.5 Hyperparameter Analysis 4.6 Scaling Analysis 4.7 Memory Analysis 5 Conclusions 6 Limitations A Experiment A.1 Detailed Baselines Introduction A.2 Evaluation Metric A.3 Comparison Results A.4 Memory Analysis A.5 Hyperparameters setting B Prompt Templates and Examples B.1 Prompt Template of Note Construction B.2 Prompt Template of Link Generation B.3 Prompt Template of Memory Evolution B.4 Examples of Q/A with A-Mem A-Mem: Agentic Memory for LLM Agents Wujiang Xu 1 , Zujie Liang 2 , Kai Mei 1 , Hang Gao 1 , Juntao Tan 1 , Yongfeng Zhang 1,3 1 Rutgers University 2 Independent Researcher 3 AIOS Foundation wujiang.xu@rutgers.edu Abstract While large language model (LLM) agents can effectiv…

**Method / approach.** Methodolodgy 3.1 Note Construction 3.2 Link Generation 3.3 Memory Evolution 3.4 Retrieve Relative Memory 4 Experiment 4.1 Dataset and Evaluation 4.2 Implementation Details 4.3 Empricial Results 4.4 Ablation Study 4.5 Hyperparameter Analysis 4.6 Scaling Analysis 4.7 Memory Analysis 5 Conclusions 6 Limitations A Experiment A.1 Detailed Baselines Introduction A.2 Evaluation Metric A.3 Comparison Results A.4 Memory Analysis A.5 Hyperparameters setting B Prompt Templates and Examples B.1 Prompt Template of Note Construction B.2 Prompt Template of Link Generation B.3 Prompt Template of Memory Evolution B.4 Examples of Q/A with A-Mem A-Mem: Agentic Memory for LLM Agents Wujiang Xu 1 , Zujie Liang 2 , Kai Mei 1 , Hang Gao 1 , Juntao Tan 1 , Yongfeng Zhang 1,3 1 Rutgers University 2 Independent Researcher 3 AIOS Foundation wujiang.xu@rutgers.edu Abstract While large language model (LLM) agents can effectively…

**Results.** Experiment 4.1 Dataset and Evaluation 4.2 Implementation Details 4.3 Empricial Results 4.4 Ablation Study 4.5 Hyperparameter Analysis 4.6 Scaling Analysis 4.7 Memory Analysis 5 Conclusions 6 Limitations A Experiment A.1 Detailed Baselines Introduction A.2 Evaluation Metric A.3 Comparison Results A.4 Memory Analysis A.5 Hyperparameters setting B Prompt Templates and Examples B.1 Prompt Template of Note Construction B.2 Prompt Template of Link Generation B.3 Prompt Template of Memory Evolution B.4 Examples of Q/A with A-Mem A-Mem: Agentic Memory for LLM Agents Wujiang Xu 1 , Zujie Liang 2 , Kai Mei 1 , Hang Gao 1 , Juntao Tan 1 , Yongfeng Zhang 1,3 1 Rutgers University 2 Independent Researcher 3 AIOS Foundation wujiang.xu@rutgers.edu Abstract While large language model (LLM) agents can effectively use external tools for complex real-world tasks, they require memory s…

**Conclusion.** Conclusions 6 Limitations A Experiment A.1 Detailed Baselines Introduction A.2 Evaluation Metric A.3 Comparison Results A.4 Memory Analysis A.5 Hyperparameters setting B Prompt Templates and Examples B.1 Prompt Template of Note Construction B.2 Prompt Template of Link Generation B.3 Prompt Template of Memory Evolution B.4 Examples of Q/A with A-Mem A-Mem: Agentic Memory for LLM Agents Wujiang Xu 1 , Zujie Liang 2 , Kai Mei 1 , Hang Gao 1 , Juntao Tan 1 , Yongfeng Zhang 1,3 1 Rutgers University 2 Independent Researcher 3 AIOS Foundation wujiang.xu@rutgers.edu Abstract While large language model (LLM) agents can effectively use external tools for complex real-world tasks, they require memo…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[a-mem]]
- **Raw:** `raw/arxiv/2502.12110v11.md` · `raw/arxiv/2502.12110v11.fulltext.md`
