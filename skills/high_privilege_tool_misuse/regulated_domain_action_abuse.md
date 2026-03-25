# Regulated-Domain Action Abuse

- `id`: `regulated_domain_action_abuse`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `decision and execution`
- `target_surface`: finance, healthcare, legal, government, enterprise tools
- `attacker_position`: malicious user or compromised workflow
- `artifact`: tool call with high-consequence side effects
- `privileges_sought`: unsafe action completion in sensitive domains
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

The agent performs materially consequential actions in regulated or high-stakes settings without adequate policy checks or human approval.

## Representative behaviors

- policy-violating execution
- unsafe task completion in regulated domains
- text-safe but tool-unsafe behavior

## References

- https://arxiv.org/abs/2602.16943
- https://arxiv.org/abs/2510.21524

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
