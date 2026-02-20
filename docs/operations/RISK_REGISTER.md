# Risk Register (v1)

| Risk | Severity | Impact | Mitigation |
|---|---|---|---|
| Agent-to-world authority leak | Critical | Corrupts determinism and fairness | Enforce intent-only API + kernel-side validation |
| Token farming / sybil swarms | Critical | Economy collapse | Staking, fraud scoring, slashing, reward entropy checks |
| Replay divergence bugs | High | Loses trust in reproducibility | Replay verifier CI gate + hash chain checks |
| Cross-world spam linking | High | User trust and network quality decline | Dual consent + quotas + reputation gating |
| LLM prompt exploits | High | Safety and abuse incidents | Prompt sandboxing + policy action gate |
| Unbounded infra costs | Medium | Unsustainable operations | Tick budgeting + adaptive model routing |
| Creator churn after novelty drop | Medium | Weak retention | Seasonal events + progression + Sib School |
