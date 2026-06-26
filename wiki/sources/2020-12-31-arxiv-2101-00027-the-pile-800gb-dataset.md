---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The Pile: An 800GB Dataset of Diverse Text for Language Modeling"
authors: Leo Gao et al.
url: https://arxiv.org/abs/2101.00027
date: 2020-12-31
citationCount: 2859
ingested: 2026-06-22
tags: [arxiv, pretraining-data, data]
---

# The Pile: An 800GB Dataset of Diverse Text for Language Modeling

**arXiv [2101.00027](https://arxiv.org/abs/2101.00027)** · 2020-12-31 · 2859 citations · Leo Gao et al.

**Significance.** The founding open-data corpus for the radar's data-stage story: it argued that *diversity beats raw web scale* and gave the open-source world a credible alternative to undisclosed lab datasets.

## Abstract
Recent work has demonstrated that increased training dataset diversity improves general cross-domain knowledge and downstream generalization capability for large-scale language models. With this in mind, we present The Pile: an 825 GiB English text corpus targeted at training large-scale language models. The Pile is constructed from 22 diverse high-quality subsets—both existing and newly constructed—many of which derive from academic or professional sources. Our evaluation of the untuned performance of GPT-2 and GPT-3 on the Pile shows that these models struggle on many of its components, such as academic writing. Conversely, models trained on the Pile improve significantly over both Raw CC and CC-100 on all components of the Pile, while improving performance on downstream evaluations. Through an in-depth exploratory analysis, we document potentially concerning aspects of the data for prospective users. We make publicly available the code used in its construction.

## From the paper (full-text)
**Contribution / method.** The Pile aggregates 22 datasets (~825 GB English text), 14 of them newly constructed, spanning academic (PubMed Central, ArXiv, PhilPapers), code (GitHub, Stack Exchange), books (Books3, PG-19), web (Pile-CC, OpenWebText2, Wikipedia), and specialized text (FreeLaw, USPTO, Enron Emails, DM Mathematics). Pile-CC is a filtered Common Crawl subset extracted with jusText to strip boilerplate. Quality is assessed in bits-per-byte (BPB) using GPT-2/GPT-3 and freshly trained models.
**Results.** GPT-2/GPT-3 show large per-component BPB gaps, struggling most on specialized domains (DM Mathematics, Enron Emails). Models trained on The Pile beat both raw Common Crawl and CC-100 on all components; the biggest gains are in specialized domains — e.g., ~1.65 BPB improvement on DM Mathematics versus Common-Crawl-trained alternatives. Pile-trained models also generalize better zero-shot on external benchmarks. A clean power-law scaling of BPB vs model size holds with no diminishing returns over the range tested.
**Takeaway.** Curated diversity, not just more tokens, drives cross-domain capability — and an open, documented 825 GB corpus made that reproducible.

## Graph
- **Concepts:** [[pretraining-data|Pre-training data]]
- **Raw:** `raw/arxiv/2101.00027.fulltext.md`
