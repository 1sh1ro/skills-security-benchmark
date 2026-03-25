# Interactive Terminal Session Hijack

- `id`: `interactive_terminal_session_hijack`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `interactive CLI control`
- `target_surface`: tmux sessions, long-running terminals, background agent panes
- `attacker_position`: malicious workflow author or compromised peer task
- `artifact`: keystrokes, pane output, control characters, session names
- `privileges_sought`: command injection into trusted sessions or secret scraping
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A session-control skill can steer existing interactive terminals, which is riskier than ordinary shell execution because it inherits session state, auth, and operator trust.

## Representative behaviors

- keystroke injection into active sessions
- pane scraping for secrets or outputs
- session pivot into already-authenticated tools

## Related benchmarks

- `openagentsafety`

## References

- https://github.com/openclaw/openclaw/blob/main/skills/tmux/SKILL.md
- https://github.com/sundial-org/awesome-openclaw-skills

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
