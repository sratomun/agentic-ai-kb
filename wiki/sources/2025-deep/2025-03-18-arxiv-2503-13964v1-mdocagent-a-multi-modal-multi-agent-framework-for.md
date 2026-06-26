---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MDocAgent: A Multi-Modal Multi-Agent Framework for Document Understanding"
authors: Siwei Han, Peng Xia, Ruiyi Zhang, Tong Sun et al.
url: https://arxiv.org/abs/2503.13964v1
date: 2025-03-18
citationCount: 51
influentialCitationCount: 14
velocity: 3.37
ingested: 2026-06-22
tags: [agentic-rag, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# MDocAgent: A Multi-Modal Multi-Agent Framework for Document Understanding

**arXiv [2503.13964v1](https://arxiv.org/abs/2503.13964v1)** · 2025-03-18 · **51 citations** (14 influential · 3.37/mo) · Siwei Han, Peng Xia, Ruiyi Zhang, Tong Sun et al.

## Abstract
Document Question Answering (DocQA) is a very common task. Existing methods using Large Language Models (LLMs) or Large Vision Language Models (LVLMs) and Retrieval Augmented Generation (RAG) often prioritize information from a single modal, failing to effectively integrate textual and visual cues. These approaches struggle with complex multi-modal reasoning, limiting their performance on real-world documents. We present MDocAgent (A Multi-Modal Multi-Agent Framework for Document Understanding), a novel RAG and multi-agent framework that leverages both text and image. Our system employs five specialized agents: a general agent, a critical agent, a text agent, an image agent and a summarizing agent. These agents engage in multi-modal context retrieval, combining their individual insights to achieve a more comprehensive understanding of the document's content. This collaborative approach enables the system to synthesize information from both textual and visual components, leading to improved accuracy in question answering. Preliminary experiments on five benchmarks like MMLongBench, LongDocURL demonstrate the effectiveness of our MDocAgent, achieve an average improvement of 12.1% compared to current state-of-the-art method. This work contributes to the development of more robust and comprehensive DocQA systems capable of handling the complexities of real-world documents containing rich textual and visual information. Our data and code are available at https://github.com/aiming-lab/MDocAgent.

## From the paper (full-text excerpts)
**Method / approach.** Method Layout Text Figure Table Others Avg \midrule LVLMs \midrule Qwen2-VL-7B-Instruct 0.264 0.386 0.308 0.207 0.500 0.296 Qwen2.5-VL-7B-Instruct 0.357 0.479 0.442 0.299 0.375 0.389 llava-v1.6-mistral-7b 0.067 0.165 0.088 0.051 0.250 0.099 llava-one-vision-7B 0.098 0.200 0.144 0.057 0.125 0.126 Phi-3.5-vision-instruct 0.245 0.375 0.291 0.187 0.375 0.280 SmolVLM-Instruct 0.128 0.224 0.164 0.100 0.250 0.163 \midrule RAG methods (top 1) \midrule ColBERTv2+Llama-3.1-8B 0.257 0.529 0.471 0.428 0.775 0.429 M3DocRAG (ColPali+Qwen2-VL-7B) 0.340 0.605 0.546 0.520 0.625 0.506 \ours (Ours) 0.341 0.612 0.540 0.527 0.750 0.517 \midrule RAG methods (top 4) \midrule ColBERTv2+Llama-3.1-8B 0.349 0.599 0.491 0.485 0.875 0.491 M3DocRAG (ColPali+Qwen2-VL-7B) 0.426 0.660 0.595 0.542 0.625 0.554 \ou…

**Results.** Experiments on different model backbones in \ours \thesubsection Additional case studies \section Experimental Setup \label sec:appendix_section \subsection Baseline Models • Qwen2-VL-7B-Instruct [ Qwen2-VL ] : A large vision-language model developed by Alibaba, designed to handle multiple images as input. • Qwen2.5-VL-7B-Instruct [ Qwen2.5-VL ] : An enhanced version of Qwen2-VL-7B-Instruct, offering improved performance in processing multiple images. • llava-v1.6-mistral-7b [ liu2023improved ] : Also called LLaVA-NeXT, a vision-language model improved upon LLaVa-1.5, capable of interpreting and generating content from multiple images. • Phi-3.5-vision-instruct [ abdin2024phi ] : A model developed by Microsoft that integrates vision and language understanding, designed to process and generate responses based on multiple images. • llava-one-vision-7B [ li2024llava ] : A model tr…

**Conclusion.** conclusion should reflect the consensus (if one exists) or the most credible and well-supported answer. Return the final answer in the following dictionary format: {”Answer”: Your final answer here} {tcolorbox} [title=Evaluation] Question : {question} Predicted Answer : {answer} Ground Truth Answer : {gt} Please evaluate whether the predicted answer is correct. • If the answer is correct, return 1. • If the answer is incorrect, return 0. Return only a string formatted as a valid JSON dictionary that can be parsed using json.loads , for example: {”correctness”: 1} \thesubsection Evaluation Metrics The metric of all benchmarks is the average binary correctness evaluated by GPT-4o. The evaluation prompt is given…

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.13964v1.md` · `raw/arxiv/2503.13964v1.fulltext.md`
