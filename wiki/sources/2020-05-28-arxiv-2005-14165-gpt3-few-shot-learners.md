---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Language Models are Few-Shot Learners"
authors: Tom B. Brown et al.
url: https://arxiv.org/abs/2005.14165
date: 2020-05-28
citationCount: omit
tags: [arxiv, pretraining]
---

# Language Models are Few-Shot Learners

**arXiv [2005.14165](https://arxiv.org/abs/2005.14165)** · 2020-05-28 · Tom B. Brown et al. (OpenAI)

**Significance.** Introduced GPT-3 (175B params) and showed that scale alone unlocks task-agnostic few-shot in-context learning with no gradient updates.

## Abstract
Recent work has demonstrated substantial gains on many NLP tasks and benchmarks by pre-training on a large corpus of text followed by fine-tuning on a specific task. While typically task-agnostic in architecture, this method still requires task-specific fine-tuning datasets of thousands or tens of thousands of examples. By contrast, humans can generally perform a new language task from only a few examples or from simple instructions – something which current NLP systems still largely struggle to do. Here we show that scaling up language models greatly improves task-agnostic, few-shot performance, sometimes even reaching competitiveness with prior state-of-the-art fine-tuning approaches. Specifically, we train GPT-3, an autoregressive language model with 175 billion parameters, 10x more than any previous non-sparse language model, and test its performance in the few-shot setting. For all tasks, GPT-3 is applied without any gradient updates or fine-tuning, with tasks and few-shot demonstrations specified purely via text interaction with the model. GPT-3 achieves strong performance on many NLP datasets, including translation, question-answering, and cloze tasks, as well as several tasks that require on-the-fly reasoning or domain adaptation, such as unscrambling words, using a novel word in a sentence, or performing 3-digit arithmetic. At the same time, we also identify some datasets where GPT-3's few-shot learning still struggles, as well as some datasets where GPT-3 faces methodological issues related to training on large web corpora. Finally, we find that GPT-3 can generate samples of news articles which human evaluators have difficulty distinguishing from articles written by humans. We discuss broader societal impacts of this finding and of GPT-3 in general.

## From the paper (full-text)
**Contribution / method.** Train an autoregressive transformer LM with 175 billion parameters (10x larger than any prior non-sparse model) and evaluate it purely via in-context learning — zero-shot, one-shot, and few-shot — with no gradient updates or fine-tuning. Training corpus: 41 monthly shards of Common Crawl 2016–2019, 45TB compressed plaintext before filtering and 570GB after filtering (~400 billion BPE tokens), blended with curated higher-quality datasets. All models trained for a total of 300 billion tokens.

**Results.** Few-shot scales faster than zero-shot as model size grows. TriviaQA: 64.3% (zero-shot), 68.0% (one-shot), 71.2% (few-shot) — the last state-of-the-art. Reaches 85.0 F1 few-shot on a reading-comprehension/QA task. Performs 3-digit arithmetic, word unscrambling, and novel-word use in-context. Human evaluators struggle to distinguish GPT-3-generated news articles from human-written ones. Authors flag datasets where few-shot still struggles and benchmark-contamination concerns from web-scale training.

**Takeaway.** Sheer scale converts a language model into a general-purpose few-shot learner — capability emerges from pretraining size, not task-specific fine-tuning.

## Graph
- **Concepts:** [[pretraining|Pre-training]]
- **Entities:** GPT-3, OpenAI, Common Crawl
- **Raw:** `raw/arxiv/2005.14165.fulltext.md`
