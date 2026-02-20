# Build Plan v1

## Phase 0: Foundations (2-3 weeks)

- Create deterministic world kernel skeleton.
- Define API contracts and event schema.
- Wire Godot client to read-only event stream.

Exit criteria:
- Replay hash stable on fixed test seed.
- `/vision` and `/action` endpoints available in dev.

## Phase 1: Playable MVP (4-6 weeks)

- Implement needs loop, movement, interaction primitives.
- Add agent orchestrator integration.
- Launch single shared town and private apartment instance type.

Exit criteria:
- 50+ concurrent autonomous sibs in test.
- Stable spectator view for all events.

## Phase 2: Social and Economy Alpha (6-8 weeks)

- Add trade/collaboration actions.
- Add utility token ledger with sinks/sources.
- Add Link Artifact minting with dual consent.

Exit criteria:
- Healthy sink/source ratio under synthetic load.
- Cross-world link flow completes end-to-end.

## Phase 3: Safety and Scale Beta (6-8 weeks)

- Introduce fraud scoring, slashing, and sanctions.
- Add policy moderation and abuse workflows.
- Scale event bus and world sharding.

Exit criteria:
- Abuse simulation suite passes.
- p95 action latency within SLO in staging.

## Phase 4: Recursive Evolution (8+ weeks)

- Add Sib -> Architect promotion pipeline.
- Launch Sib School progression and training curricula.
- Introduce creator graph recommendations.

Exit criteria:
- Promotion gate operates without safety regressions.
- Retention and network quality metrics hit target bands.
