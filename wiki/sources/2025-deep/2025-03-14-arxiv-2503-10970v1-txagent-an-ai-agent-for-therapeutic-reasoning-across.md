---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "TxAgent: An AI Agent for Therapeutic Reasoning Across a Universe of Tools"
authors: Shanghua Gao, Richard Zhu, Zhenglun Kong, Ayush Noori et al.
url: https://arxiv.org/abs/2503.10970v1
date: 2025-03-14
citationCount: 71
influentialCitationCount: 5
velocity: 4.65
ingested: 2026-06-22
tags: [recommendation-agents, clinical-agents, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# TxAgent: An AI Agent for Therapeutic Reasoning Across a Universe of Tools

**arXiv [2503.10970v1](https://arxiv.org/abs/2503.10970v1)** · 2025-03-14 · **71 citations** (5 influential · 4.65/mo) · Shanghua Gao, Richard Zhu, Zhenglun Kong, Ayush Noori et al.

## Abstract
Precision therapeutics require multimodal adaptive models that generate personalized treatment recommendations. We introduce TxAgent, an AI agent that leverages multi-step reasoning and real-time biomedical knowledge retrieval across a toolbox of 211 tools to analyze drug interactions, contraindications, and patient-specific treatment strategies. TxAgent evaluates how drugs interact at molecular, pharmacokinetic, and clinical levels, identifies contraindications based on patient comorbidities and concurrent medications, and tailors treatment strategies to individual patient characteristics. It retrieves and synthesizes evidence from multiple biomedical sources, assesses interactions between drugs and patient conditions, and refines treatment recommendations through iterative reasoning. It selects tools based on task objectives and executes structured function calls to solve therapeutic tasks that require clinical reasoning and cross-source validation. The ToolUniverse consolidates 211 tools from trusted sources, including all US FDA-approved drugs since 1939 and validated clinical insights from Open Targets. TxAgent outperforms leading LLMs, tool-use models, and reasoning agents across five new benchmarks: DrugPC, BrandPC, GenericPC, TreatmentPC, and DescriptionPC, covering 3,168 drug reasoning tasks and 456 personalized treatment scenarios. It achieves 92.1% accuracy in open-ended drug reasoning tasks, surpassing GPT-4o and outperforming DeepSeek-R1 (671B) in structured multi-step reasoning. TxAgent generalizes across drug name variants and descriptions. By integrating multi-step inference, real-time knowledge grounding, and tool-assisted decision-making, TxAgent ensures that treatment recommendations align with established clinical guidelines and real-world evidence, reducing the risk of adverse events and improving therapeutic decision-making.

## From the paper (full-text excerpts)
**Method / approach.** methods [ 24 , 25 ] . Many models exhibit high variance when drugs are referenced by brand names, generic names, or detailed descriptions [ 24 ] . In contrast, TxAgent achieves an exceptionally low accuracy variance of 0.01 across these variations, whereas GPT-4o exhibits a variance of 9.96, indicating a much higher sensitivity to representation shifts. On DescriptionPC, a benchmark that evaluates drug reasoning when drug names are replaced with descriptive narratives, TxAgent attains 56.5% accuracy, outperforming GPT-4o by 8.3% and indicating TxAgent ’s robustness to infer drug identities from contextual clues. TxAgent also excels in personalized treatment recommendations, where it evaluates patient-specific drug selection. On TreatmentPC, which assesses 456 real-world treatment scenarios, TxAgent outperforms GPT-4o by 13.6% and Llama-3.1-70B-Instruct by 25.4% in the open-ended setting, establishing its superiority in personalized medicine. Compared to DeepSeek-R1 [ 26 ] , a 671-b…

**Results.** experiments. First, we assess the impact of thought generation by removing this process. Second, we examine how the number of reasoning steps in training data affects performance by limiting the maximum reasoning traces. Finally, we evaluate the influence of reasoning during inference by imposing a step limit, forcing TxAgent to generate a final answer after a predefined number of steps. Explicit thought generation drives reasoning in TxAgent . We evaluate the impact of thought generation by comparing TxAgent with and without this process on the DrugPC and TreatmentPC benchmarks, using accuracy as the metric (Figure 3 e). Unlike existing tool-use LLMs that generate only function calls, TxAgent produces both reasoning thoughts and function calls at each step. To assess the importance of thought generation, we modify TxAgent to generate only function calls without intermediate reasoning. At the final step, it directly outputs the ans…

**Conclusion.** conclusions. TxAgent also surpasses distilled variants, including DeepSeek-R1-Llama-8B/70B, which are trained on Llama-3.1-8B and Llama-3.1-70B. Against DeepSeek-R1-Llama-8B, which shares the same base model as TxAgent , TxAgent achieves accuracy gains of 36.1% in multiple-choice and 34.9% in open-ended tasks. Unlike reasoning LLMs that rely solely on internal knowledge, TxAgent integrates multi-step reasoning with verified external information from ToolUniverse , making it more effective for specialized treatment recommendation tasks. Examples of TxAgent reasoning traces for specialized treatments We present detailed TxAgent reasoning traces for four personalized treatment questions, evaluating its ability to incorporate drug mec…

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[clinical-agents|Clinical agents]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gpt-5]] · [[deepseek]]
- **Raw:** `raw/arxiv/2503.10970v1.md` · `raw/arxiv/2503.10970v1.fulltext.md`
