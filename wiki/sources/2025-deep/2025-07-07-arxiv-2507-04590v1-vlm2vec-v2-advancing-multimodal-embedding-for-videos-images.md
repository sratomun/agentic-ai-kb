---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "VLM2Vec-V2: Advancing Multimodal Embedding for Videos, Images, and Visual Documents"
authors: Rui Meng, Ziyan Jiang, Ye Liu, Mingyi Su et al.
url: https://arxiv.org/abs/2507.04590v1
date: 2025-07-07
citationCount: 75
influentialCitationCount: 17
velocity: 6.52
ingested: 2026-06-22
tags: [recommendation-agents, agentic-rag, agent-evaluation, arxiv, 2025, cited]
---

# VLM2Vec-V2: Advancing Multimodal Embedding for Videos, Images, and Visual Documents

**arXiv [2507.04590v1](https://arxiv.org/abs/2507.04590v1)** · 2025-07-07 · **75 citations** (17 influential · 6.52/mo) · Rui Meng, Ziyan Jiang, Ye Liu, Mingyi Su et al.

## Abstract
Multimodal embedding models have been crucial in enabling various downstream tasks such as semantic similarity, information retrieval, and clustering over different modalities. However, existing multimodal embeddings like VLM2Vec, E5-V, GME are predominantly focused on natural images, with limited support for other visual forms such as videos and visual documents. This restricts their applicability in real-world scenarios, including AI agents, multi-modal search and recommendation, and retrieval-augmented generation (RAG). To close this gap, we propose VLM2Vec-V2, a unified framework for learning embeddings across diverse visual forms. First, we introduce MMEB-V2, a comprehensive benchmark that extends MMEB with five new task types: visual document retrieval, video retrieval, temporal grounding, video classification and video question answering - spanning text, image, video, and visual document inputs. Next, we train VLM2Vec-V2, a general-purpose embedding model that supports text, image, video, and visual document inputs. Extensive experiments show that VLM2Vec-V2 achieves strong performance not only on the newly introduced video and document retrieval tasks, but also improves over prior baselines on the original image benchmarks. Through extensive evaluation, our study offers insights into the generalizability of various multimodal embedding models and highlights effective strategies for unified embedding learning, laying the groundwork for more scalable and adaptable representation learning in both research and real-world settings.

## From the paper (full-text excerpts)
**Introduction.** Introduction Embedding models play a crucial role in connecting data across various modalities. By encoding heterogeneous multimodal data into a shared dense representation space, they enable many down-stream applications like classification, clustering, retrieval, etc. In recent years, we have witnessed significant advances in embedding models, largely driven by the progress of large foundation models. For instance, recent breakthroughs in text embedding (Su et al., 2023; Wang et al., 2024a; Meng et al., 2024; BehnamGhader et al., 2024) have been achieved by integrating pretrained large language models with multi-task instruction embedding tuning. Similarly, Jiang et al. (2024); Zhang et al. (2024b); Chen et al. (2025) demonstrated strong performance across multiple text-image tasks by instruction-tuning vision language models (VLMs) into effective embedding models. Existing multimodal embedding models are trained on datasets like MMEB (Jiang et al., 2024) and M-BEIR (Wei et al., 2023), which are focused predominantly on natural images or photographs, sourced from MSCOCO (Lin et al…

**Method / approach.** methods aim to build models capable of retrieving information across multiple data types—such as text, images, audio, and video—within a single framework. Approaches like GME (Zhang et al., 2024b) and Uni-Retrieval (Jia et al., 2025) leverage multimodal large language models and prompt-tuning to accommodate diverse queries and modalities, achieving strong performance on universal benchmarks. Meanwhile, methods such as UniversalRAG (Yeo et al., 2025) and UniRAG (Sharifymoghaddam et al., 9 Preprint. 2025) improve retrieval-augmented generation by dynamically routing queries to the most suitable modality and granularity, enhancing both flexibility and accuracy. However, none of these models are designed to unify image, video, and visual document retrieval within a single framework, as our VLM2Vec-V2 does. 6 Conclusion We introduced MMEB-V2, a comprehensive benchmark for evaluating multimodal embedding models across text, image, video, and visual document modalities. Alongside it, w…

**Results.** experiments show that VLM2Vec-V2 achieves strong performance not only on the newly introduced video and document retrieval tasks, but also improves over prior baselines on the original image benchmarks. Through extensive evaluation, our study offers insights into the generalizability of various multimodal embedding models and highlights effective strategies for unified embedding learning, laying the groundwork for more scalable and adaptable representation learning in both research and real-world settings. 1 Introduction Embedding models play a crucial role in connecting data across various modalities. By encoding heterogeneous multimodal data into a shared dense representation space, they enable many down-stream applications like classification, clustering, retrieval, etc. In recent years, we have witnessed significant advances in embedding models, largely driven by the progress of large foundation models. For instance, recent break…

**Conclusion.** Conclusion We introduced MMEB-V2, a comprehensive benchmark for evaluating multimodal embedding models across text, image, video, and visual document modalities. Alongside it, we proposed VLM2Vec-V2, a strong baseline trained via contrastive learning across a diverse range of tasks and modality combinations. Our extensive experiments demonstrate the effectiveness of VLM2Vec-V2 and the diagnostic value of MMEB-V2. References Lisa Anne Hendricks, Oliver Wang, Eli Shechtman, Josef Sivic, Trevor Darrell, and Bryan Russell. Localizing moments in video with natural language. In Proceedings of the IEEE international conference on computer vision, pp. 5803–5812, 2017. Parishad BehnamGhader, Vaibhav Adlakha, Marius Mosbach, Dzmitry Bahdanau, Nicol…

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2507.04590v1.md` · `raw/arxiv/2507.04590v1.fulltext.md`
