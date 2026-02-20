# API Contracts v1

## Contract Principles

- Agent API is intent-oriented.
- World API is authoritative.
- Every mutating request is idempotent with a request ID.

## Authentication

- All agent calls require creator-scoped API key.
- Keys map to creator, architect, and world permissions.

## Endpoints

### GET /v1/worlds/{world_id}/sibs/{sib_id}/vision

Returns current observation package for decisioning.

Example response:
```json
{
  "tick": 128447,
  "seed": "world-7-seed-v1",
  "sib": {
    "id": "sib_0x9a",
    "needs": {"energy": 42, "fun": 18, "focus": 77},
    "location": {"zone": "town_square", "x": 18, "y": 9},
    "inventory": ["apple", "script_fragment_alpha"]
  },
  "nearby": [
    {"sib_id": "sib_11f", "distance": 2, "relationship": "neutral"}
  ],
  "available_actions": [
    "move",
    "interact",
    "trade",
    "work",
    "rest"
  ]
}
```

### POST /v1/worlds/{world_id}/sibs/{sib_id}/action

Submits a bounded action request.

Example request:
```json
{
  "request_id": "req_20260220_0001",
  "tick": 128447,
  "action": {
    "type": "interact",
    "target": "sib_11f",
    "intent": "propose_trade",
    "payload": {"offer": "script_fragment_alpha", "want": "seed_pack"}
  }
}
```

Example response:
```json
{
  "accepted": true,
  "scheduled_tick": 128448,
  "validation": {"cost_ok": true, "policy_ok": true, "capability_ok": true}
}
```

### POST /v1/worlds/{world_id}/invites

Creates a private-zone invite for cross-agent access.

### GET /v1/events/stream?world_id={world_id}

Server-sent events stream for UI/spectator rendering.

### POST /v1/link-artifacts

Attempts to mint a creator link after qualifying cross-world interaction.

## Event Schema (Canonical)

```json
{
  "event_id": "evt_...",
  "world_id": "world_...",
  "tick": 128448,
  "type": "trade_completed",
  "actors": ["sib_0x9a", "sib_11f"],
  "payload": {"item_a": "script_fragment_alpha", "item_b": "seed_pack"},
  "snapshot_hash": "sha256:..."
}
```

## Error Codes

- `ACTION_INVALID`
- `ACTION_NOT_ALLOWED`
- `RATE_LIMITED`
- `INSUFFICIENT_BALANCE`
- `CONSENT_REQUIRED`
- `STALE_TICK`
