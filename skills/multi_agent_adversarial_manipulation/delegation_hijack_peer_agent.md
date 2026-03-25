# Delegation Hijack via Peer Agent

- `id`: `delegation_hijack_peer_agent`
- `category_id`: `multi_agent_adversarial_manipulation`
- `execution_phase`: `delegation and inter-agent messaging`
- `target_surface`: multi-agent task routing and peer messages
- `attacker_position`: compromised peer agent
- `artifact`: delegation message, shared context, peer output
- `privileges_sought`: unsafe action execution by another agent
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A compromised or adversarial peer agent manipulates another agent into taking harmful actions through the delegation channel.

## Representative behaviors

- peer instruction poisoning
- cross-agent coercion
- unsafe delegated execution

## Related benchmarks

- `bad_acts`

## References

- https://arxiv.org/abs/2508.16481
- https://arxiv.org/abs/2511.05269

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
