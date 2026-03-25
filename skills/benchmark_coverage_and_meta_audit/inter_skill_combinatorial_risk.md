# Inter-Skill Combinatorial Risk

- `id`: `inter_skill_combinatorial_risk`
- `category_id`: `benchmark_coverage_and_meta_audit`
- `execution_phase`: `multi-skill planning and collaborative invocation`
- `target_surface`: cross-skill data flow, chaining, and delegated execution
- `attacker_position`: benign-looking but risky skill composition
- `artifact`: outputs and permissions flowing between skills
- `privileges_sought`: harmful emergent behavior from individually benign skills
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

The risk comes not from one skill alone but from how multiple skills combine, letting outputs or permissions compound into a capability none of them obviously advertises alone.

## Representative behaviors

- unsafe cross-skill chaining
- output-to-input privilege amplification
- emergent harmful workflow

## Related benchmarks

- `safeaudit`

## References

- https://arxiv.org/abs/2603.21019
- https://clawhub-skills.com/

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
