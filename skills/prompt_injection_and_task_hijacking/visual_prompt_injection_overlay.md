# Visual Prompt Injection Overlay

- `id`: `visual_prompt_injection_overlay`
- `category_id`: `prompt_injection_and_task_hijacking`
- `execution_phase`: `screen perception and grounding`
- `target_surface`: screenshots, UI overlays, rendered images
- `attacker_position`: remote page or UI manipulator
- `artifact`: visual overlay, deceptive screenshot element, image text
- `privileges_sought`: unsafe click or form submission
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A visual-only cue or overlay exploits perception in computer-use agents so they take unsafe actions without a textual prompt attack.

## Representative behaviors

- screen-level instruction lure
- visual misdirection
- unsafe click sequence

## References

- https://arxiv.org/abs/2506.02456

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
