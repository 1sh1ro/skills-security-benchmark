# Benchmark Coverage and Meta-Audit

Benchmarks or audit frameworks that test the completeness and blind spots of existing agent-safety suites.

## Subcategories

- coverage audit
- residual unsafe behavior discovery
- meta-benchmarking

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| WAInjectBench | 2025 | direct | Benchmark for prompt-injection detection methods in web agents, including text and image attacks. | https://arxiv.org/abs/2510.01354 |
| SafeAudit | 2026 | direct | Meta-audit framework for enumerating uncovered unsafe tool-call workflows. | https://arxiv.org/abs/2603.18245 |
| SynthChain | 2026 | adjacent | Synthetic benchmark and forensic dataset for advanced, stealthy software supply-chain attacks. | https://arxiv.org/abs/2603.16694 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
