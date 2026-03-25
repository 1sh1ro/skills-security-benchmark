# Tool Metadata and MCP Poisoning

Attacks that poison tool descriptions, MCP metadata, manifests, names, or response channels before or during tool selection and invocation.

## Subcategories

- tool description poisoning
- name collision
- user impersonation
- false error escalation
- tool transfer
- retrieval injection

## Mapped benchmarks

| Benchmark | Year | Tier | Focus | Source |
| --- | --- | --- | --- | --- |
| MCP Security Bench (MSB) | 2025 | direct | End-to-end evaluation of MCP-specific attacks across planning, invocation, and response handling. | https://arxiv.org/abs/2510.15994 |
| MCP-SafetyBench | 2025 | direct | Multi-turn safety benchmark on real MCP servers with cross-server workflows. | https://arxiv.org/abs/2512.15163 |
| MCPTox | 2025 | direct | Systematic benchmark for MCP tool poisoning via malicious metadata without execution. | https://arxiv.org/abs/2508.14925 |
| RAS-Eval | 2025 | direct | Comprehensive security benchmark supporting simulated and real-world tool execution. | https://arxiv.org/abs/2506.15253 |

## Contribution notes

- Add a new benchmark here when it directly evaluates this threat family or a clearly adjacent transfer setting.
- Keep exploit details abstract; store benchmark metadata, scope, and links instead of ready-to-run harmful payloads.
- If a benchmark spans multiple families, keep the canonical metadata in `data/benchmark_catalog.json` and reference it from each relevant category.
