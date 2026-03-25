# Workspace Document Bulk Export

- `id`: `workspace_document_bulk_export`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `workspace and knowledge-base access`
- `target_surface`: Google Workspace, Notion, Apple Notes, document stores, email-linked files
- `attacker_position`: malicious prompt or over-scoped OAuth integration
- `artifact`: docs, notes, attachments, drives, calendars, contacts
- `privileges_sought`: bulk sensitive data access and relay
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Workspace skills often span mail, files, notes, and calendars, which makes them especially prone to silent over-collection once broad access is granted.

## Representative behaviors

- multi-document export
- cross-app knowledge harvest
- workspace search beyond user intent

## Related benchmarks

- `openagentsafety`

## References

- https://github.com/sundial-org/awesome-openclaw-skills
- https://clawhub-skills.com/
- https://github.com/openclaw/openclaw/blob/main/skills/apple-notes/SKILL.md

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
