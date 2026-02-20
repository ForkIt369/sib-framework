# TheSibs Architecture v1

## Architectural Intent

Build a reproducible emergent world where AI agents can act autonomously without compromising determinism, safety, or economy integrity.

## Authority Model

- Deterministic world kernel is the source of truth.
- Agent orchestrator is non-authoritative and intent-only.
- Godot client is a renderer/input adapter, not truth owner.
- Economy ledger is append-only and auditable.

## High-Level Topology

```text
+----------------------+         +----------------------+
| OpenClaw/LangGraph   |<------->| Agent Orchestrator   |
| agent runtimes       | intents | (plan + tool policy) |
+----------+-----------+         +----------+-----------+
           |                                 |
           | validated action request        | event stream
           v                                 v
+----------+---------------------------------+-----------+
|                World Kernel (authoritative)            |
| deterministic tick, resources, physics, relationships  |
+----------+----------------------+----------------------+
           |                      |
           v                      v
+----------+-----------+   +------+----------------------+
| Economy Ledger       |   | Social Bridge / Link Graph |
| rewards+sinks+fraud  |   | cross-world artifacts      |
+----------+-----------+   +------+----------------------+
           |                      |
           +-----------+----------+
                       v
             +---------+----------+
             | Realtime Event Bus |
             +---------+----------+
                       |
                       v
      +----------------+----------------+
      | Godot Client + Spectator Web UI |
      +----------------------------------+
```

## Determinism Contract

For each simulation tick:

1. Read world snapshot `S_t`.
2. Read ordered action list `A_t`.
3. Validate all actions against policy, capability, and cost.
4. Apply deterministic transition function `T(S_t, A_t) -> S_t+1`.
5. Emit event log and snapshot hash.

Required properties:
- Tick order is total and stable.
- State transition is pure given seed + action list.
- Any replay with same seed + actions must produce same hash.

## Core Services

### World Kernel
- Tick scheduler.
- Action validator.
- State transition engine.
- Snapshot/event persistence.

### Agent Orchestrator
- Converts observations into candidate intents.
- Applies tool/role constraints.
- Outputs bounded action requests.

### Economy Ledger
- Utility token accounting.
- Sources/sinks enforcement.
- Fraud score hooks and slashing integration.

### Social Bridge
- Cross-world encounter resolution.
- Link Artifact minting (consent + quotas).
- Creator graph updates.

### Policy/Safety
- Content moderation.
- Abuse and spam rate controls.
- Reputation penalties and temporary bans.

### Replay Verifier
- Determinism test runner.
- Snapshot integrity hashing.
- Regression alarms when replay diverges.

## Data Boundaries

- Agent prompt memory cannot directly mutate world state.
- Game clients cannot bypass action validation.
- Economy writes happen only through ledger service.
- Link Artifacts require dual-sided consent events.

## Technology Alignment

- Rendering and simulation UX: Godot 4.6.x stable line.
- Deterministic backend control plane: Convex + worker services.
- Agent planning: LangGraph/OpenClaw integrations.
- Eventing: durable stream with ordered partition per world.
