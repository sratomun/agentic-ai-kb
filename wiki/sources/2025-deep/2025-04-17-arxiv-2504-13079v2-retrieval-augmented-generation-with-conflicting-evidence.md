---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Retrieval-Augmented Generation with Conflicting Evidence"
authors: Han Wang, Archiki Prasad, Elias Stengel-Eskin, Mohit Bansal
url: https://arxiv.org/abs/2504.13079v2
date: 2025-04-17
citationCount: 56
influentialCitationCount: 4
velocity: 3.96
ingested: 2026-06-22
tags: [agent-reliability, agentic-rag, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Retrieval-Augmented Generation with Conflicting Evidence

**arXiv [2504.13079v2](https://arxiv.org/abs/2504.13079v2)** · 2025-04-17 · **56 citations** (4 influential · 3.96/mo) · Han Wang, Archiki Prasad, Elias Stengel-Eskin, Mohit Bansal

## Abstract
Large language model (LLM) agents are increasingly employing retrieval-augmented generation (RAG) to improve the factuality of their responses. However, in practice, these systems often need to handle ambiguous user queries and potentially conflicting information from multiple sources while also suppressing inaccurate information from noisy or irrelevant documents. Prior work has generally studied and addressed these challenges in isolation, considering only one aspect at a time, such as handling ambiguity or robustness to noise and misinformation. We instead consider multiple factors simultaneously, proposing (i) RAMDocs (Retrieval with Ambiguity and Misinformation in Documents), a new dataset that simulates complex and realistic scenarios for conflicting evidence for a user query, including ambiguity, misinformation, and noise; and (ii) MADAM-RAG, a multi-agent approach in which LLM agents debate over the merits of an answer over multiple rounds, allowing an aggregator to collate responses corresponding to disambiguated entities while discarding misinformation and noise, thereby handling diverse sources of conflict jointly. We demonstrate the effectiveness of MADAM-RAG using both closed and open-source models on AmbigDocs -- which requires presenting all valid answers for ambiguous queries -- improving over strong RAG baselines by up to 11.40% and on FaithEval -- which requires suppressing misinformation -- where we improve by up to 15.80% (absolute) with Llama3.3-70B-Instruct. Furthermore, we find that RAMDocs poses a challenge for existing RAG baselines (Llama3.3-70B-Instruct only obtains 32.60 exact match score). While MADAM-RAG begins to address these conflicting factors, our analysis indicates that a substantial gap remains especially when increasing the level of imbalance in supporting evidence and misinformation.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Retrieval-Augmented Generation. RAG Evaluation Benchmarks. Knowledge Conflict in LLMs. 3 Ram Docs: R etrieval with A mbiguity M isinformation in Doc ument s Ambiguous Queries. Distribution of Supporting Documents. Misinformation and Noisy Documents. 4 Madam -RAG: M ulti- a gent D ebate for A mbiguity and M isinformation in RAG Role of a Single LLM Agent. Aggregator Module. Multi-round Debate. End of Debate and Final Answer. 5 Experiments and Results 5.1 Experimental Setup Datasets. Metrics. Models. Baselines. 5.2 Main Results Madam -RAG outperforms baselines across tasks. Ram Docs is a challenging RAG setting. 6 Ablations and Analysis 6.1 Importance of Using the Aggregator and Multiple Rounds of Debate Setup. Takeaway. 6.2 Impact of varying the number of Supporting Documents Setup. Takeaway. 6.3 Impact of Increasing Misinformation Setup. Takeaway. 7 Conclusion A Ram Docs: Dataset Statistics B Speculative RAG C Astute RAG Adaptive Internal Knowledge Gen…

**Method / approach.** methods and document encoding strategies to enhance efficiency and scalability. However, these do not fully address the critical challenge of handling conflicting information across multiple retrieved documents. Prior work, such as Chen et al. ( 2022 ); Zou et al. ( 2024 ) , has shown that RAG systems often propagate misinformation if retrieved documents contain errors, or arbitrarily choose an answer or use parametric knowledge to break ties when documents provide conflicting claims. Unlike existing solutions like Self-RAG (Asai et al., 2024 ) that use LLM-generated critiques, Astute RAG (Wang et al., 2024a ) that uses the LLM’s parametric knowledge and clustering to combine retrieved documents and filter outliers or misinformation, and Speculative RAG (Wang et al., 2025 ) , which uses a small specialist LM to draft multiple answers in parallel from distinct subset documents, and a larger generalist LM to verify and select the best one, Madam -RAG employs multi-agent debate over…

**Results.** Experiments and Results 5.1 Experimental Setup Datasets. Metrics. Models. Baselines. 5.2 Main Results Madam -RAG outperforms baselines across tasks. Ram Docs is a challenging RAG setting. 6 Ablations and Analysis 6.1 Importance of Using the Aggregator and Multiple Rounds of Debate Setup. Takeaway. 6.2 Impact of varying the number of Supporting Documents Setup. Takeaway. 6.3 Impact of Increasing Misinformation Setup. Takeaway. 7 Conclusion A Ram Docs: Dataset Statistics B Speculative RAG C Astute RAG Adaptive Internal Knowledge Generation. Iterative Source-aware Knowledge Consolidation. Answer Finalization. D Computational Efficiency of Madam -RAG E Prompts Retrieval-Augmented Generation with Conflicting Evidence Han Wang Archiki Prasad Elias Stengel-Eskin Mohit Bansal University of North Carolina at Chapel Hill {hwang, archiki, esteng, mban…

**Conclusion.** Conclusion A Ram Docs: Dataset Statistics B Speculative RAG C Astute RAG Adaptive Internal Knowledge Generation. Iterative Source-aware Knowledge Consolidation. Answer Finalization. D Computational Efficiency of Madam -RAG E Prompts Retrieval-Augmented Generation with Conflicting Evidence Han Wang Archiki Prasad Elias Stengel-Eskin Mohit Bansal University of North Carolina at Chapel Hill {hwang, archiki, esteng, mbansal}@cs.unc.edu Abstract Large language model (LLM) agents are increasingly employing retrieval-augmented generation (RAG) to improve the factuality of their responses. However, in practice, these systems often need to handle ambiguous user queries and potentially conflicting infor…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.13079v2.md` · `raw/arxiv/2504.13079v2.fulltext.md`
