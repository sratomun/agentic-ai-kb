---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SealQA: Raising the Bar for Reasoning in Search-Augmented Language Models"
authors: Thinh Pham, Nguyen Nguyen, Pratibha Zunjare, Weiyuan Chen et al.
url: https://arxiv.org/abs/2506.01062v4
date: 2025-06-01
citationCount: 50
influentialCitationCount: 9
velocity: 3.94
ingested: 2026-06-22
tags: [agent-reliability, agent-security, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# SealQA: Raising the Bar for Reasoning in Search-Augmented Language Models

**arXiv [2506.01062v4](https://arxiv.org/abs/2506.01062v4)** · 2025-06-01 · **50 citations** (9 influential · 3.94/mo) · Thinh Pham, Nguyen Nguyen, Pratibha Zunjare, Weiyuan Chen et al.

## Abstract
We introduce SealQA, a new challenge benchmark for evaluating SEarch-Augmented Language models on fact-seeking questions where web search yields conflicting, noisy, or unhelpful results. SealQA comes in three flavors: (1) Seal-0 (main) and (2) Seal-Hard, which assess factual accuracy and reasoning capabilities, with Seal-0 focusing on the most challenging questions where chat models (e.g., GPT-4.1) typically achieve near-zero accuracy; and (3) LongSeal, which extends SealQA to test long-context, multi-document reasoning in "needle-in-a-haystack" settings. Our evaluation reveals critical limitations in current models: Even frontier LLMs perform poorly across all SealQA flavors. On Seal-0, frontier agentic models equipped with tools like o3 and o4-mini achieve only 17.1% and 6.3% accuracy, respectively, at their best reasoning efforts. We find that advanced reasoning models such as DeepSeek-R1-671B and o3-mini are highly vulnerable to noisy search results. Notably, increasing test-time compute does not yield reliable gains across o3-mini, o4-mini, and o3, with performance often plateauing or even declining early. Additionally, while recent models are less affected by the "lost-in-the-middle" issue, they still fail to reliably identify relevant documents in LongSeal when faced with numerous distractors. To facilitate future work, we release SealQA at huggingface.co/datasets/vtllms/sealqa.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Data collection Human annotators: Question types: Annotation criteria: Quality control: Diversity: Curation of SealQA flavors: Evaluation protocol: Auto-rater reliability: 3 Experiments 3.1 Experiment setup 3.1.1 Seal-0 and Seal-Hard Baselines: Human competitors: 3.1.2 LongSeal 3.2 Results on Seal-0 and Seal-Hard Naive search and integration can amplify noise rather than improve accuracy: Advanced reasoning models can be highly vulnerable to noisy search results: Test-time scaling does not lead to reliable gains on SealQA : The effect of repeated sampling: SealQA requires careful search and robust reasoning: 3.3 Results on LongSeal Frontier LLMs struggle on LongSeal with increased distractors: Absence of classic positional bias in Liu et al. ( 2024 ) : 4 Related work Reasoning under knowledge conflict: Measuring factuality and reasoning in LLMs : 5 Conclusion References A Additional test-time scaling results on SealQA B Sample SealQA questions C Template for GPT-4o mini auto-rater D…

**Method / approach.** methods like FreshPrompt . While GPT-4.1 gains a performance boost from built-in search (+5.5%), FreshPrompt slightly reduces its accuracy (15.0% → \rightarrow 14.6%). Built-in search generally improves performance on Seal-Hard for both GPT-4.0 and GPT-4.1 . With that said, FreshPrompt remains useful for most open-weight models without tool-use training. For example, Qwen3-235B-A22B and DeepSeek-R1-Distill-Qwen-14B achieve gains of +7.1% and +9.7%, respectively, on Seal-Hard when using FreshPrompt . However, search can sometimes be detrimental. GPT-4.1-mini , when equipped with built-in search, drops in accuracy from 13.8% to 11.8%. Since SealQA questions are designed to elicit conflicting or noisy search results, naive retrieval and integration can harm model accuracy. Figure 4: Advanced reasoning models such as DeepSeek-R1-671B and o3-mini are highly vulnerable to noisy search results. Advanced reasoning models can be highly vulnerable to noisy search results: As shown…

**Results.** Experiments 3.1 Experiment setup 3.1.1 Seal-0 and Seal-Hard Baselines: Human competitors: 3.1.2 LongSeal 3.2 Results on Seal-0 and Seal-Hard Naive search and integration can amplify noise rather than improve accuracy: Advanced reasoning models can be highly vulnerable to noisy search results: Test-time scaling does not lead to reliable gains on SealQA : The effect of repeated sampling: SealQA requires careful search and robust reasoning: 3.3 Results on LongSeal Frontier LLMs struggle on LongSeal with increased distractors: Absence of classic positional bias in Liu et al. ( 2024 ) : 4 Related work Reasoning under knowledge conflict: Measuring factuality and reasoning in LLMs : 5 Conclusion References A Additional test-time scaling results on SealQA B Sample SealQA questions C Template for GPT-4o mini auto-rater D Seal-Hard results by question category E Seal-Hard results by…

**Conclusion.** Conclusion References A Additional test-time scaling results on SealQA B Sample SealQA questions C Template for GPT-4o mini auto-rater D Seal-Hard results by question category E Seal-Hard results by answer type F Human performance G Qualitative analysis H Sample model outputs I Additional Seal-0 results License: arXiv.org perpetual non-exclusive license arXiv:2506.01062v4 [cs.CL] 09 Apr 2026 SealQA : Raising the Bar for Reasoning in Search-Augmented Language Models Thinh Pham Nguyen Nguyen Pratibha Zunjare Weiyuan Chen Yu-Min Tseng Tu Vu Virginia Tech {thinhphp,tuvu}@vt.edu Abstract We introduce SealQA , a challenge benchmark for evaluating SE arch- A ugmented L anguage models on…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[deepseek]]
- **Raw:** `raw/arxiv/2506.01062v4.md` · `raw/arxiv/2506.01062v4.fulltext.md`
