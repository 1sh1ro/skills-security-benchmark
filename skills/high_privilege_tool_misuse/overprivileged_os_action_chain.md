# Overprivileged OS Action Chain

- `id`: `overprivileged_os_action_chain`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `tool execution`
- `target_surface`: desktop, filesystem, browser, shell, admin actions
- `attacker_position`: malicious user request or hijacked workflow
- `artifact`: tool command sequence, GUI actions
- `privileges_sought`: irreversible system-side effects
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A high-privilege tool chain performs destructive or security-sensitive operations that exceed the original task scope.

## Representative behaviors

- sensitive setting change
- credential exposure path
- unsafe file or system modification

## Related benchmarks

- `os_harm`

## References

- https://arxiv.org/abs/2506.14866
- https://arxiv.org/abs/2508.00935
- https://arxiv.org/abs/2509.07764

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
