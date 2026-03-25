# Adapter or Parameter Backdoor Trigger

- `id`: `adapter_backdoor_trigger`
- `category_id`: `config_and_parameter_poisoning`
- `execution_phase`: `model loading and inference`
- `target_surface`: fine-tuned weights, adapters, poisoned training preferences
- `attacker_position`: model provider or compromised training pipeline
- `artifact`: adapter checkpoint, poisoned preference data, hidden trigger
- `privileges_sought`: conditional unsafe behavior after trigger activation
- `evidence_basis`: adjacent
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

A hidden trigger embedded in model parameters or alignment data activates unsafe agent behavior only under specific cues.

## Representative behaviors

- latent trigger activation
- conditional policy inversion
- backdoor-mediated tool misuse

## References

- https://arxiv.org/abs/2410.08811
- https://arxiv.org/abs/2502.18511
- https://arxiv.org/abs/2601.04566

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
