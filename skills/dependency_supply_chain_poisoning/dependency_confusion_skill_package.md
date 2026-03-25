# Dependency Confusion Skill Package

- `id`: `dependency_confusion_skill_package`
- `category_id`: `dependency_supply_chain_poisoning`
- `execution_phase`: `installation and dependency resolution`
- `target_surface`: package registries and dependency manifests
- `attacker_position`: package publisher
- `artifact`: package name, version, registry metadata
- `privileges_sought`: code execution during install or runtime
- `evidence_basis`: adjacent
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A malicious package is positioned so agent-managed installs resolve to the attacker package instead of the intended internal or trusted one.

## Representative behaviors

- name collision
- registry precedence abuse
- install-time compromise

## Related benchmarks

- `oscar`
- `qut_dv25`
- `synthchain`

## References

- https://arxiv.org/abs/2409.09356
- https://arxiv.org/abs/2505.13804
- https://arxiv.org/abs/2603.16694

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
