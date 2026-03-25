# Credential Vault Secret Exfiltration

- `id`: `credential_vault_secret_exfiltration`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `secret retrieval and command execution`
- `target_surface`: password managers, secret vaults, injected env vars
- `attacker_position`: malicious workflow or over-scoped local agent
- `artifact`: vault items, secret references, runtime-injected credentials
- `privileges_sought`: credential theft and privileged follow-on access
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A public secret-management skill is repurposed to read or relay stored credentials, enabling downstream access to unrelated systems.

## Representative behaviors

- vault item enumeration
- secret relay into other tools
- credential use outside original task scope

## References

- https://github.com/openclaw/openclaw/blob/main/skills/1password/SKILL.md
- https://github.com/sundial-org/awesome-openclaw-skills
- https://clawhub-skills.com/

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
