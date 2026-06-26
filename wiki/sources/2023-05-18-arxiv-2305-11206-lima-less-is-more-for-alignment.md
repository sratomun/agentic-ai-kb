---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "LIMA: Less Is More for Alignment"
authors: Chunting Zhou et al.
url: https://arxiv.org/abs/2305.11206
date: 2023-05-18
ingested: 2026-06-22
tags: [arxiv, sft, post-training]
---

# LIMA: Less Is More for Alignment

**arXiv [2305.11206](https://arxiv.org/abs/2305.11206)** · 2023-05-18 · Chunting Zhou, Pengfei Liu, Puxin Xu, Srini Iyer, Jiao Sun, Yuning Mao, Xuezhe Ma, Avia Efrat, Ping Yu, Lili Yu, Susan Zhang, Gargi Ghosh, Mike Lewis, Luke Zettlemoyer, Omer Levy (Meta AI / CMU / USC / Tel Aviv University)

**Significance.** The "less is more" result: plain supervised fine-tuning on just 1,000 curated examples — no RLHF, no preference modeling — makes a 65B model competitive with RLHF-trained frontier systems. The empirical case that alignment is mostly surfacing pretraining knowledge, not teaching it.

## Abstract
Large language models are trained in two stages: (1) unsupervised pretraining from raw text, to learn general-purpose representations, and (2) large scale instruction tuning and reinforcement learning, to better align to end tasks and user preferences. We measure the relative importance of these two stages by training LIMA, a 65B parameter LLaMa language model fine-tuned with the standard supervised loss on only 1,000 carefully curated prompts and responses, without any reinforcement learning or human preference modeling. LIMA demonstrates remarkably strong performance, learning to follow specific response formats from only a handful of examples in the training data, including complex queries that range from planning trip itineraries to speculating about alternate history. Moreover, the model tends to generalize well to unseen tasks that did not appear in the training data. In a controlled human study, responses from LIMA are either equivalent or strictly preferred to GPT-4 in 43% of cases; this statistic is as high as 58% when compared to Bard and 65% versus DaVinci003, which was trained with human feedback. Taken together, these results strongly suggest that almost all knowledge in large language models is learned during pretraining, and only limited instruction tuning data is necessary to teach models to produce high quality output.

## From the paper (full-text)
**Contribution / method.** LIMA is a pretrained 65B-parameter LLaMa fine-tuned with the standard supervised loss on only 1,000 curated prompt–response demonstrations (~750k tokens), with no RLHF and no preference modeling. The 1,000 examples are 750 curated from community forums plus 250 manually authored by the authors: Stack Exchange STEM (200), Stack Exchange Other (200), wikiHow (200), Reddit r/WritingPrompts (150), Natural Instructions (50), and author-written (200), selected for quality and task diversity with a uniform AI-assistant response style. The paper frames this with the **Superficial Alignment Hypothesis**: "A model's knowledge and capabilities are learnt almost entirely during pretraining, while alignment teaches it which subdistribution of formats should be used when interacting with users."

**Results.** In the controlled human preference study, LIMA gives equal-or-preferable responses vs GPT-4 in 43%, vs Claude in 46%, and vs Bard in 58% of cases; the abstract frames it as equivalent-or-strictly-preferred to GPT-4 in 43%, Bard in 58%, and the RLHF-trained DaVinci003 in 65% of cases. LIMA also outperforms a 65B Alpaca reproduction trained on 52,000 examples. In the absolute quality study (50 random examples scored Fail/Pass/Excellent), 50% are rated Excellent, 38% Pass, 12% Fail — 88% meet the prompt requirements. Ablations (7B LLaMa, GPT-3.5-graded on a 1–6 Likert scale) show data quality and diversity dominate: filtered vs unfiltered Stack Exchange data gives a ~0.5-point gain, diverse data beats homogeneous wikiHow data, while doubling training quantity yields no improvement. Adding just 30 hand-crafted multi-turn dialogue chains (trained on 1,030 examples total) lifts Excellent-rated dialogue turns from 45.2% to 76.1% and cuts failures from 15-per-42-turns to 1-per-46.

**Takeaway.** Almost all of an LLM's capability comes from pretraining; a tiny, high-quality, diverse SFT set — and a handful of dialogue examples — is enough to align it, no RLHF required. Data quality and diversity matter far more than quantity.

## Graph
- **Concepts:** [[sft|SFT]]
- **Entities:** [[rlhf]] · [[meta-ai|Meta]] · [[llama]]
- **Raw:** `raw/arxiv/2305.11206.fulltext.md`
