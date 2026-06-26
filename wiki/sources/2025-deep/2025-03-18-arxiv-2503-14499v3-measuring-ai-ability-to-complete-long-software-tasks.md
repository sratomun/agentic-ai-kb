---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Measuring AI Ability to Complete Long Software Tasks"
authors: Thomas Kwa, Ben West, Joel Becker, Amy Deng et al.
url: https://arxiv.org/abs/2503.14499v3
date: 2025-03-18
citationCount: 98
influentialCitationCount: 6
velocity: 6.47
ingested: 2026-06-22
tags: [agent-reliability, tool-use, agent-evaluation, arxiv, 2025, cited]
---

# Measuring AI Ability to Complete Long Software Tasks

**arXiv [2503.14499v3](https://arxiv.org/abs/2503.14499v3)** · 2025-03-18 · **98 citations** (6 influential · 6.47/mo) · Thomas Kwa, Ben West, Joel Becker, Amy Deng et al.

## Abstract
Despite rapid progress on AI benchmarks, the real-world meaning of benchmark performance remains unclear. To quantify the capabilities of AI systems in terms of human capabilities, we propose a new metric: 50%-task-completion time horizon. This is the time humans typically take to complete tasks that AI models can complete with 50% success rate. We first timed humans with relevant domain expertise on a combination of RE-Bench, HCAST, and 66 novel shorter tasks. On these tasks, current frontier AI models such as Claude 3.7 Sonnet have a 50% time horizon of around 50 minutes. Furthermore, frontier AI time horizon has been doubling approximately every seven months since 2019, though the trend may have accelerated in 2024. The increase in AI models' time horizons seems to be primarily driven by greater reliability and ability to adapt to mistakes, combined with better logical reasoning and tool use capabilities. We discuss the limitations of our results -- including their degree of external validity -- and the implications of increased autonomy for dangerous capabilities. If these results generalize to real-world software tasks, extrapolation of this trend predicts that within 5 years, AI systems will be capable of automating many software tasks that currently take humans a month.

## From the paper (full-text excerpts)
**Introduction.** Introduction 1.1 Related Work Agentic AI capability benchmarks AI capability forecasting Human psychometric methods 2 Measuring AI agent performance on realistic tasks 2.1 Task suite / dataset Example tasks 2.2 Baselining 2.3 Results 3 Time horizon 3.1 Computing time horizon 3.2 Time horizon vs. release date 3.2.1 Time horizons at 50% success rate vs 80% success rate 3.3 Qualitative analysis 4 External validity and robustness 4.1 SWE-bench Verified 5 Extrapolation Extrapolating towards one-month-horizon AI Sensitivity analysis Task distribution limitations Future changes in time horizon trends 6 Discussion Summary Limitations and future work References A Expanded Related work A.1 Agent and capability benchmarks A.2 Forecasting AI progress A.3 Psychometric methods and Item Response Theory B Task suite details B.1 Task subsuites B.1.1 HCAST suite B.1.2 RE-Bench suite B.1.3 Software atomic actions (SWAA) suite Decisions (multiple choice) Fill-in-the-blank RE-Bench B.2 Limi…

**Method / approach.** methods 2 Measuring AI agent performance on realistic tasks 2.1 Task suite / dataset Example tasks 2.2 Baselining 2.3 Results 3 Time horizon 3.1 Computing time horizon 3.2 Time horizon vs. release date 3.2.1 Time horizons at 50% success rate vs 80% success rate 3.3 Qualitative analysis 4 External validity and robustness 4.1 SWE-bench Verified 5 Extrapolation Extrapolating towards one-month-horizon AI Sensitivity analysis Task distribution limitations Future changes in time horizon trends 6 Discussion Summary Limitations and future work References A Expanded Related work A.1 Agent and capability benchmarks A.2 Forecasting AI progress A.3 Psychometric methods and Item Response Theory B Task suite details B.1 Task subsuites B.1.1 HCAST suite B.1.2 RE-Bench suite B.1.3 Software atomic actions (SWAA) suite Decisions (multiple choice) Fill-in-the-blank RE-Bench B.2 Limitations of the tas…

**Results.** experiments, which find little evidence of performance trends being slower on the somewhat more realistic tasks we tested, but do not rule out the possibility that trends are meaningfully slower on the distribution of tasks required to automate software engineer jobs. We also find evidence that AI agent time horizons can differ by a large factor depending on the task domain and reference human population. We conclude by discussing implications for AI capabilities forecasting (Section 5 ). Naively extrapolating the trend in horizon length implies that AI will reach a time horizon of 1 month (167 work hours) between mid-2028 and mid-2031 (Figure 6 ). However, extrapolation is affected by both external validity concerns and future changes in the trend. Figure 2: Our methodology for measuring AI agent time horizon. First, we create a diverse task suite of 170 tasks. Second, we have both humans and AI agents (consisting of an AI mode…

**Conclusion.** Discussion Summary Limitations and future work References A Expanded Related work A.1 Agent and capability benchmarks A.2 Forecasting AI progress A.3 Psychometric methods and Item Response Theory B Task suite details B.1 Task subsuites B.1.1 HCAST suite B.1.2 RE-Bench suite B.1.3 Software atomic actions (SWAA) suite Decisions (multiple choice) Fill-in-the-blank RE-Bench B.2 Limitations of the task suite C Methodological details C.1 Human baselines C.1.1 HCAST tasks C.1.2 RE-Bench baselines C.1.3 SWAA baselines C.1.4 Baseline success rate Human time horizon C.1.5 Baseline time analysis C.2 Internal PR tasks Summary Methodology Example issues ‣ Example i…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]]
- **Raw:** `raw/arxiv/2503.14499v3.md` · `raw/arxiv/2503.14499v3.fulltext.md`
