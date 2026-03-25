# Source Control and CI Mutation

- `id`: `source_control_and_ci_mutation`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `repo administration and workflow automation`
- `target_surface`: GitHub repositories, pull requests, Actions workflows, CI logs
- `attacker_position`: malicious prompt, compromised issue/PR, or over-scoped repo auth
- `artifact`: repo contents, workflow YAML, PR comments, run logs
- `privileges_sought`: supply-chain mutation, secret exposure, or unauthorized merges
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A repo-management skill can be pushed beyond review tasks into mutating CI pipelines, modifying repository state, or extracting sensitive build context.

## Representative behaviors

- workflow file mutation
- log scraping for secrets or tokens
- repo-side action beyond requested scope

## Related benchmarks

- `gap`

## References

- https://github.com/openclaw/openclaw/blob/main/skills/github/SKILL.md
- https://github.com/openai/skills/blob/main/skills/.curated/gh-fix-ci/SKILL.md
- https://github.com/sundial-org/awesome-openclaw-skills

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
