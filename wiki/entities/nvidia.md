---
type: entity
entity_type: org
tags: [hardware, infrastructure, nvidia]
created: 2026-06-21
updated: 2026-06-22
source_count: 1
---

# NVIDIA

*The hardware and compute layer of the AI stack — its Vera Rubin platform is explicitly built for agentic AI inference at scale.*

## What it is
NVIDIA is the dominant AI compute provider. Its Vera Rubin platform (announced at GTC March 2026) unifies seven new chips into an AI supercomputer claiming ~10x inference throughput per watt and ~1/10 cost per token versus Blackwell, specifically targeted at agentic AI and reasoning workloads. R100 sampling Q4 2026, volume Q1 2027. → [[2026-06-21-nvidia-vera-rubin-platform]]

## Why it matters
Agent economics — cost per task, latency per decision — are currently dominated by inference cost. Vera Rubin's ~10x efficiency claim, if it ships on schedule, will reshape what agentic deployments are economically viable. The chip layer is now explicitly optimizing for agents-in-production as the dominant workload. See also: [[agentic-ai]]

## Relationships
- builds [[vera-rubin]]
- supplies the compute layer for [[frontier-model-training]]; cashes out [[scaling-laws]]
- customers of its platform: [[openai]], [[mistral]]
