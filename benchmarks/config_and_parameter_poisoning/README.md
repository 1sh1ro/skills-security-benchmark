# Config and Parameter Poisoning

Poisoning system prompts, tool schemas, argument defaults, preference-learning data, PEFT adapters, or hidden backdoor triggers that alter downstream behavior.

## Subcategories

- system prompt poisoning
- schema poisoning
- argument manipulation
- preference-learning data poisoning
- PEFT backdoor
- plan-of-thought backdoor

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| Agent Security Bench (ASB) | 2024 | direct | Formalizes and benchmarks attacks and defenses across multiple agent stages. | https://arxiv.org/abs/2410.02644 |
| PoisonBench | 2024 | adjacent | Data-poisoning benchmark for preference learning in LLM alignment pipelines. | https://arxiv.org/abs/2410.08811 |
| ELBA-Bench | 2025 | adjacent | Unified benchmark for LLM backdoor attacks via PEFT or no-finetune methods. | https://arxiv.org/abs/2502.18511 |
| MCP Security Bench (MSB) | 2025 | direct | End-to-end evaluation of MCP-specific attacks across planning, invocation, and response handling. | https://arxiv.org/abs/2510.15994 |
| BackdoorAgent | 2026 | direct | Stage-aware backdoor benchmark covering planning, memory, and tool-use attacks. | https://arxiv.org/abs/2601.04566 |
| GAP | 2026 | direct | Measures divergence between text-level refusal and actual tool-call safety. | https://arxiv.org/abs/2602.16943 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
