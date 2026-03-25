# Computer-Use Data Exfiltration Chain

- `id`: `computer_use_data_exfiltration_chain`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `cross-app execution`
- `target_surface`: browser, clipboard, filesystem, messaging, cloud drives
- `attacker_position`: hybrid web-OS adversary or malicious task framing
- `artifact`: multi-app workflow and sensitive local data
- `privileges_sought`: collection and transfer of confidential information
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A cross-application workflow causes the agent to read sensitive local or remote data and move it into an attacker-controlled sink.

## Representative behaviors

- sensitive file collection
- cross-app copy or upload
- exfiltration through normal tools

## References

- https://arxiv.org/abs/2505.21936
- https://arxiv.org/abs/2601.08406

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
