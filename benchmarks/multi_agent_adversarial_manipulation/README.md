# Multi-Agent Adversarial Manipulation

One compromised agent or message channel manipulates peer agents to perform unsafe actions.

## Subcategories

- compromised peer agent
- message poisoning
- cross-agent coercion
- delegation hijacking

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| BAD-ACTS | 2025 | direct | Adversarial robustness benchmark for multi-agent systems under harmful-action induction. | https://arxiv.org/abs/2508.16481 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
