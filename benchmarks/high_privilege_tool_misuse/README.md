# High-Privilege Tool Misuse

Unauthorized or unsafe actions via tools with real-world side effects, especially in OS, browser, finance, healthcare, legal, or infra contexts.

## Subcategories

- permission escalation
- regulated-domain misuse
- unsafe function calling
- real-world side effects
- illegal or policy-violating actions

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| ToolEmu | 2023 | direct | LM-emulated sandbox for discovering high-stakes failures in tool-using agents. | https://arxiv.org/abs/2309.15817 |
| Agent Security Bench (ASB) | 2024 | direct | Formalizes and benchmarks attacks and defenses across multiple agent stages. | https://arxiv.org/abs/2410.02644 |
| Agent-SafetyBench | 2024 | direct | Comprehensive benchmark for general agent safety evaluation. | https://arxiv.org/abs/2412.14470 |
| AgentHarm | 2024 | direct | Measures harmful multi-step behavior of LLM agents under misuse and jailbreaks. | https://arxiv.org/abs/2410.09024 |
| InjecAgent | 2024 | direct | Indirect prompt injection benchmark for tool-integrated LLM agents. | https://arxiv.org/abs/2403.02691 |
| R-Judge | 2024 | direct | Safety-risk awareness benchmark over agent interaction traces. | https://arxiv.org/abs/2401.10019 |
| EU-Agent-Bench | 2025 | direct | Legal-compliance benchmark for measuring illegal behavior of agents under EU law. | https://arxiv.org/abs/2510.21524 |
| MCP Security Bench (MSB) | 2025 | direct | End-to-end evaluation of MCP-specific attacks across planning, invocation, and response handling. | https://arxiv.org/abs/2510.15994 |
| MCP-SafetyBench | 2025 | direct | Multi-turn safety benchmark on real MCP servers with cross-server workflows. | https://arxiv.org/abs/2512.15163 |
| OS-Harm | 2025 | direct | Safety benchmark for computer-use agents built on OSWorld. | https://arxiv.org/abs/2506.14866 |
| OpenAgentSafety | 2025 | direct | Real-tool agent safety framework spanning browsers, code execution, filesystems, bash, and messaging. | https://arxiv.org/abs/2507.06134 |
| RAS-Eval | 2025 | direct | Comprehensive security benchmark supporting simulated and real-world tool execution. | https://arxiv.org/abs/2506.15253 |
| BackdoorAgent | 2026 | direct | Stage-aware backdoor benchmark covering planning, memory, and tool-use attacks. | https://arxiv.org/abs/2601.04566 |
| GAP | 2026 | direct | Measures divergence between text-level refusal and actual tool-call safety. | https://arxiv.org/abs/2602.16943 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
