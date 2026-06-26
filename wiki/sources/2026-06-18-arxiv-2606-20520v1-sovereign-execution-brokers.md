---
type: source
source_type: arxiv
title: "Sovereign Execution Brokers: Enforcing Certificate-Bound Authority in Agentic Control Planes"
authors: Jun He, Deying Yu
url: https://arxiv.org/abs/2606.20520v1
date: 2026-06-18
ingested: 2026-06-21
depth: full-text
tags: [agent-security, arxiv, governance-gap, tool-use]
---

# Sovereign Execution Brokers: Enforcing Certificate-Bound Authority in Agentic Control Planes

**Why it matters:** If you let agents touch production infra at ADP, this is the missing enforcement layer — a runtime broker that holds the only credentials to mutate state and checks a signed certificate at the moment of execution, so a hallucinated or hijacked agent can't open a firewall or drop a database. It's per-action authorization, not per-identity, and it closes the gap between "we approved this" and "this actually ran safely."

## The problem they target
IAM authorizes *identities*; assurance layers certify *proposed actions*. Neither enforces certified authority at the moment of mutation. Once an agent (or its wrapper) holds standing production credentials, the whole admission process can be bypassed — a compromised wrapper or direct API call mutates state without ever passing through the gate. Worse, even a properly admitted action faces a TOCTOU window: between when a proposal is certified (t1) and when it executes (t2), the live state or security posture can drift, turning a safe-at-admission action unsafe. IAM answers a binary "is this principal allowed?"; the authors argue agentic control planes need to answer "is *this specific certified mutation* still valid under current evidence, policy epoch, revocation epoch, and live-state drift?"

## Method
The **Sovereign Execution Broker (SEB)** is a runtime enforcement boundary in the OpenKedge stack (where SQA validates proposals, the Sovereign Assurance Boundary / SAB certifies admitted authority, and SEB enforces certificates at mutation time). Core design:
- **No standing credentials for agents.** SEB is the *only* autonomous-path entity holding mutation credentials; production APIs are configured to reject all non-broker identities (the security theorem depends on this deployment assumption, enforced via cloud IAM/RBAC, mutating + validating admission webhooks, and broker-owned proxies for parameter-level checks IAM can't express).
- **Verification pipeline at execution.** On each request the broker verifies the SAB certificate Ω (Ed25519 signature over RFC 8785 canonical JSON), matches the request against the certified contract C, and checks validity windows, policy epoch, revocation epoch, and live-state drift before acting.
- **Scoped, just-in-time identity.** Credentials are minted only at execution time, scoped to contract, target resource, action/parameters, validity window, and revocation epoch — via AWS STS AssumeRole (minimum 900s session) or Kubernetes TokenRequest (60s projected tokens).
- **Drift predicate + epoch revocation.** A projection/distance check (tolerance ε_C) compares admitted evidence vs. live state; a global revocation epoch counter ρ means any pending certificate signed under an older epoch is rejected (revocation-before-execution) instead of maintaining distributed CRLs.
- **Fail-closed.** If the revocation service is unreachable, drift can't be evaluated, or the policy epoch is stale, the broker rejects. A 5s poll / 5s TTL cache means a partitioned broker fails closed within ~5s.
- **Signed ledger.** Every decision and outcome is written to PostgreSQL and signed with the broker's Ed25519 key; atomic (cid, nonce) nonce reservation prevents replay/double-spend.

Prototype: ~4,200 lines of Go, 3 HA replicas on AWS EKS v1.28 (m6i.xlarge), RDS PostgreSQL v15 ledger.

## Evaluation & results
Evaluated live on AWS + Kubernetes (5,000 trials per config after 100 warm-ups; fault-injection simulated in a controlled harness):
- **Local logic is cheap; network round-trips dominate.** Ed25519 verification, parsing, and contract matching add <0.3 ms total. The cost is drift queries and credential minting: AWS STS minting p50 46.7 ms (p99 158.4 ms), K8s TokenRequest p50 12.1 ms.
- **End-to-end broker overhead:** ~28.2 ms broker-side for Kubernetes mutations (client p50 ~40.7 ms) and ~136.9 ms for AWS security-group mutations (client p50 ~221.9 ms). Of that AWS overhead, the live drift check is 62.3% and credential minting 34.1%.
- **Security: 100% rejection / 0% unsafe-escape across all 9 injected attack classes** (1,000 cases each): uncertified mutation, request-cert mismatch, replayed (cid, nonce), stale policy epoch, stale revocation epoch, revocation partition, malformed Ω, live-state subnet drift, parameter-level violation.
- **Crash recovery:** across 50 injected broker crashes, 25 pre-invocation crashes failed closed (no mutation); the other 25 were resolved against target APIs via idempotency tokens with 100% correct ledger outcomes and no duplicate mutations.
- **Revocation propagation:** max observed delay from epoch advance to 100% rejection was 5.2s (mean 2.6s), bounded by the 5s poll interval.
- **Throughput ceiling is the cloud provider:** K8s TokenRequest scales linearly to ~820 req/s; AWS STS peaks at ~240 req/s before RequestLimitExceeded throttling.

Authors position SEB for **high-risk, low-frequency** mutations (firewall changes, autoscaling, DB exports) where ~140 ms is negligible — explicitly *not* for microsecond control loops. Stated limits include trust in cloud providers, broker as a critical dependency, and that semantic safety stays external (in SAB).

## So what
This is the concrete architectural answer to "how do we let agents act on infra without handing them the keys." The pattern — zero standing privilege, just-in-time scoped tokens, fail-closed enforcement, signed audit ledger, revoke-before-execute — is exactly what a regulated payroll/HR shop would need before agents touch cloud control planes. Two things to flag internally: the security guarantee is entirely contingent on production APIs being locked to reject non-broker identities (the hard part operationally), and the latency profile only works for high-stakes, low-frequency actions. It echoes the per-agent governed-identity direction (cf. MS Scout) but pushes enforcement down to the mutation boundary rather than the identity layer.

**Connects to:** [[agent-security]] [[governance-gap]] [[tool-use]]
**Raw:** `raw/arxiv/2606.20520v1.fulltext.md`
