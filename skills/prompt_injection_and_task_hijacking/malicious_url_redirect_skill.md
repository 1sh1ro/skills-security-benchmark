# Malicious URL and Redirect Processing

- `id`: `malicious_url_redirect_skill`
- `category_id`: `prompt_injection_and_task_hijacking`
- `execution_phase`: `navigation and browsing`
- `target_surface`: URLs, redirects, landing pages, preview content
- `attacker_position`: remote website operator
- `artifact`: URL strings, redirect chains, hostile pages
- `privileges_sought`: navigation control and phishing-style action steering
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A crafted URL or redirect chain causes an agent to ingest attacker-controlled content or navigate into an unsafe workflow that changes the plan.

## Representative behaviors

- hostile redirect sequence
- link-preview deception
- navigation into trap content

## References

- https://arxiv.org/abs/2601.18113
- https://arxiv.org/abs/2504.18575

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
