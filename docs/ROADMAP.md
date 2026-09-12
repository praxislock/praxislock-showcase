# Roadmap

## Current generation — Runtime enforcement

PraxisLock currently focuses on:

- content trust / taint
- intent alignment
- DLP
- destination policy
- tool authority
- human approval
- agent identity
- inter-agent trust
- MCP/tool fingerprinting
- tamper-evident auditing

## Next research direction — Adaptive Authority

Instead of only deciding whether a single action should be allowed, PraxisLock will explore dynamically changing **which capabilities the agent possesses** based on the trustworthiness of the information influencing it.

```text
Normal state
    ↓
Agent consumes suspicious content
    ↓
High-impact capabilities quarantined
    ↓
Read-only / investigation capabilities preserved
    ↓
Action necessity evaluated
    ↓
Exact one-use authority may be restored
```

### Research components

- Capability Quarantine
- Capability Shock
- Intent-bound capability leases
- Security-state epochs
- Plan Integrity / Plan Lock
- Memory Immune System
- Causal Influence Graph
- Tool behavioral attestation
- Agent recovery / rollback

## Validation roadmap

Before production use, planned testing includes:

- larger adversarial datasets
- realistic agent workflows
- multi-agent attack chains
- concurrency and race-condition testing
- chaos / failure testing
- performance and latency testing
- restart-state recovery
- external security review
