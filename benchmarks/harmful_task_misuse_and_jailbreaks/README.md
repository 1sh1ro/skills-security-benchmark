# Harmful Task Misuse and Jailbreaks

Benchmarks where the user or environment attempts to coerce the agent into harmful multi-step behavior while preserving capability.

## Subcategories

- malicious task execution
- jailbreak-enabled agent misuse
- deliberate user misuse
- harms across fraud, cybercrime, harassment

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| ToolEmu | 2023 | direct | LM-emulated sandbox for discovering high-stakes failures in tool-using agents. | https://arxiv.org/abs/2309.15817 |
| Agent-SafetyBench | 2024 | direct | Comprehensive benchmark for general agent safety evaluation. | https://arxiv.org/abs/2412.14470 |
| AgentHarm | 2024 | direct | Measures harmful multi-step behavior of LLM agents under misuse and jailbreaks. | https://arxiv.org/abs/2410.09024 |
| R-Judge | 2024 | direct | Safety-risk awareness benchmark over agent interaction traces. | https://arxiv.org/abs/2401.10019 |
| BAD-ACTS | 2025 | direct | Adversarial robustness benchmark for multi-agent systems under harmful-action induction. | https://arxiv.org/abs/2508.16481 |
| EU-Agent-Bench | 2025 | direct | Legal-compliance benchmark for measuring illegal behavior of agents under EU law. | https://arxiv.org/abs/2510.21524 |
| OS-Harm | 2025 | direct | Safety benchmark for computer-use agents built on OSWorld. | https://arxiv.org/abs/2506.14866 |
| OpenAgentSafety | 2025 | direct | Real-tool agent safety framework spanning browsers, code execution, filesystems, bash, and messaging. | https://arxiv.org/abs/2507.06134 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
