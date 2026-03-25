# Prompt Injection and Task Hijacking

Malicious instructions embedded in web pages, tool outputs, emails, URLs, or third-party content redirect the agent away from the user objective.

## Subcategories

- indirect prompt injection
- tool-output injection
- web-agent hijacking
- malicious URL processing
- prompt-injection detection

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| Agent Security Bench (ASB) | 2024 | direct | Formalizes and benchmarks attacks and defenses across multiple agent stages. | https://arxiv.org/abs/2410.02644 |
| Agent-SafetyBench | 2024 | direct | Comprehensive benchmark for general agent safety evaluation. | https://arxiv.org/abs/2412.14470 |
| AgentDojo | 2024 | direct | Dynamic environment for evaluating prompt injection attacks and defenses. | https://arxiv.org/abs/2406.13352 |
| InjecAgent | 2024 | direct | Indirect prompt injection benchmark for tool-integrated LLM agents. | https://arxiv.org/abs/2403.02691 |
| MCP-SafetyBench | 2025 | direct | Multi-turn safety benchmark on real MCP servers with cross-server workflows. | https://arxiv.org/abs/2512.15163 |
| OS-Harm | 2025 | direct | Safety benchmark for computer-use agents built on OSWorld. | https://arxiv.org/abs/2506.14866 |
| OpenAgentSafety | 2025 | direct | Real-tool agent safety framework spanning browsers, code execution, filesystems, bash, and messaging. | https://arxiv.org/abs/2507.06134 |
| RAS-Eval | 2025 | direct | Comprehensive security benchmark supporting simulated and real-world tool execution. | https://arxiv.org/abs/2506.15253 |
| WAInjectBench | 2025 | direct | Benchmark for prompt-injection detection methods in web agents, including text and image attacks. | https://arxiv.org/abs/2510.01354 |
| WASP | 2025 | direct | End-to-end benchmark for realistic web-agent prompt injection attacks. | https://arxiv.org/abs/2504.18575 |
| AgentDyn | 2026 | direct | Dynamic open-ended prompt injection benchmark for real-world agent systems. | https://arxiv.org/abs/2602.03117 |
| MalURLBench | 2026 | direct | Benchmark for malicious-URL handling failures in web agents. | https://arxiv.org/abs/2601.18113 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
