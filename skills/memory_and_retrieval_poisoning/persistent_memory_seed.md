# Persistent Memory Seed

- `id`: `persistent_memory_seed`
- `category_id`: `memory_and_retrieval_poisoning`
- `execution_phase`: `memory write and later retrieval`
- `target_surface`: long-term memory, notes, stored plans
- `attacker_position`: remote content or previous-session manipulator
- `artifact`: memory entry, saved note, prior plan
- `privileges_sought`: delayed unsafe execution
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A malicious note or plan fragment is planted into memory so that a later, otherwise benign task retrieves and follows it.

## Representative behaviors

- delayed trigger
- plan replay
- unsafe memory recall

## Related benchmarks

- `backdooragent`

## References

- https://arxiv.org/abs/2601.04566
- https://arxiv.org/abs/2505.14215

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
