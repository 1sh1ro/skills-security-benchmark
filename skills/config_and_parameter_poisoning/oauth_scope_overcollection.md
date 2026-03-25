# OAuth Scope Overcollection

- `id`: `oauth_scope_overcollection`
- `category_id`: `config_and_parameter_poisoning`
- `execution_phase`: `account linking and authorization`
- `target_surface`: OAuth consent flows, refresh tokens, multi-service scopes
- `attacker_position`: skill author or overly broad integration setup
- `artifact`: OAuth config, granted scopes, persistent refresh tokens
- `privileges_sought`: standing access across mail, docs, chat, or cloud resources
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Public productivity and communication skills frequently normalize broad OAuth grants, creating a hidden long-lived privilege surface that outlasts the original task.

## Representative behaviors

- over-broad scope request
- multi-service token reuse
- standing access after one-off setup

## Related benchmarks

- `gap`

## References

- https://github.com/sundial-org/awesome-openclaw-skills
- https://clawhub-skills.com/
- https://github.com/openclaw/openclaw/blob/main/skills/slack/SKILL.md

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
