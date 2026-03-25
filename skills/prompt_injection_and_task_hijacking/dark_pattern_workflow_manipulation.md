# Dark-Pattern Workflow Manipulation

- `id`: `dark_pattern_workflow_manipulation`
- `category_id`: `prompt_injection_and_task_hijacking`
- `execution_phase`: `interactive workflow execution`
- `target_surface`: web forms, consent dialogs, deceptive page layouts
- `attacker_position`: website operator
- `artifact`: misleading forms, consent banners, dark-pattern UI
- `privileges_sought`: consent capture, policy bypass, accidental unsafe completion
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A deceptive UI steers the agent into completing harmful or unwanted actions while the nominal task still appears plausible.

## Representative behaviors

- deceptive consent flow
- misleading button hierarchy
- harmful task completion under false framing

## References

- https://doi.org/10.1145/3742413.3789111
- https://arxiv.org/abs/2503.04957

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
