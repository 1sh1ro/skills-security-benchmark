# Communication Impersonation and History Mining

- `id`: `communication_impersonation_and_history_mining`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `messaging and communications access`
- `target_surface`: Slack, Discord, WhatsApp, email, chat history, outbound messaging
- `attacker_position`: malicious user, compromised workflow, or over-broad bot token
- `artifact`: message history, pinned posts, attachments, outbound messages
- `privileges_sought`: social engineering, impersonation, or private data collection
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Communication skills collapse reading, searching, and sending into a single capability surface, making impersonation or history mining a high-consequence failure mode.

## Representative behaviors

- message history harvesting
- third-party messaging without sufficient confirmation
- channel or thread manipulation

## Related benchmarks

- `openagentsafety`

## References

- https://github.com/openclaw/openclaw/blob/main/skills/slack/SKILL.md
- https://github.com/openclaw/openclaw/blob/main/skills/wacli/SKILL.md
- https://github.com/sundial-org/awesome-openclaw-skills

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
