---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebExplorer: Explore and Evolve for Training Long-Horizon Web Agents"
authors: Junteng Liu, Yunji Li, Chi Zhang, Jingyang Li et al.
url: https://arxiv.org/abs/2509.06501v3
date: 2025-09-08
citationCount: 65
influentialCitationCount: 7
velocity: 6.89
ingested: 2026-06-22
tags: [computer-use-agents, embodied-agents, agentic-rl, agent-memory, tool-use, arxiv, 2025, cited]
---

# WebExplorer: Explore and Evolve for Training Long-Horizon Web Agents

**arXiv [2509.06501v3](https://arxiv.org/abs/2509.06501v3)** · 2025-09-08 · **65 citations** (7 influential · 6.89/mo) · Junteng Liu, Yunji Li, Chi Zhang, Jingyang Li et al.

## Abstract
The paradigm of Large Language Models (LLMs) has increasingly shifted toward agentic applications, where web browsing capabilities are fundamental for retrieving information from diverse online sources. However, existing open-source web agents either demonstrate limited information-seeking abilities on complex tasks or lack transparent implementations. In this work, we identify that the key challenge lies in the scarcity of challenging data for information seeking. To address this limitation, we introduce WebExplorer: a systematic data generation approach using model-based exploration and iterative, long-to-short query evolution. This method creates challenging query-answer pairs that require multi-step reasoning and complex web navigation. By leveraging our curated high-quality dataset, we successfully develop advanced web agent WebExplorer-8B through supervised fine-tuning followed by reinforcement learning. Our model supports 128K context length and up to 100 tool calling turns, enabling long-horizon problem solving. Across diverse information-seeking benchmarks, WebExplorer-8B achieves the state-of-the-art performance at its scale. Notably, as an 8B-sized model, WebExplorer-8B is able to effectively search over an average of 16 turns after RL training, achieving higher accuracy than WebSailor-72B on BrowseComp-en/zh and attaining the best performance among models up to 100B parameters on WebWalkerQA and FRAMES. Beyond these information-seeking tasks, our model also achieves strong generalization on the HLE benchmark even though it is only trained on knowledge-intensive QA data. These results highlight our approach as a practical path toward long-horizon web agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 WebExplorer : Synthesizing Challenging QA Pairs 2.1 Preliminaries 2.2 Model-Based Exploration 2.3 Iterative Query Evolution 2.4 The WebExplorer -QA Dataset 3 Cold Start and Reinforcement learning 3.1 Supervised Fine-tuning for Cold Start 3.2 Reinforcement Learning 4 Experiments 4.1 Experimental Setups 4.2 Experimental Results 5 Conclusion A Trajectory Example B Details of WebExplorer -QA Synthesis Framework B.1 Model-Based Exploration B.2 Iterative Query Evolution C Tool Schemas C.1 Search Tool C.2 Browse Tool \reportnumber WebExplorer : Explore and Evolve for Training Long-Horizon Web Agents Junteng Liu 1* Yunji Li 2* Chi Zhang 2 Jingyang Li 2 Aili Chen 2 Ke Ji 2 Weiyu Cheng 2 Zijia Wu 2 Chengyu Du 2 Qidi Xu 2 Jiayuan Song 2 Zhengmao Zhu 2 Wenhu Chen 3 Pengyu Zhao 2 Junxian He 1 1 The Hong Kong University of Science and Technology 2 MiniMax 3 University of Waterloo jliugi@cse.ust.hk junxianh@cse.ust.hk https://github.com/hkust-nlp/WebExplorer Abstract The p…

**Method / approach.** method creates challenging query-answer pairs that require multi-step reasoning and complex web navigation. By leveraging our curated high-quality dataset, we successfully develop advanced web agent WebExplorer -8B through supervised fine-tuning followed by reinforcement learning. Our model supports 128K context length and up to 100 tool calling turns, enabling long-horizon problem solving. Across diverse information-seeking benchmarks, WebExplorer -8B achieves the state-of-the-art performance at its scale. Notably, as an 8B-sized model, WebExplorer -8B is able to effectively search over an average of 16 turns after RL training, achieving higher accuracy than WebSailor-72B on BrowseComp-en/zh and attaining the best performance among models up to 100B parameters on WebWalkerQA and FRAMES. Beyond these information-seeking tasks, our model also achieves strong generalization on the HLE benchmark even though it is only trained on knowledge-intensive QA data. These results highlight our ap…

**Results.** Experiments 4.1 Experimental Setups 4.2 Experimental Results 5 Conclusion A Trajectory Example B Details of WebExplorer -QA Synthesis Framework B.1 Model-Based Exploration B.2 Iterative Query Evolution C Tool Schemas C.1 Search Tool C.2 Browse Tool \reportnumber WebExplorer : Explore and Evolve for Training Long-Horizon Web Agents Junteng Liu 1* Yunji Li 2* Chi Zhang 2 Jingyang Li 2 Aili Chen 2 Ke Ji 2 Weiyu Cheng 2 Zijia Wu 2 Chengyu Du 2 Qidi Xu 2 Jiayuan Song 2 Zhengmao Zhu 2 Wenhu Chen 3 Pengyu Zhao 2 Junxian He 1 1 The Hong Kong University of Science and Technology 2 MiniMax 3 University of Waterloo jliugi@cse.ust.hk junxianh@cse.ust.hk https://github.com/hkust-nlp/WebExplorer Abstract The paradigm of Large Language Models (LLMs) has increasingly shifted toward agentic applications, where web browsing capabilities are fundamental for retrieving i…

**Conclusion.** Conclusion A Trajectory Example B Details of WebExplorer -QA Synthesis Framework B.1 Model-Based Exploration B.2 Iterative Query Evolution C Tool Schemas C.1 Search Tool C.2 Browse Tool \reportnumber WebExplorer : Explore and Evolve for Training Long-Horizon Web Agents Junteng Liu 1* Yunji Li 2* Chi Zhang 2 Jingyang Li 2 Aili Chen 2 Ke Ji 2 Weiyu Cheng 2 Zijia Wu 2 Chengyu Du 2 Qidi Xu 2 Jiayuan Song 2 Zhengmao Zhu 2 Wenhu Chen 3 Pengyu Zhao 2 Junxian He 1 1 The Hong Kong University of Science and Technology 2 MiniMax 3 University of Waterloo jliugi@cse.ust.hk junxianh@cse.ust.hk https://github.com/hkust-nlp/WebExplorer Abstract The paradigm of Large Language Mode…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Raw:** `raw/arxiv/2509.06501v3.md` · `raw/arxiv/2509.06501v3.fulltext.md`
