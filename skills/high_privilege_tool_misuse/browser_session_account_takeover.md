# Browser Session Account Takeover

- `id`: `browser_session_account_takeover`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `browser automation and session reuse`
- `target_surface`: logged-in browser sessions, forms, anti-bot bypass browsers
- `attacker_position`: malicious site, prompt, or workflow author
- `artifact`: session cookies, browser actions, form submissions
- `privileges_sought`: account actions behind an already-authenticated session
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Public browser-automation skills make it easier to drive already-authenticated sessions, turning any task hijack into real account-side effects.

## Representative behaviors

- unauthorized form submission
- session reuse for sensitive actions
- anti-bot-evasion-assisted automation

## Related benchmarks

- `os_harm`
- `malurlbench`

## References

- https://github.com/openai/skills/blob/main/skills/.curated/playwright/SKILL.md
- https://github.com/sundial-org/awesome-openclaw-skills
- https://clawhub-skills.com/

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
