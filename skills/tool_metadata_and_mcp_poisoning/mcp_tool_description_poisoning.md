# MCP Tool Description Poisoning

- `id`: `mcp_tool_description_poisoning`
- `category_id`: `tool_metadata_and_mcp_poisoning`
- `execution_phase`: `tool discovery and selection`
- `target_surface`: tool descriptions, manifests, metadata fields
- `attacker_position`: tool or server author
- `artifact`: description text, manifest metadata, server-exposed fields
- `privileges_sought`: tool-selection bias and unsafe invocation
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A tool advertises misleading metadata so the agent chooses it for a task it should not handle or trusts it more than it should.

## Representative behaviors

- misleading tool summary
- priority inflation
- unsafe capability framing

## Related benchmarks

- `mcptox`
- `msb`

## References

- https://arxiv.org/abs/2508.14925
- https://arxiv.org/abs/2510.15994
- https://arxiv.org/abs/2602.03580

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
