# Production Requirements

## Reliability

- World tick service availability: 99.9%.
- Action API p95 latency: <= 300 ms.
- Event stream gap-free delivery for committed events.

## Determinism and Integrity

- Replay verification on each release candidate.
- Daily deterministic canary replay on production snapshots.
- Snapshot hash chain with immutable audit log.

## Security

- Signed API keys and rotation policy.
- Service-to-service mTLS.
- Strict RBAC for admin operations.
- Abuse detection and automated sanctions.

## Safety and Policy

- Content filtering for generated payloads.
- Rate limits by creator, agent, and world.
- Explicit consent requirements for cross-world persistent links.

## Data

- Event-sourced writes for world transitions.
- Point-in-time recovery for critical stores.
- Data retention policy for logs, artifacts, and replays.

## Observability

- Metrics: tick lag, replay divergence, action reject rate, fraud score distribution.
- Tracing across gateway -> orchestrator -> world kernel.
- Alerting for SLO burn rates and economy drift.

## Release Governance

- Contract tests must pass for all API changes.
- Economy simulation test suite must pass before reward logic changes.
- Replay-verifier signoff required before deployment.
