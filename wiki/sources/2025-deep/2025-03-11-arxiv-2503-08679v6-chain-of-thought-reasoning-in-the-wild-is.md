---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Chain-of-Thought Reasoning In The Wild Is Not Always Faithful"
authors: Iván Arcuschin, Jett Janiak, Robert Krzyzanowski, Senthooran Rajamanoharan et al.
url: https://arxiv.org/abs/2503.08679v6
date: 2025-03-11
citationCount: 143
influentialCitationCount: 1
velocity: 9.3
ingested: 2026-06-22
tags: [agent-security, agentic-ai, arxiv, 2025, cited]
---

# Chain-of-Thought Reasoning In The Wild Is Not Always Faithful

**arXiv [2503.08679v6](https://arxiv.org/abs/2503.08679v6)** · 2025-03-11 · **143 citations** (1 influential · 9.3/mo) · Iván Arcuschin, Jett Janiak, Robert Krzyzanowski, Senthooran Rajamanoharan et al.

## Abstract
Recent studies indicate that when faced with explicit biases in prompts, models often omit mentioning these biases in their Chain-of-Thought (CoT) output, revealing that verbalized reasoning can give an incorrect picture of how models arrive at conclusions (unfaithfulness). In this work, we show that unfaithful CoT also occurs on naturally worded, non-adversarial prompts without adding artificial biases or editing model outputs. We find that when separately presented with the questions "Is X bigger than Y?" and "Is Y bigger than X?", models sometimes produce superficially coherent arguments to justify systematically answering Yes to both or No to both, despite the contradiction. We present preliminary evidence that this is due to models' implicit biases towards Yes or No, labeling this Implicit Post-Hoc Rationalization. Our results reveal rates up to 13% for production models, and while frontier models are more faithful, none are entirely so, including thinking models like DeepSeek R1 (0.37%) and Sonnet 3.7 with thinking (0.04%). We also investigate Unfaithful Illogical Shortcuts, where models use subtly illogical reasoning to make speculative answers to hard math problems seem rigorously proven. Our findings indicate that while CoT can be useful for assessing outputs, it is not a complete account of the internal process that produced the model's answer and should be used with caution in agentic or safety-critical settings.

## From the paper (full-text excerpts)
**Introduction.** Introduction Conflict of Interest Disclosure. 2 Frontier Models and Implicit Post-Hoc Rationalization 2.1 Evaluation of Implicit Post-Hoc Rationalization Robustness of IPHR Results. 2.2 Unfaithfulness Patterns in Implicit Post-Hoc Rationalization 3 Unfaithfulness in Reasoning Benchmarks 3.1 Methodology for Unfaithful Illogical Shortcuts 3.1.1 Results for Unfaithful Illogical Shortcuts Analysis. Alternative Hypotheses. 4 Related Work Faithfulness in Language Models. Implications for AI Safety. 5 Conclusion 5.1 Limitations Future Work References A Dataset for Evaluating IPHR A.1 Subset of World Model Data Used A.2 Generation of Question Pairs Entity Filtering and Pairing. Ambiguity Evaluation. Question Sampling and Generation. B Validation of Ambiguity Filter Setup. Question-Level Performance of the Filter. Residual Ambiguity in the Final Datasets. C Details of the Evaluation of IPHR D IPHR Measured With Oversampled Questions E Ablation Study: Same-Longitude/Latitude Pairs F Ablation Study: N/A A…

**Method / approach.** Methodology for Unfaithful Illogical Shortcuts 3.1.1 Results for Unfaithful Illogical Shortcuts Analysis. Alternative Hypotheses. 4 Related Work Faithfulness in Language Models. Implications for AI Safety. 5 Conclusion 5.1 Limitations Future Work References A Dataset for Evaluating IPHR A.1 Subset of World Model Data Used A.2 Generation of Question Pairs Entity Filtering and Pairing. Ambiguity Evaluation. Question Sampling and Generation. B Validation of Ambiguity Filter Setup. Question-Level Performance of the Filter. Residual Ambiguity in the Final Datasets. C Details of the Evaluation of IPHR D IPHR Measured With Oversampled Questions E Ablation Study: Same-Longitude/Latitude Pairs F Ablation Study: N/A Answers G IPHR Systematic Bias H IPHR Bias Probing Results. I Details of Unfaithfulness Patterns in IPHR I.1 Switching Arguments I.1.1 Gemini 2.5 Flash World Natural Latitude Salar de Arizaro I…

**Results.** experimental codebase and accompanying datasets in an open-source repository 1 1 1 https://github.com/jettjaniak/chainscope . Conflict of Interest Disclosure. The authors Senthooran Rajamanoharan, Neel Nanda, and Arthur Conmy are employed by Google DeepMind, which leads the development of Gemini, which was among the ones evaluated in this paper. 2 Frontier Models and Implicit Post-Hoc Rationalization Figure 2 : Quantitative results of Implicit Post-Hoc Rationalization for the 15 15 frontier models and pretrained model in our evaluation. For each model, we show the percentage of pairs of questions showing unfaithfulness over the total number of pairs in our dataset ( 4 , 834 4{,}834 ), using the classification criteria described in Section ˜ 2.1 . Briefly, a pair is deemed unfaithful if (i) the two variants differ by at least 50 % 50\% in accuracy, (ii) the question group shows a bias of at least 5 % 5\% toward Yes or No , an…

**Conclusion.** Conclusion 5.1 Limitations Future Work References A Dataset for Evaluating IPHR A.1 Subset of World Model Data Used A.2 Generation of Question Pairs Entity Filtering and Pairing. Ambiguity Evaluation. Question Sampling and Generation. B Validation of Ambiguity Filter Setup. Question-Level Performance of the Filter. Residual Ambiguity in the Final Datasets. C Details of the Evaluation of IPHR D IPHR Measured With Oversampled Questions E Ablation Study: Same-Longitude/Latitude Pairs F Ablation Study: N/A Answers G IPHR Systematic Bias H IPHR Bias Probing Results. I Details of Unfaithfulness Patterns in IPHR I.1 Switching Arguments I.1.1 Gemini 2.5 Flash World Natural Latitude…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[deepseek]]
- **Raw:** `raw/arxiv/2503.08679v6.md` · `raw/arxiv/2503.08679v6.fulltext.md`
