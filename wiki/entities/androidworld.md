---
type: entity
entity_type: benchmark
tags: [agents, benchmark]
created: 2026-06-21
updated: 2026-06-22
census_count: 25
---

# AndroidWorld

*A benchmark for mobile-device GUI agents operating real Android apps — no API access, pure UI navigation.*

## What it is
AndroidWorld runs agents inside a real Android emulator where they must complete tasks by navigating UIs, tapping, typing, and swiping through actual installed apps — no API shortcuts. Appears in ~25 of the 2026 H1 census papers as the standard benchmark for mobile GUI agents.

## Why it matters
Computer-use on mobile is the hardest end of the GUI-agent spectrum; AndroidWorld performance sets the ceiling on what enterprise computer-use agents can handle in unstructured UI environments — directly relevant to field or mobile workflows where APIs don't exist.

## Relationships
- evaluates [[computer-use-agents]]
