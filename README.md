# AntRouteAGI

AntRouteAGI is an orchestration layer for domain intelligence systems.  
Its core purpose is to route user requests to the right domain agents, coordinate reusable capability agents, verify trustworthiness, and return a unified, high-confidence answer.

## Refined V1 Architecture

1. **Intelligence Router**: decides *who should work* using intent, complexity, cost, and policy.
2. **Planner / Task Decomposer**: decides *what sequence of work should happen* by creating an execution graph.
3. **Capability Agents**: reusable skills (search, reasoning, math, coding, deterministic simulation).
4. **Domain Agents**: field owners (e.g., climate, finance, medical) that orchestrate capability agents.
5. **Shared Infrastructure**: memory, knowledge graph, tool registry, vector DB, and cache.
6. **Selective Multi-Agent Debate (SMAD)**: triggered only for disagreement, low confidence, missing evidence, or conflicting citations; capped at two rounds with strict stop conditions.
7. **Verification & Trust Engine**: checks factual correctness, citation validity, cross-agent consistency, confidence quality, and safety/refusal policy.
8. **MARS**: structures multi-agent outputs into coherent final responses.
9. **Evaluator (Offline, V1)**: benchmarks accuracy, latency, cost, token usage, calibration (ECE), and routing/utilization efficiency.

## Project Direction

- **Phase 1 — Orchestration**: robust routing, planning, verification, and response structuring.
- **Phase 2 — Optimization**: adaptive policies, cost-aware planning, dynamic model selection, and improved calibration.
- **Phase 3 — Emergent Intelligence**: self-improving orchestration, long-horizon autonomy, persistent memory, and agent societies.

In short, AntRouteAGI is designed to unify specialized intelligence systems into one reliable, verifiable decision layer rather than acting as just another standalone agent framework.
