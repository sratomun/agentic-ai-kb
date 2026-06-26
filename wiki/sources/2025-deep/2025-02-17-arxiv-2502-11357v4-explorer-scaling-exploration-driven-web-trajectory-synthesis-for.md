---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Explorer: Scaling Exploration-driven Web Trajectory Synthesis for Multimodal Web Agents"
authors: Vardaan Pahuja, Yadong Lu, Corby Rosset, Boyu Gou et al.
url: https://arxiv.org/abs/2502.11357v4
date: 2025-02-17
citationCount: 60
influentialCitationCount: 3
velocity: 3.73
ingested: 2026-06-22
tags: [computer-use-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Explorer: Scaling Exploration-driven Web Trajectory Synthesis for Multimodal Web Agents

**arXiv [2502.11357v4](https://arxiv.org/abs/2502.11357v4)** · 2025-02-17 · **60 citations** (3 influential · 3.73/mo) · Vardaan Pahuja, Yadong Lu, Corby Rosset, Boyu Gou et al.

## Abstract
Recent success in large multimodal models (LMMs) has sparked promising applications of agents capable of autonomously completing complex web tasks. While open-source LMM agents have made significant advances in offline evaluation benchmarks, their performance still falls substantially short of human-level capabilities in more realistic online settings. A key bottleneck is the lack of diverse and large-scale trajectory-level datasets across various domains, which are expensive to collect. In this paper, we address this challenge by developing a scalable recipe to synthesize the largest and most diverse trajectory-level dataset to date, containing over 94K successful multimodal web trajectories, spanning 49K unique URLs, 720K screenshots, and 33M web elements. In particular, we leverage extensive web exploration and refinement to obtain diverse task intents. The average cost is 28 cents per successful trajectory, making it affordable to a wide range of users in the community. Leveraging this dataset, we train Explorer, a multimodal web agent, and demonstrate strong performance on both offline and online web agent benchmarks such as Mind2Web-Live, Multimodal-Mind2Web, and MiniWob++. Additionally, our experiments highlight data scaling as a key driver for improving web agent capabilities. We hope this study makes state-of-the-art LMM-based agent research at a larger scale more accessible.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Data Recipe 3.1 Website Selection 3.2 Data Generation Pipeline Task Proposer. Task Refiner. Task Summarizer. Task Verifier. 3.3 Dataset Analysis 4 Experiments Multimodal-Mind2Web. Mind2Web-Live. MiniWob++. 5 Results 5.1 In-domain Evaluation 5.2 Mind2Web-Live Results Improvement over base pre-trained models. Improvement over higher capacity pre-trained models. 5.3 Multimodal-Mind2Web Results 5.4 MiniWob++ Results 5.5 Data Scaling Experiments 6 Analyses Diversity Analysis. Analysis of Verifier Accuracy. Failure Modes of Trajectory Generation. 7 Conclusion A Mind2Web Training and Evaluation Details A.1 Mind2Web-Live A.2 Multimodal-Mind2Web A.3 Ablation Studies A.4 Case Studies for Mind2Web-Live B Cost Analysis C Task Complexity Analysis D System Prompts E Trajectory Examples F More Related Work F.1 LLM-based Web Agents F.2 Web Agent Benchmarks and Datasets Explorer: Scaling Exploration-driven Web Trajectory Synthesis for Multimodal Web Agents Va…

**Method / approach.** methods of effective agent tuning for large language models . In Findings of ACL . Cheng et al. (2024) Kanzhi Cheng, Qiushi Sun, Yougang Chu, Fangzhi Xu, Yantao Li, Jianbing Zhang, and Zhiyong Wu. 2024. Seeclick: Harnessing GUI grounding for advanced visual GUI agents . In Proceedings of ACL . Deng et al. (2023) Xiang Deng, Yu Gu, Boyuan Zheng, Shijie Chen, Samual Stevens, Boshi Wang, Huan Sun, and Yu Su. 2023. Mind2web: Towards a generalist agent for the web . In Proceedings of NeurIPS . Gou et al. (2025) Boyu Gou, Ruohan Wang, Boyuan Zheng, Yanan Xie, Cheng Chang, Yiheng Shu, Huan Sun, and Yu Su. 2025. Navigating the digital world as humans do: Universal visual grounding for GUI agents . In Proceedings of ICLR . Gur et al. (2024) Izzeddin Gur, Hiroki Furuta, Austin V. Huang, Mustafa Safdari, Yutaka Matsuo, Douglas Eck, and Aleksandra Faust. 2024. A real-world webagent with planning, long context understanding, and program synthesis . In Proceedi…

**Results.** Experiments Multimodal-Mind2Web. Mind2Web-Live. MiniWob++. 5 Results 5.1 In-domain Evaluation 5.2 Mind2Web-Live Results Improvement over base pre-trained models. Improvement over higher capacity pre-trained models. 5.3 Multimodal-Mind2Web Results 5.4 MiniWob++ Results 5.5 Data Scaling Experiments 6 Analyses Diversity Analysis. Analysis of Verifier Accuracy. Failure Modes of Trajectory Generation. 7 Conclusion A Mind2Web Training and Evaluation Details A.1 Mind2Web-Live A.2 Multimodal-Mind2Web A.3 Ablation Studies A.4 Case Studies for Mind2Web-Live B Cost Analysis C Task Complexity Analysis D System Prompts E Trajectory Examples F More Related Work F.1 LLM-based Web Agents F.2 Web Agent Benchmarks and Datasets Explorer: Scaling Exploration-driven Web Trajectory Synthesis for Multimodal Web Agents Vardaan Pahuja 1 ∗† , Yadong Lu 2 1 1 1 Equal Contribution.…

**Conclusion.** Conclusion A Mind2Web Training and Evaluation Details A.1 Mind2Web-Live A.2 Multimodal-Mind2Web A.3 Ablation Studies A.4 Case Studies for Mind2Web-Live B Cost Analysis C Task Complexity Analysis D System Prompts E Trajectory Examples F More Related Work F.1 LLM-based Web Agents F.2 Web Agent Benchmarks and Datasets Explorer: Scaling Exploration-driven Web Trajectory Synthesis for Multimodal Web Agents Vardaan Pahuja 1 ∗† , Yadong Lu 2 1 1 1 Equal Contribution. † † \dagger † Work partly done during internship at Microsoft Research. ¶ ¶ \P ¶ Project Lead. ¶ , Corby Rosset 2 , Boyu Gou 1 , Arindam Mitra 2 , Spencer Whitehead 2 , Yu Su 1 , Ahmed Awadallah 2 1 The Ohio State University 2 Microsoft Rese…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.11357v4.md` · `raw/arxiv/2502.11357v4.fulltext.md`
