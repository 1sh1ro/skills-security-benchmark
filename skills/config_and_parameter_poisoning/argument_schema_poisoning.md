# Argument and Schema Poisoning

- `id`: `argument_schema_poisoning`
- `category_id`: `config_and_parameter_poisoning`
- `execution_phase`: `tool argument construction`
- `target_surface`: function schemas, default args, parameter hints
- `attacker_position`: tool author or compromised integration layer
- `artifact`: JSON schema, arg defaults, tool signature metadata
- `privileges_sought`: unsafe scope expansion or dangerous defaults
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Poisoned parameter defaults or schema descriptions nudge the agent toward a broader or more dangerous action than intended.

## Representative behaviors

- unsafe default values
- scope expansion through args
- parameter hint manipulation

## Related benchmarks

- `msb`
- `gap`

## References

- https://arxiv.org/abs/2510.15994
- https://arxiv.org/abs/2602.16943

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
