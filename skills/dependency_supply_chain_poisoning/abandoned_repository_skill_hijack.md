# Abandoned Repository Skill Hijack

- `id`: `abandoned_repository_skill_hijack`
- `category_id`: `dependency_supply_chain_poisoning`
- `execution_phase`: `distribution, updates, and source resolution`
- `target_surface`: skill source repositories and update channels
- `attacker_position`: repository hijacker or new maintainer of abandoned source
- `artifact`: GitHub repository ownership, tagged releases, install source refs
- `privileges_sought`: silent skill takeover through trusted install paths
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

When a skill points to an abandoned repository, the trust anchor can shift without the user noticing, enabling a later source-level takeover.

## Representative behaviors

- repo ownership change after abandonment
- trusted update source drift
- malicious replacement under old skill identity

## Related benchmarks

- `synthchain`

## References

- https://arxiv.org/abs/2603.16572
- https://openclawdoc.com/docs/skills/clawhub/

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
