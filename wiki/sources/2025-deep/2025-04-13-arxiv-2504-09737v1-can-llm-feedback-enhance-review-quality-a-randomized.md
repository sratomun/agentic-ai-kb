---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Can LLM feedback enhance review quality? A randomized study of 20K reviews at ICLR 2025"
authors: Nitya Thakkar, Mert Yuksekgonul, Jake Silberg, Animesh Garg et al.
url: https://arxiv.org/abs/2504.09737v1
date: 2025-04-13
citationCount: 50
influentialCitationCount: 4
velocity: 3.5
ingested: 2026-06-22
tags: [agent-reliability, agentic-ai, arxiv, 2025, cited]
---

# Can LLM feedback enhance review quality? A randomized study of 20K reviews at ICLR 2025

**arXiv [2504.09737v1](https://arxiv.org/abs/2504.09737v1)** · 2025-04-13 · **50 citations** (4 influential · 3.5/mo) · Nitya Thakkar, Mert Yuksekgonul, Jake Silberg, Animesh Garg et al.

## Abstract
Peer review at AI conferences is stressed by rapidly rising submission volumes, leading to deteriorating review quality and increased author dissatisfaction. To address these issues, we developed Review Feedback Agent, a system leveraging multiple large language models (LLMs) to improve review clarity and actionability by providing automated feedback on vague comments, content misunderstandings, and unprofessional remarks to reviewers. Implemented at ICLR 2025 as a large randomized control study, our system provided optional feedback to more than 20,000 randomly selected reviews. To ensure high-quality feedback for reviewers at this scale, we also developed a suite of automated reliability tests powered by LLMs that acted as guardrails to ensure feedback quality, with feedback only being sent to reviewers if it passed all the tests. The results show that 27% of reviewers who received feedback updated their reviews, and over 12,000 feedback suggestions from the agent were incorporated by those reviewers. This suggests that many reviewers found the AI-generated feedback sufficiently helpful to merit updating their reviews. Incorporating AI feedback led to significantly longer reviews (an average increase of 80 words among those who updated after receiving feedback) and more informative reviews, as evaluated by blinded researchers. Moreover, reviewers who were selected to receive AI feedback were also more engaged during paper rebuttals, as seen in longer author-reviewer discussions. This work demonstrates that carefully designed LLM-generated review feedback can enhance peer review quality by making reviews more specific and actionable while increasing engagement between reviewers and authors. The Review Feedback Agent is publicly available at https://github.com/zou-group/review_feedback_agent.

## From the paper (full-text excerpts)
**Introduction.** Introduction Scientific peer review is a critical step before publication, where domain experts evaluate the research to ensure thoroughness and scientific integrity, prevent false claims, and provide a strong foundation for future work [1, 2]. High-quality reviews are essential for authors to improve their work, address key limitations, and advance scientific progress. However, in a survey of 11,800 researchers worldwide, while 98% view peer review as essential to maintaining the quality and integrity of academic communication, only 55.4% expressed satisfaction with the quality of reviews they receive [3]. This dissatisfaction has grown as obtaining constructive and high-quality peer reviews has become more challenging due to the increase in the number of paper submissions, especially in fast-moving areas like Artificial Intelligence (AI) [4, 5]. For example, the International Conference on Learning Representations (ICLR) experienced year-over-year submission increases of 47% in 2024 and 61% in 2025 [6]. To maintain a rigorous and meaningful peer review process amid this growth, it…

**Method / approach.** methods you feel are missing from the current comparison? Could you elaborate why? Does Figure 5 of the paper answer your question? In particular: “In Transformers, the proposed technique provides 25% relative improvement in wall-clock time (Figure 5)”. We appreciate your review, but kindly request that you focus your comments on the content and methodology of the paper rather than making personal remarks about the authors. C The reviewer's comments are already specific and actionable, so I do not need to provide any feedback on them. Paper Reviewer comment: This paper could use more experimental baselines. Feedback to the reviewer: It would be helpful to suggest specific baselines that you think must be included. Are there particular methods you feel are missing from the current comparison? Could you elaborate why? It would be helpful to suggest specific baselines that you think must be included. Are there particular methods you feel are missing from the current comparison? Coul…

**Results.** Experiment highlighted inconsistencies in the peer review process by showing that approximately 25% of paper acceptance decisions differed between two independent review committees [10]. These issues not only frustrate authors but potentially allow weaker research to be accepted while strong work is rejected, ultimately preventing papers from reaching their full potential due to the decline of meaningful dialogue between reviewers and authors. Large language models (LLMs) [11] have the potential to enhance the quality and usefulness of peer reviews for authors [12]. Recent studies demonstrated that LLMs can serve as effective critics, generating detailed and constructive feedback [13, 14]. Furthermore, LLMs have already shown high utilization in the peer review process. Reviewers are increasingly turning to LLMs to assist in drafting their reviews, with an estimated 10.6% of reviewers at ICLR 2024 using LLMs for this purpose [15, 16]. T…

**Conclusion.** discussions. This work demonstrates that carefully designed LLM-generated review feedback can enhance peer review quality by making reviews more specific and actionable while increasing engagement between reviewers and authors. The Review Feedback Agent is publicly available at https://github.com/zou-group/review feedback agent. 1 Introduction Scientific peer review is a critical step before publication, where domain experts evaluate the research to ensure thoroughness and scientific integrity, prevent false claims, and provide a strong foundation for future work [1, 2]. High-quality reviews are essential for authors to improve their work, address key limitations, and advance scientific progress. However, in a survey of 11,800 researcher…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.09737v1.md` · `raw/arxiv/2504.09737v1.fulltext.md`
