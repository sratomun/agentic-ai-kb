---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The Danger of Overthinking: Examining the Reasoning-Action Dilemma in Agentic Tasks"
authors: Alejandro Cuadron, Dacheng Li, Wenjie Ma, Xingyao Wang et al.
url: https://arxiv.org/abs/2502.08235v1
date: 2025-02-12
citationCount: 143
influentialCitationCount: 6
velocity: 8.79
ingested: 2026-06-22
tags: [coding-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# The Danger of Overthinking: Examining the Reasoning-Action Dilemma in Agentic Tasks

**arXiv [2502.08235v1](https://arxiv.org/abs/2502.08235v1)** · 2025-02-12 · **143 citations** (6 influential · 8.79/mo) · Alejandro Cuadron, Dacheng Li, Wenjie Ma, Xingyao Wang et al.

## Abstract
Large Reasoning Models (LRMs) represent a breakthrough in AI problem-solving capabilities, but their effectiveness in interactive environments can be limited. This paper introduces and analyzes overthinking in LRMs. A phenomenon where models favor extended internal reasoning chains over environmental interaction. Through experiments on software engineering tasks using SWE Bench Verified, we observe three recurring patterns: Analysis Paralysis, Rogue Actions, and Premature Disengagement. We propose a framework to study these behaviors, which correlates with human expert assessments, and analyze 4018 trajectories. We observe that higher overthinking scores correlate with decreased performance, with reasoning models exhibiting stronger tendencies toward overthinking compared to non-reasoning models. Our analysis reveals that simple efforts to mitigate overthinking in agentic environments, such as selecting the solution with the lower overthinking score, can improve model performance by almost 30% while reducing computational costs by 43%. These results suggest that mitigating overthinking has strong practical implications. We suggest that by leveraging native function-calling capabilities and selective reinforcement learning overthinking tendencies could be mitigated. We also open-source our evaluation framework and dataset to facilitate research in this direction at https://github.com/AlexCuadron/Overthinking.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large Reasoning Models (LRMs) (Guan et al., 2025; Xu et al., 2025), such as OpenAI’s o1 (OpenAI, 2024e), Alibaba’s QwQ (Qwen, 2024b), or Deepseek’s R1 (Guo et al., 2025) represent a breakthrough in large language models (LLMs). These advanced systems have fundamentally redefined AI’s problem-solving capabilities across various domains (Besta et al., 2025). In particular, LRM’s selfcorrection abilities enable them to achieve impressive scores in several benchmarks, such as AIME 2024 (AoPS, 2024), MMLU (Hendrycks et al., 2021), or GPQA-Diamond (Rein et al., 2023) among others (Guo et al., 2025; OpenAI, 2024e;d; Qwen, 2024b; Guan et al., 2025). 1 Department of EECS, University of California, Berkeley, USA Department of Computer Science, ETH, Zurich, Switzerland 3 Department of Computer Science, University of Illinois UrbanaChampaign, USA 4 Department of Computer Science, Carnegie Mellon University, USA. Correspondence to: Alejandro Cuadron <acuadron@berkeley.edu>. 2 Despite extensive analysis of LRMs in non-agentic environ1 The Danger of Overthinking: Examining the Reas…

**Method / approach.** method using an LLMbased evaluator. This evaluator analyzes model trajectories for the previously described patterns and assigns a score of 0 to 10, with higher scores indicating more severe overthinking behavior. Each score includes a detailed justification explaining which patterns were identified and their severity. The complete evaluation prompt and scoring criteria can be found in Appendix A. Analysis Paralysis LRMs tend to shift their focus from immediate actions to elaborate future planning. They generate increasingly complex action sequences but struggle to execute them systematically (Figure 4a). Rather than addressing immediate errors, they construct intricate plans that often remain unexecuted, leading to a cycle of planning without progress. To validate our LLM-based evaluator, we conduct an independent assessment where four expert annotators manually scored 20 randomly selected model traces, as shown in Figure 5. Using these standardized scores, we conduct a comprehensi…

**Results.** experiments on software engineering tasks using SWE Bench Verified, we observe three recurring patterns: Analysis Paralysis, Rogue Actions, and Premature Disengagement. We propose a framework to study these behaviors, which correlates with human expert assessments, and analyze 4018 trajectories. We observe that higher overthinking scores correlate with decreased performance, with reasoning models exhibiting stronger tendencies toward overthinking compared to non-reasoning models. Our analysis reveals that simple efforts to mitigate overthinking in agentic environments — such as selecting the solution with the lower overthinking score — can improve model performance by almost 30% while reducing computational costs by 43%. These results suggest that mitigating overthinking has strong practical implications. We suggest that by leveraging native function-calling capabilities and selective reinforcement learning overthinking tendencies could…

**Conclusion.** Conclusion 6. Discussion In this work, we present the first comprehensive empirical study of Large Reasoning Models (LRMs) in agentic environments. We identify a fundamental challenge: the Reasoning-Action Dilemma, in which models must balance environmental engagement against internal reasoning about potential actions and their hypothetical consequences. Our analysis reveals that LRMs consistently favor internal 6.1. Can native function calling affect overthinking? Our experimental analysis compares o1 model configurations with high reasoning effort, evaluating performance both with and without native function calling (FC) capabilities. The integration of FC capabilities yields substantial improvements, increasing the performance score f…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2502.08235v1.md` · `raw/arxiv/2502.08235v1.fulltext.md`
