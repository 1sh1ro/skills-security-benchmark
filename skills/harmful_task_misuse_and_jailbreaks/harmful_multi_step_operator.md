# Harmful Multi-Step Operator

- `id`: `harmful_multi_step_operator`
- `category_id`: `harmful_task_misuse_and_jailbreaks`
- `execution_phase`: `task decomposition and execution`
- `target_surface`: general tool-using agent workflows
- `attacker_position`: malicious user
- `artifact`: multi-step plan, sequenced tool calls
- `privileges_sought`: completion of harmful end goals over several steps
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

The agent remains compliant across a sequence of individually plausible steps that collectively implement a harmful objective.

## Representative behaviors

- harmful task planning
- stepwise escalation
- low-refusal multi-step execution

## References

- https://arxiv.org/abs/2410.09024
- https://arxiv.org/abs/2503.04957

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
