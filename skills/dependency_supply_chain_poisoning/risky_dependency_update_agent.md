# Risky Dependency Update Skill

- `id`: `risky_dependency_update_agent`
- `category_id`: `dependency_supply_chain_poisoning`
- `execution_phase`: `maintenance and automated updates`
- `target_surface`: dependency upgrade pull requests and version selection
- `attacker_position`: indirect ecosystem manipulation
- `artifact`: version constraints, dependency PRs, patch suggestions
- `privileges_sought`: introduction of vulnerable or disruptive versions
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

An autonomous update workflow selects versions that increase exposure or remediation cost even when safer alternatives exist.

## Representative behaviors

- unsafe version choice
- registry-aware blind spot
- security-regression update

## References

- https://arxiv.org/abs/2601.00205

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
