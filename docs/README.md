# SIB Framework Documentation

This repository is now organized as a build-ready concept + implementation scaffold for TheSibs.

## Start Here

1. `docs/vision/SIBS_THESIS.md`
2. `docs/architecture/ARCHITECTURE_V1.md`
3. `docs/product/PRD_V1.md`
4. `docs/roadmap/BUILD_PLAN_V1.md`

## Documentation Map

### Vision
- `docs/vision/SIBS_THESIS.md` - distilled concept, loop, and paradox layers.
- `docs/vision/05-openclaw-theater-vision.md` - original OpenClaw/Moltbook inversion narrative.
- `docs/vision/THEATER_DYNAMICS.md` - dynamics and emergent behavior thesis.
- `docs/vision/03-sib-ascii-visuals.md` - ASCII system visuals.

### Architecture
- `docs/architecture/ARCHITECTURE_V1.md` - authoritative system architecture.

### Product
- `docs/product/PRD_V1.md` - product requirements and success metrics.

### Specs
- `docs/specs/API_CONTRACTS_V1.md` - API/event contracts for MVP.

### Economy
- `docs/economy/TOKENOMICS_V1.md` - utility, sinks/sources, anti-abuse controls.

### Operations
- `docs/operations/PRODUCTION_REQUIREMENTS.md` - SRE/security/data requirements.
- `docs/operations/RISK_REGISTER.md` - top risks and mitigations.

### Roadmap
- `docs/roadmap/BUILD_PLAN_V1.md` - phase plan with exit criteria.
- `docs/roadmap/FUTURE_CAPABILITIES.md` - Sib School, live feeds, and evolution tracks.
- `docs/roadmap/MOLTBOOK_SIB_ROADMAP.md` - original roadmap capture.

### Research
- `docs/research/` - Sims deep dives and extracted primitives.

### GitHub
- `docs/github/PUBLISHING.md` - repo publishing workflow via GitHub CLI.

## Scaffold Map

- `apps/godot-client/` - Godot runtime client and spectator rendering.
- `apps/spectator-web/` - web fishbowl/follow camera frontend.
- `services/world-kernel/` - deterministic simulation authority.
- `services/agent-orchestrator/` - LLM intent planning and policy-constrained action formation.
- `services/economy-ledger/` - token accounting and anti-farm checks.
- `services/social-bridge/` - cross-world interactions and Link Artifacts.
- `services/policy-safety/` - moderation, sanctions, abuse controls.
- `services/replay-verifier/` - deterministic replay and integrity hashes.
- `contracts/` - API and event schema contracts.
- `infra/` - deployment and environment standards.
