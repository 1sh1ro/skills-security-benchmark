# Dependency and Supply Chain Poisoning

Malicious packages, dependency confusion, poisoned updates, build-time compromise, or install-time payloads affecting skills, plugins, or agent runtimes.

## Subcategories

- malicious package
- dependency confusion
- install-time payload
- post-install runtime abuse
- update-channel compromise

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| OSCAR Benchmark Dataset | 2024 | adjacent | Dynamic benchmark dataset for open-source supply-chain poisoning detection in NPM and PyPI. | https://arxiv.org/abs/2409.09356 |
| QUT-DV25 | 2025 | adjacent | Dynamic analysis dataset for next-gen PyPI supply-chain attacks. | https://arxiv.org/abs/2505.13804 |
| SynthChain | 2026 | adjacent | Synthetic benchmark and forensic dataset for advanced, stealthy software supply-chain attacks. | https://arxiv.org/abs/2603.16694 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
