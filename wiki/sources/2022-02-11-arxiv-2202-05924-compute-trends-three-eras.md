---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Compute Trends Across Three Eras of Machine Learning"
authors: Jaime Sevilla et al.
url: https://arxiv.org/abs/2202.05924
date: 2022-02-11
citationCount: omit
tags: [arxiv, scaling-laws]
---

# Compute Trends Across Three Eras of Machine Learning

**arXiv [2202.05924](https://arxiv.org/abs/2202.05924)** · 2022-02-11 · Jaime Sevilla et al.

**Significance.** Splits ML history into three compute eras and quantifies how training-compute doubling time collapsed from ~21 months to ~6 months once deep learning arrived.

## Abstract
Compute, data, and algorithmic advances are the three fundamental factors that guide the progress of modern Machine Learning (ML). In this paper we study trends in the most readily quantified factor – compute. We show that before 2010 training compute grew in line with Moore's law, doubling roughly every 20 months. Since the advent of Deep Learning in the early 2010s, the scaling of training compute has accelerated, doubling approximately every 6 months. In late 2015, a new trend emerged as firms developed large-scale ML models with 10 to 100-fold larger requirements in training compute. Based on these observations we split the history of compute in ML into three eras: the Pre Deep Learning Era, the Deep Learning Era and the Large-Scale Era. Overall, our work highlights the fast-growing compute requirements for training advanced ML systems.

## From the paper (full-text)
**Contribution / method.** Curate a dataset of 123 milestone ML systems with estimated training compute (FLOPs) spanning 1952–2022, then fit log-linear trends to identify regime changes and split history into three eras.

**Results.** Three eras and their fitted doubling times (Table 2 medians):
- **Pre Deep Learning Era (1952–2010, n=19):** 3e4 to 2e14 FLOPs; ~0.2 OOMs/year; doubling time 21.3 months [17.0; 21.2; 29.3] — roughly Moore's law (Conclusion: "18-month doubling time between 1952 and 2010").
- **Deep Learning Era (2010–2022, regular-scale, n=72):** 7e14 to 2e18 FLOPs; ~0.6 OOMs/year; doubling time 5.7 months [4.3; 5.6; 9.0].
- **Large-Scale Era (Sept 2015–2022, large-scale models, n=16):** 4e21 to 8e23 FLOPs; ~0.4 OOMs/year; doubling time 9.9 months [7.7; 10.1; 17.1].

Large-scale models began ~2 to 3 orders of magnitude above the prior trend (abstract phrases the gap as "10 to 100-fold larger" requirements), starting around AlphaGo in late 2015. Supporting text: pre-2010 doubled every "17 to 29 months," then "every 4 to 9 months."

**Takeaway.** Training-compute growth has accelerated ~3.5x over Moore's law since deep learning began, with a distinct large-scale trend (~10-month doubling) layered on top after 2015.

## Graph
- **Concepts:** [[scaling-laws|Scaling laws]]
- **Entities:** AlphaGo, Moore's law, Epoch (compute dataset)
- **Raw:** `raw/arxiv/2202.05924.fulltext.md`
