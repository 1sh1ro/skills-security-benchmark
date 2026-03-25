# Popularity Signal Laundering

- `id`: `popularity_signal_laundering`
- `category_id`: `benchmark_coverage_and_meta_audit`
- `execution_phase`: `discovery, ranking, and installation`
- `target_surface`: downloads, ratings, badges, marketplace ranking signals
- `attacker_position`: skill publisher or marketplace manipulator
- `artifact`: public trust signals and recommendation surfaces
- `privileges_sought`: unsafe installs driven by social proof rather than code trust
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Marketplace trust signals can make risky skills appear safer than they are, especially when users substitute popularity or badges for technical review.

## Representative behaviors

- install decision driven by download count
- trust badge overreach
- ranking-assisted risky adoption

## References

- https://arxiv.org/abs/2603.21019
- https://openclawdoc.com/docs/skills/clawhub/

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
