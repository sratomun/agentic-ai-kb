---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Neural Machine Translation of Rare Words with Subword Units"
authors: Rico Sennrich et al.
url: https://arxiv.org/abs/1508.07909
date: 2015-08-31
ingested: 2026-06-22
tags: [arxiv, tokenization, data]
---

# Neural Machine Translation of Rare Words with Subword Units

**arXiv [1508.07909](https://arxiv.org/abs/1508.07909)** · 2015-08-31 (v5 2016-06-10) · Rico Sennrich, Barry Haddow, Alexandra Birch (University of Edinburgh)

**Significance.** The paper that brought byte pair encoding (BPE) to NLP — the subword tokenization scheme that nearly every modern LLM tokenizer descends from. Solved open-vocabulary translation with a fixed-size vocabulary and no back-off dictionary.

## Abstract
Neural machine translation (NMT) models typically operate with a fixed vocabulary, but translation is an open-vocabulary problem. Previous work addresses the translation of out-of-vocabulary words by backing off to a dictionary. In this paper, we introduce a simpler and more effective approach, making the NMT model capable of open-vocabulary translation by encoding rare and unknown words as sequences of subword units. This is based on the intuition that various word classes are translatable via smaller units than words, for instance names (via character copying or transliteration), compounds (via compositional translation), and cognates and loanwords (via phonological and morphological transformations). We discuss the suitability of different word segmentation techniques, including simple character n-gram models and a segmentation based on the byte pair encoding compression algorithm, and empirically show that subword models improve over a back-off dictionary baseline for the WMT 15 translation tasks English→German and English→Russian by up to 1.1 and 1.3 BLEU, respectively.

## From the paper (full-text)
**Contribution / method.** Adapts byte pair encoding (Gage, 1994) — a data-compression algorithm — to word segmentation. Initialize the symbol vocabulary with the character vocabulary; represent each word as a character sequence plus an end-of-word marker; then iteratively count all symbol pairs and merge the most frequent pair ('A','B') into a new symbol 'AB'. Final vocabulary size = initial character vocabulary + number of merge operations, which is the algorithm's only hyperparameter. The authors evaluate independent source/target BPE vs. joint BPE (learned on the union of both vocabularies) to improve cross-lingual segmentation consistency; for EN→RU they transliterate Russian to Latin (ISO-9) to learn joint merges, then map back to Cyrillic.

**Results.** On WMT15 newstest2015 (8-model ensembles, English→German): the WDict back-off-dictionary baseline scored 24.2 BLEU; joint BPE (BPE-J90k) reached 24.7 BLEU / 54.1 CHRF3, and char-bigram C2-50k hit the best BLEU at 25.3. Rare-word unigram F1 rose from 36.8% (WDict) to 41.8% (BPE-J90k). For English→Russian, where alphabets differ and copying OOVs fails, BPE-J90k improved 1.3 BLEU and 2.0 CHRF3 over WDict and lifted OOV unigram F1 from 6.6% to 18.3%. Corpus statistics: BPE compresses the German training corpus to a 63,000-type vocabulary (vs. 1.75M unsegmented types) with zero unknown tokens in the dev set.

**Takeaway.** A fixed-size subword vocabulary built by greedy frequency-based merges gives genuinely open-vocabulary models — simpler and more effective than large vocabularies plus back-off dictionaries — and reducing the vocabulary can even improve performance.

## Graph
- **Concepts:** [[tokenization]]
- **Raw:** `raw/arxiv/1508.07909.fulltext.md`
