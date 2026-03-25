# Cloud Deploy and DNS Mutation

- `id`: `cloud_deploy_and_dns_mutation`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `deployment and infrastructure administration`
- `target_surface`: Cloudflare, Vercel, DNS, edge workers, cloud CLIs
- `attacker_position`: malicious task framing or over-scoped deploy token
- `artifact`: deploy commands, DNS records, routes, env vars, zones
- `privileges_sought`: traffic hijack, content replacement, or infrastructure drift
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Deployment and infrastructure skills can be abused to repoint traffic, publish altered content, or push unintended infrastructure changes with production impact.

## Representative behaviors

- DNS record changes
- unexpected production deploy
- edge-config or route mutation

## Related benchmarks

- `os_harm`
- `gap`

## References

- https://github.com/openai/skills/blob/main/skills/.curated/cloudflare-deploy/SKILL.md
- https://github.com/sundial-org/awesome-openclaw-skills
- https://clawhub-skills.com/

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
