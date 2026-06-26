---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search"
authors: Yutaro Yamada, Robert Tjarko Lange, Cong Lu, Shengran Hu et al.
url: https://arxiv.org/abs/2504.08066v1
date: 2025-04-10
citationCount: 269
influentialCitationCount: 21
velocity: 18.69
ingested: 2026-06-22
tags: [science-agents, agent-security, agentic-ai, arxiv, 2025, cited]
---

# The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search

**arXiv [2504.08066v1](https://arxiv.org/abs/2504.08066v1)** · 2025-04-10 · **269 citations** (21 influential · 18.69/mo) · Yutaro Yamada, Robert Tjarko Lange, Cong Lu, Shengran Hu et al.

## Abstract
AI is increasingly playing a pivotal role in transforming how scientific discoveries are made. We introduce The AI Scientist-v2, an end-to-end agentic system capable of producing the first entirely AI generated peer-review-accepted workshop paper. This system iteratively formulates scientific hypotheses, designs and executes experiments, analyzes and visualizes data, and autonomously authors scientific manuscripts. Compared to its predecessor (v1, Lu et al., 2024 arXiv:2408.06292), The AI Scientist-v2 eliminates the reliance on human-authored code templates, generalizes effectively across diverse machine learning domains, and leverages a novel progressive agentic tree-search methodology managed by a dedicated experiment manager agent. Additionally, we enhance the AI reviewer component by integrating a Vision-Language Model (VLM) feedback loop for iterative refinement of content and aesthetics of the figures. We evaluated The AI Scientist-v2 by submitting three fully autonomous manuscripts to a peer-reviewed ICLR workshop. Notably, one manuscript achieved high enough scores to exceed the average human acceptance threshold, marking the first instance of a fully AI-generated paper successfully navigating a peer review. This accomplishment highlights the growing capability of AI in conducting all aspects of scientific research. We anticipate that further advancements in autonomous scientific discovery technologies will profoundly impact human knowledge generation, enabling unprecedented scalability in research productivity and significantly accelerating scientific breakthroughs, greatly benefiting society at large. We have open-sourced the code at https://github.com/SakanaAI/AI-Scientist-v2 to foster the future development of this transformative technology. We also discuss the role of AI in science, including AI safety.

## From the paper (full-text excerpts)
**Introduction.** Introduction Automated scientific discovery empowered by artificial intelligence (AI) has garnered considerable attention in recent years (Cornelio et al., 2023; Gil et al., 2014; King et al., 2009; Kitano, 2021; Wang et al., 2023; Xu et al., 2021). The development of end-to-end frameworks capable of autonomously formulating hypotheses, performing experiments, analyzing results, and authoring manuscripts could fundamentally transform the scientific process. A notable recent advance in this direction is The AI Scientist-v1 (Lu et al., 2024), which demonstrated the feasibility of a fully automated scientific workflow and downstream manuscript production. However, significant limitations constrained its broad applicability and autonomy. Specifically, it relied heavily on human-authored code templates requiring manual effort to create a new template for each new topic area. Furthermore, its linear and shallow experimentation approach prevented deeper exploration of scientific hypotheses. In this paper, we introduce The AI Scientist-v2, a substantially improved successor that directly add…

**Method / approach.** methodology managed by a dedicated experiment manager agent. Additionally, we enhance the AI reviewer component by integrating a Vision-Language Model (VLM) feedback loop for iterative refinement of content and aesthetics of the figures. We evaluated Th e A I Sc i e n t i s t - v 2 by submitting three fully autonomous manuscripts to a peer-reviewed ICLR workshop. Notably, one manuscript achieved high enough scores to exceed the average human acceptance threshold, marking the first instance of a fully AI-generated paper successfully navigating a peer review. This accomplishment highlights the growing capability of AI in conducting all aspects of scientific research. We anticipate that further advancements in autonomous scientific discovery technologies will profoundly impact human knowledge generation, enabling unprecedented scalability in research productivity and significantly accelerating scientific breakthroughs, greatly benefiting society at large. We have open-sourced the code at…

**Results.** experiments, analyzes and visualizes data, and autonomously authors scientific manuscripts. Compared to its predecessor (v1, Lu et al., 2024), The AI Scientist-v2 eliminates the reliance on human-authored code templates, generalizes effectively across diverse machine learning domains, and leverages a novel progressive agentic tree-search methodology managed by a dedicated experiment manager agent. Additionally, we enhance the AI reviewer component by integrating a Vision-Language Model (VLM) feedback loop for iterative refinement of content and aesthetics of the figures. We evaluated Th e A I Sc i e n t i s t - v 2 by submitting three fully autonomous manuscripts to a peer-reviewed ICLR workshop. Notably, one manuscript achieved high enough scores to exceed the average human acceptance threshold, marking the first instance of a fully AI-generated paper successfully navigating a peer review. This accomplishment highlights the growing cap…

**Conclusion.** conclusion of each stage. These repeated runs provide statistics (mean and standard deviation) for figures and reported results. 3.2.2. Parallelized Agentic Tree Search Th e A I Sc i e n t i s t - v 1 operated strictly linearly, where each code refinement directly built on the immediately preceding experiment. In contrast, The AI Scientist-v2 adopts a significantly more flexible and exploratory approach inspired by recent successes in integrating tree search with LLM-driven workflows (Chan et al., 2025; Jiang et al., 2025; Wijk et al., 2024) and research on openendedness (Clune, 2019; Mouret and Clune, 2015). We incorporate this agentic tree search approach across all four experimentation stages outlined in §3.2.1, enabling deeper and more…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.08066v1.md` · `raw/arxiv/2504.08066v1.fulltext.md`
