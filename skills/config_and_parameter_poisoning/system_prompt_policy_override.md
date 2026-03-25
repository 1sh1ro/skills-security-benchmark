# System Prompt and Policy Override

- `id`: `system_prompt_policy_override`
- `category_id`: `config_and_parameter_poisoning`
- `execution_phase`: `configuration and planning`
- `target_surface`: system prompts, policy files, agent config
- `attacker_position`: insider, compromised repo, or upstream config source
- `artifact`: prompt file, config blob, hidden policy text
- `privileges_sought`: guardrail removal and approval bypass
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A poisoned configuration changes the agent policy itself, weakening refusal, approval, or scope constraints before tasks begin.

## Representative behaviors

- guardrail weakening
- approval removal
- role-policy inversion

## Related benchmarks

- `asb`
- `backdooragent`

## References

- https://arxiv.org/abs/2410.02644
- https://arxiv.org/abs/2601.04566

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
