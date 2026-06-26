---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Hilbert: Recursively Building Formal Proofs with Informal Reasoning"
authors: Sumanth Varambally, Thomas Voice, Yanchao Sun, Zhifeng Chen et al.
url: https://arxiv.org/abs/2509.22819v2
date: 2025-09-26
citationCount: 42
influentialCitationCount: 9
velocity: 4.75
ingested: 2026-06-22
tags: [multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Hilbert: Recursively Building Formal Proofs with Informal Reasoning

**arXiv [2509.22819v2](https://arxiv.org/abs/2509.22819v2)** · 2025-09-26 · **42 citations** (9 influential · 4.75/mo) · Sumanth Varambally, Thomas Voice, Yanchao Sun, Zhifeng Chen et al.

## Abstract
Large Language Models (LLMs) demonstrate impressive mathematical reasoning abilities, but their solutions frequently contain errors that cannot be automatically checked. Formal theorem proving systems such as Lean 4 offer automated verification with complete accuracy, motivating recent efforts to build specialized prover LLMs that generate verifiable proofs in formal languages. However, a significant gap remains: current prover LLMs solve substantially fewer problems than general-purpose LLMs operating in natural language. We introduce Hilbert, an agentic framework that bridges this gap by combining the complementary strengths of informal reasoning and formal verification. Our system orchestrates four components: an informal LLM that excels at mathematical reasoning, a specialized prover LLM optimized for Lean 4 tactics, a formal verifier, and a semantic theorem retriever. Given a problem that the prover is unable to solve, Hilbert employs recursive decomposition to split the problem into subgoals that it solves with the prover or reasoner LLM. It leverages verifier feedback to refine incorrect proofs as necessary. Experimental results demonstrate that Hilbert substantially outperforms existing approaches on key benchmarks, achieving 99.2\% on miniF2F, 6.6\% points above the best publicly available method. Hilbert achieves the \textbf{strongest known result} from a publicly available model on PutnamBench. It solves 462/660 problems (70.0\%), outperforming proprietary approaches like SeedProver (50.4\%) and achieving a 422\% improvement over the best publicly available baseline. Thus, Hilbert effectively narrows the gap between informal reasoning and formal proof generation. Code is available at https://github.com/Rose-STL-Lab/ml-hilbert.

## From the paper (full-text excerpts)
**Method / approach.** method. H ILBERT achieves the strongest known result from a publicly available model on PutnamBench. It solves 462/660 problems (70.0%), outperforming proprietary approaches like SeedProver (50.4%) and achieving a 422% improvement over the best publicly available baseline. Thus, H ILBERT effectively narrows the gap between informal reasoning and formal proof generation. Code is available at https://github.com/Rose-STL-Lab/ml-hilbert. 1 I NTRODUCTION General-purpose Large Language Models (LLMs) have achieved dramatic improvements in mathematical understanding. Reasoning LLMs like GPT-5 and Gemini 2.5 Pro attain near-perfect performance on highschool olympiad exams such as AIME and can solve a significant proportion of competitive undergraduatelevel problems from the Putnam exam (Dekoninck et al., 2025). These systems also show promise on research-level benchmarks like FrontierMath (Glazer et al., 2024; OpenAI, 2025). However, several fundamental limitations severely constrain their…

**Results.** Experimental results demonstrate that H ILBERT substantially outperforms existing approaches on key benchmarks, achieving 99.2% on miniF2F, 6.6% points above the best publicly available method. H ILBERT achieves the strongest known result from a publicly available model on PutnamBench. It solves 462/660 problems (70.0%), outperforming proprietary approaches like SeedProver (50.4%) and achieving a 422% improvement over the best publicly available baseline. Thus, H ILBERT effectively narrows the gap between informal reasoning and formal proof generation. Code is available at https://github.com/Rose-STL-Lab/ml-hilbert. 1 I NTRODUCTION General-purpose Large Language Models (LLMs) have achieved dramatic improvements in mathematical understanding. Reasoning LLMs like GPT-5 and Gemini 2.5 Pro attain near-perfect performance on highschool olympiad exams such as AIME and can solve a significant proportion of competitive undergraduatelevel pro…

**Conclusion.** discussions about this work. RY was supported in part by the U.S. Army Research Office under Army-ECASE award W911NF-07-R-0003-03, the U.S. Department Of Energy, Office of Science, IARPA HAYSTAC Program, NSF Grants #2205093, #2146343, and #2134274, CDC-RFA-FT-23-0069, as well as DARPA AIE FoundSci and DARPA YFA. R EFERENCES Sandhini Agarwal, Lama Ahmad, Jason Ai, Sam Altman, Andy Applebaum, Edwin Arbus, Rahul K Arora, Yu Bai, Bowen Baker, Haiming Bao, et al. gpt-oss-120b & gpt-oss-20b model card. arXiv preprint arXiv:2508.10925, 2025. Team AlphaProof and Team AlphaGeometry. Ai achieves silver-medal standard solving international 178 mathematical olympiad problems. DeepMind blog, 179:45, 2024. Kaito Baba, Chaoran Liu, Shuhei Kurita, and Aki…

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.22819v2.md` · `raw/arxiv/2509.22819v2.fulltext.md`
