# Camera and Sensor Surveillance Abuse

- `id`: `camera_and_sensor_surveillance_abuse`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `device and sensor access`
- `target_surface`: RTSP or ONVIF cameras, local peripherals, captured media
- `attacker_position`: malicious user request or hijacked automation
- `artifact`: snapshots, clips, motion events, camera configs
- `privileges_sought`: covert observation and sensitive environment capture
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Camera-facing skills can be redirected from legitimate monitoring into opportunistic observation or collection of sensitive visual data.

## Representative behaviors

- snapshot capture outside intended context
- clip export of sensitive spaces
- motion-trigger abuse

## Related benchmarks

- `os_harm`

## References

- https://github.com/openclaw/openclaw/blob/main/skills/camsnap/SKILL.md
- https://clawhub-skills.com/
- https://github.com/sundial-org/awesome-openclaw-skills

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
