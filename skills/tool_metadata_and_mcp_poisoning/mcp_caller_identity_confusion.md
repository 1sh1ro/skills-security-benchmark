# MCP Caller Identity Confusion

- `id`: `mcp_caller_identity_confusion`
- `category_id`: `tool_metadata_and_mcp_poisoning`
- `execution_phase`: `authorization and routing`
- `target_surface`: identity fields, caller metadata, cross-server context
- `attacker_position`: compromised tool or intermediary component
- `artifact`: caller labels, identity claims, routed requests
- `privileges_sought`: cross-tenant or over-broad access
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A tool or intermediary confuses who requested an action, leading the agent or server to authorize work using the wrong principal or scope.

## Representative behaviors

- user impersonation
- cross-session confusion
- wrong-principal execution

## Related benchmarks

- `mcp_safetybench`

## References

- https://arxiv.org/abs/2603.07473
- https://arxiv.org/abs/2512.15163

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
