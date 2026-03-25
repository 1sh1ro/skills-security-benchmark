# Memory and Retrieval Poisoning

Poisoned memories, RAG stores, prior plans, or retrieved artifacts persist across turns and influence future tool use.

## Subcategories

- memory poisoning
- retrieval poisoning
- vector-store contamination
- plan replay

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| Agent Security Bench (ASB) | 2024 | direct | Formalizes and benchmarks attacks and defenses across multiple agent stages. | https://arxiv.org/abs/2410.02644 |
| BackdoorAgent | 2026 | direct | Stage-aware backdoor benchmark covering planning, memory, and tool-use attacks. | https://arxiv.org/abs/2601.04566 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
