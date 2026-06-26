---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "OctoTools: An Agentic Framework with Extensible Tools for Complex Reasoning"
authors: Pan Lu, Bowen Chen, Sheng Liu, Rahul Thapa et al.
url: https://arxiv.org/abs/2502.11271v2
date: 2025-02-16
citationCount: 65
influentialCitationCount: 7
velocity: 4.03
ingested: 2026-06-22
tags: [agent-reliability, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# OctoTools: An Agentic Framework with Extensible Tools for Complex Reasoning

**arXiv [2502.11271v2](https://arxiv.org/abs/2502.11271v2)** · 2025-02-16 · **65 citations** (7 influential · 4.03/mo) · Pan Lu, Bowen Chen, Sheng Liu, Rahul Thapa et al.

## Abstract
Solving complex reasoning tasks may involve visual understanding, domain knowledge retrieval, numerical calculation, and multi-step reasoning. Existing methods augment large language models (LLMs) with external tools but are restricted to specialized domains, limited tool types, or require additional training data. In this paper, we introduce OctoTools, a training-free, user-friendly, and easily extensible multi-agent framework designed to tackle complex reasoning across diverse domains. OctoTools introduces standardized tool cards to encapsulate tool functionality, a planner for both high-level and low-level planning, and an executor to carry out tool usage. We validate OctoTools' generality across 16 diverse tasks (including MathVista, MMLU-Pro, MedQA, and GAIA-Text), achieving substantial average accuracy gains of 9.3% over GPT-4o. Furthermore, OctoTools also outperforms AutoGen, GPT-Functions, and LangChain by up to 10.6% when given the same set of tools. Through comprehensive analysi, ablations, and robustness tests with compact backbones and noisy tool environments, OctoTools demonstrates advantages in task planning, effective tool usage, and multi-step problem solving. Code, demos, and visualization are publicly available at https://octotools.github.io/.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large language models (LLMs) (Brown et al., 2020; Chowdhery et al., 2022; OpenAI, 2023b) have made rapid progress on tasks such as summarization, translation (Thoppilan et al., 2022), code generation (Nakano et al., 2021), and math problem solving (Shuster et al., 2022). However, complex reasoning tasks that involve multiple steps, logical decomposition, or specialized domain knowledge remain challenging. For example, solving a visual riddle may require fine-grained image understanding and text-based reasoning, while a math or chemistry question can require thorough computations or domain expertise. Existing prompting methods often fail to orchestrate these varied processes into a coherent chain of reasoning (Yao et al., 2022). A promising direction to address these challenges is Average Accuracy on 16 Tasks (%) Pan Lu∗ , Bowen Chen∗ , Sheng Liu∗ , Rahul Thapa , Joseph Boen , James Zou * Equal contribution Stanford University Website: https://octotools.github.io Code Demo Tool Cards Visualization Video 60 58.5 55 50 49.2 51.0 50.8 51.2 47.9 45 40 en ols ain -…

**Method / approach.** methods augment large language models (LLMs) with external tools but are restricted to specialized domains, limited tool types, or require additional training data. In this paper, we introduce OctoTools, a training-free, user-friendly, and easily extensible multi-agent framework designed to tackle complex reasoning across diverse domains. OctoTools introduces standardized tool cards to encapsulate tool functionality, a planner for both high-level and low-level planning, and an executor to carry out tool usage. We validate OctoTools’ generality across 16 diverse tasks (including MathVista, MMLU-Pro, MedQA, and GAIAText), achieving substantial average accuracy gains of 9.3% over GPT-4o. Furthermore, OctoTools also outperforms AutoGen, GPT-Functions, and LangChain by up to 10.6% when given the same set of tools. Through comprehensive analysi, ablations, and robustness tests with compact backbones and noisy tool environments, OctoTools demonstrates advantages in task planning, effective t…

**Results.** experiments across 16 reasoning benchmarks spanning vision, mathematical, scientific, medical, and agentic domains. As shown in Figure 1, OctoTools substantially outperforms baselines, with an average accuracy gain of 9.3% over zero-shot prompting by GPT-4o and 7.7% over chainof-thought (CoT), as well as up to 10.6% improvement over existing agentic frameworks with the same tools (AutoGen, 2024; OpenAI, 2023a; LangChain, 2024). Analyses show that OctoTools effectively combines multi-step planning and specialized tool usage, with each providing distinct improvements. Tool usage is particularly valuable for intricate calculations or specialized knowledge, while multi-step planning offers significant gains for reasoning decomposition. Furthermore, our comprehensive studies provide insights into OctoTools’s performance and robustness under different conditions. Accuracy increases with higher step budgets, highlighting the value of longer mu…

**Conclusion.** Conclusion: CONTINUE Step 1: Command Executor The image shows four blue buckets, each containing five baseballs. Each bucket has a handle on the side. Step 1: Context Verifier Completeness: Context provides a description of the image. Inconsistencies: There are no inconsistencies. Verification: Given limitations of Image Captioner Tool in counting, verify the count using Object Detector Tool. Ambiguities: There are no ambiguities. Conclusion: CONTINUE Step 2: 2: Command Action Predictor Step Executor Input (label): ["baseball"] Output (detected objects): OctoTools: An Agentic Framework with Extensible Tools for Complex "label": "baseball", Detector Tool: Example 1 Sub-goal: Detect and count the number ofObject baseballs. "confidence…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2502.11271v2.md` · `raw/arxiv/2502.11271v2.fulltext.md`
