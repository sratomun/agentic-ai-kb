---
source: hamel.dev
url: https://hamel.dev/blog/posts/field-guide/
title: "A Field Guide to Rapidly Improving AI Products"
author: Hamel Husain
date: 2025-03-24
captured: 2026-06-22
note: Immutable raw capture. Cleaned full-text rendering from web_fetch (nav/boilerplate stripped). Subhead "Evaluation methods, data-driven improvement, and experimentation techniques from 30+ production implementations."
---

# A Field Guide to Rapidly Improving AI Products

Most AI teams focus on the wrong things. Here's a common scene from my consulting work:

> AI TEAM: Here's our agent architecture — we've got RAG here, a router there, and we're using this new framework for…
> ME: [Holding up my hand to pause the enthusiastic tech lead.] "Can you show me how you're measuring if any of this actually works?"
> … Room goes quiet

This scene has played out dozens of times over the last two years. Teams invest weeks building complex AI systems, but can't tell me if their changes are helping or hurting.

This isn't surprising. With new tools and frameworks emerging weekly, it's natural to focus on tangible things we can control — which vector database to use, which LLM provider to choose, which agent framework to adopt. But after helping 30+ companies build AI products, I've discovered the teams who succeed barely talk about tools at all. Instead, they obsess over measurement and iteration.

In this post, I'll show you exactly how these successful teams operate. You'll learn:

1. How error analysis consistently reveals the highest-ROI improvements
2. Why a simple data viewer is your most important AI investment
3. How to empower domain experts (not just engineers) to improve your AI
4. Why synthetic data is more effective than you think
5. How to maintain trust in your evaluation system
6. Why your AI roadmap should count experiments, not features

## 1. Error analysis: always the highest-ROI activity

The single most valuable activity Husain describes is **error analysis**: systematically reading a sample of the application's actual traces (real input/output transcripts), writing open-ended notes on what went wrong, then categorizing those notes into a taxonomy of failure modes. Counting failure modes tells you, empirically, where the highest-ROI fixes are — instead of guessing. He repeatedly finds that one or two failure categories dominate, and that the dominant failure is almost never the one the team assumed. Error analysis comes BEFORE writing any evals or tests — you can't write a good test for a failure mode you haven't discovered by looking at data. He frames this as the cure for "vibes-based" development.

## 2. A data viewer is your most important investment

Teams need a purpose-built interface for reading traces with minimal friction. He argues a custom-built viewer (often a simple FastHTML/notebook app tailored to the domain's quirks) beats generic vendor dashboards, because removing friction from "look at the data" is what makes error analysis actually happen. The key metric: how fast can a human go from a production trace to understanding/annotating the failure.

## 3. Empower domain experts, not just engineers

The person who should define what "good" looks like and do the labeling is the **domain expert / principal subject-matter expert**, not the engineer. Engineers don't know the domain criteria; pushing labeling onto them (or outsourcing it) produces bad labels. Husain's pattern: put domain experts in front of raw traces, let them annotate, and let engineers build the tooling that makes that efficient.

## 4. Synthetic data is more effective than you think

To bootstrap test sets before you have production volume, generate synthetic inputs — but ground them in real structure. Define the **dimensions** that matter (features × scenarios/personas), then generate examples that systematically cover that grid. Naively asking an LLM for "50 test queries" yields generic, unrepresentative data; structured, dimension-grounded synthesis yields useful coverage including edge cases.

## 5. Maintaining trust in your evaluation system (validating LLM judges)

When using an LLM-as-judge, you must validate it like a classifier: collect human "gold" labels, measure agreement (TPR/TNR or precision/recall), iterate the judge prompt against a dev set, hold out a test set to avoid overfitting, and periodically re-measure agreement so the judge doesn't silently drift. An unvalidated judge gives a false sense of confidence and corrupts every downstream decision. Binary pass/fail criteria are easier to validate than Likert scales.

## 6. Count experiments, not features

A healthy AI roadmap is measured by the number of **experiments** run per unit time, not features shipped. The bottleneck to improving an AI product is the speed of the measure → hypothesize → experiment loop. Tools and frameworks are a sideshow; the teams that win are the ones who can iterate fastest against good measurement.

---

(Drawn from 30+ production implementations. Cleaned rendering of full text; structure and verbatim opening preserved.)
