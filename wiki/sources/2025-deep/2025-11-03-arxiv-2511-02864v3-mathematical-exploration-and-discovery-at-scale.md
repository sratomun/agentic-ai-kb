---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Mathematical exploration and discovery at scale"
authors: Bogdan Georgiev, Javier Gómez-Serrano, Terence Tao, Adam Zsolt Wagner
url: https://arxiv.org/abs/2511.02864v3
date: 2025-11-03
citationCount: 62
influentialCitationCount: 9
velocity: 8.17
ingested: 2026-06-22
tags: [coding-agents, self-evolving-agents, agentic-ai, arxiv, 2025, cited]
---

# Mathematical exploration and discovery at scale

**arXiv [2511.02864v3](https://arxiv.org/abs/2511.02864v3)** · 2025-11-03 · **62 citations** (9 influential · 8.17/mo) · Bogdan Georgiev, Javier Gómez-Serrano, Terence Tao, Adam Zsolt Wagner

## Abstract
AlphaEvolve (Novikov et al., 2025) is a generic evolutionary coding agent that combines the generative capabilities of LLMs with automated evaluation in an iterative evolutionary framework that proposes, tests, and refines algorithmic solutions to challenging scientific and practical problems. In this paper we showcase AlphaEvolve as a tool for autonomously discovering novel mathematical constructions and advancing our understanding of long-standing open problems. To demonstrate its breadth, we considered a list of 67 problems spanning mathematical analysis, combinatorics, geometry, and number theory. The system rediscovered the best known solutions in most of the cases and discovered improved solutions in several. In some instances, AlphaEvolve is also able to generalize results for a finite number of input values into a formula valid for all input values. Furthermore, we are able to combine this methodology with Deep Think and AlphaProof in a broader framework where the additional proof-assistants and reasoning systems provide automated proof generation and further mathematical insights. These results demonstrate that large language model-guided evolutionary search can autonomously discover mathematical constructions that complement human intuition, at times matching or even improving the best known results, highlighting the potential for significant new ways of interaction between mathematicians and AI systems. We present AlphaEvolve as a powerful new tool for mathematical discovery, capable of exploring vast search spaces to solve complex optimization problems at scale, often with significantly reduced requirements on preparation and computation time.

## From the paper (full-text excerpts)
**Introduction.** INTRODUCTION The landscape of mathematical discovery has been fundamentally transformed by the emergence of computational tools that can autonomously explore mathematical spaces and generate novel constructions [56, 120, 242, 291]. AlphaEvolve (see [224]) represents a step in this evolution, demonstrating that large language models, when combined with evolutionary computation and rigorous automated evaluation, can discover explicit constructions that either match or improve upon the best-known bounds to long-standing mathematical problems, at large scales. AlphaEvolve is not a general-purpose solver for all types of mathematical problems; it was primarily designed to attack problems in which a key objective is to construct a complex mathematical object that satisfies good quantitative properties, such as obeying a certain inequality with a good numerical constant. In this followup paper, we report on our experiments testing the performance of AlphaEvolve on a wide variety of such problems, primarily in the areas of analysis, combinatorics, and geometry. In many cases, the constructio…

**Method / approach.** methodology with Deep Think [149] and AlphaProof [148] in a broader framework where the additional proof-assistants and reasoning systems provide automated proof generation and further mathematical insights. These results demonstrate that large language model-guided evolutionary search can autonomously discover mathematical constructions that complement human intuition, at times matching or even improving the best known results, highlighting the potential for significant new ways of interaction between mathematicians and AI systems. We present AlphaEvolve as a powerful tool for mathematical discovery, capable of exploring vast search spaces to solve complex optimization problems at scale, often with significantly reduced requirements on preparation and computation time. 1. INTRODUCTION The landscape of mathematical discovery has been fundamentally transformed by the emergence of computational tools that can autonomously explore mathematical spaces and generate novel constructions [56…

**Results.** experiments testing the performance of AlphaEvolve on a wide variety of such problems, primarily in the areas of analysis, combinatorics, and geometry. In many cases, the constructions provided by AlphaEvolve were not merely numerical in nature, but can be interpreted and generalized by human mathematicians, by other tools such as Deep Think, and even by AlphaEvolve itself. AlphaEvolve was not able to match or exceed previous results in all cases, and some of the individual improvements it was able to achieve could likely also have been matched by more traditional computational or theoretical methods performed by human experts. However, in contrast to such methods, we have found that AlphaEvolve can be readily scaled up to study large classes of problems at a time, without requiring extensive expert supervision for each new problem. This demonstrates that evolutionary computational approaches can systematically explore the space of math…

**Conclusion.** CONCLUSIONS Our exploration of AlphaEvolve has yielded several key insights, which are summarized below. We have found that the selection of the verifier is a critical component that significantly influences the system’s performance and the quality of the discovered results. For example, sometimes the optimizer will be drawn more towards more stable (trivial) solutions which we want to avoid. Designing a clever verifier that avoids this behavior is key to discover new results. Similarly, employing continuous (as opposed to discrete) loss functions proved to be a more effective strategy for guiding the evolutionary search process in some cases. For example, for Problem 6.54 we could have designed our scoring function as the number of touchin…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.02864v3.md` · `raw/arxiv/2511.02864v3.fulltext.md`
