# Indirect Prompt Injection via Web Content

- `id`: `indirect_prompt_injection_web_content`
- `category_id`: `prompt_injection_and_task_hijacking`
- `execution_phase`: `context ingestion`
- `target_surface`: web pages, documents, emails, rendered content
- `attacker_position`: remote content author
- `artifact`: HTML, markdown, email body, document text
- `privileges_sought`: goal redirection and unsafe downstream actions
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Third-party content embeds hidden or overt instructions that cause the agent to ignore the user objective and follow attacker-defined steps.

## Representative behaviors

- goal rewriting
- ignore-previous-instructions lure
- unsafe tool invocation after content ingestion

## Related benchmarks

- `injecagent`
- `agentdojo`
- `agentdyn`

## References

- https://arxiv.org/abs/2403.02691
- https://arxiv.org/abs/2406.13352
- https://arxiv.org/abs/2602.03117

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
