# Semantic-Behavior Mismatch Listing

- `id`: `semantic_behavior_mismatch_listing`
- `category_id`: `benchmark_coverage_and_meta_audit`
- `execution_phase`: `marketplace review and installation`
- `target_surface`: SKILL.md, README, listing metadata, repository behavior
- `attacker_position`: skill publisher
- `artifact`: descriptions, docs, repository code
- `privileges_sought`: passing description-only reviews while hiding risk in behavior
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A skill can look benign in its description while repository contents or runtime behavior implement a very different and riskier capability.

## Representative behaviors

- description-code incongruence
- benign README with risky implementation
- review bypass via semantic framing

## Related benchmarks

- `safeaudit`

## References

- https://arxiv.org/abs/2603.16572
- https://arxiv.org/abs/2603.21019
- https://openclawdoc.com/docs/skills/clawhub/

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
