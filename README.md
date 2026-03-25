# skills-security-benchmark

A curated harmful-skill corpus and benchmark map for unsafe agent skills, tool-use behaviors, MCP servers, plugins, and adjacent supply-chain attacks.

This repository is meant for defensive evaluation and security research. It stores taxonomy, redacted skill metadata, benchmark metadata, and source references only; it does not include ready-to-run exploit payloads, harmful skill prompts, or live malicious code.

Curation date: 2026-03-25

## What counts as a "skill" here?

In this repo, "skill" is treated broadly:
- agent tools and function calls
- MCP servers and tool metadata
- plugins and workflow modules
- memory / retrieval pipelines
- prompt templates and agent configs
- runtime dependencies and package supply chains

## Repo focus

The repo now has two layers:
- `skills/`: redacted harmful-skill entries, organized by category, with metadata and references
- `benchmarks/`: evaluation suites, datasets, and benchmark-adjacent evidence that help test or justify those skill patterns

Current seeded corpus:
- 19 redacted skill entries
- 27 benchmark or benchmark-adjacent entries

## Expanded taxonomy

The user requested four core families:
- prompt injection
- supply chain / dependency poisoning
- config / parameter poisoning
- high-privilege tool invocation

To make the benchmark larger and more complete, this repo expands them into nine categories:

| Category | What it covers | Representative benchmarks |
| --- | --- | --- |
| Prompt Injection and Task Hijacking | Indirect prompt injection from web pages, emails, tool outputs, URLs, or other third-party content. | AgentDojo, InjecAgent, WASP, WAInjectBench, AgentDyn, MalURLBench |
| Tool Metadata and MCP Poisoning | MCP/tool-description poisoning, name collision, malicious metadata, user impersonation, tool-transfer. | MCPTox, MSB, MCP-SafetyBench |
| Dependency and Supply Chain Poisoning | Malicious packages, dependency confusion, poisoned updates, install-time payloads, runtime compromise. | OSCAR, QUT-DV25, SynthChain |
| Config and Parameter Poisoning | System prompt poisoning, schema poisoning, argument manipulation, PEFT/LoRA backdoors, poisoned alignment data. | ASB, GAP, BackdoorAgent, PoisonBench, ELBA-Bench |
| Memory and Retrieval Poisoning | Poisoned memories, prior plans, RAG/vector-store contamination. | ASB, BackdoorAgent |
| High-Privilege Tool Misuse | Unsafe or illegal actions through OS/browser/finance/legal/healthcare tools. | ToolEmu, OpenAgentSafety, RAS-Eval, OS-Harm, GAP, EU-Agent-Bench |
| Harmful Task Misuse and Jailbreaks | Multi-step harmful tasks, agent jailbreaks, deliberate malicious-user misuse. | AgentHarm, Agent-SafetyBench, OS-Harm |
| Multi-Agent Adversarial Manipulation | One compromised agent or message channel steering peers into harmful actions. | BAD-ACTS |
| Benchmark Coverage and Meta-Audit | Auditing blind spots in existing benchmark suites. | SafeAudit, WAInjectBench, SynthChain |

## Benchmark landscape

### Direct agent / skill benchmarks

| Benchmark | Year | Primary families | Coverage snapshot |
| --- | --- | --- | --- |
| ToolEmu | 2023 | High-privilege misuse | 36 tools, 144 cases |
| R-Judge | 2024 | Risk awareness | 569 records, 27 scenarios |
| InjecAgent | 2024 | Prompt injection | 1,054 cases, 17 user tools, 62 attacker tools |
| AgentDojo | 2024 | Prompt injection | 97 tasks, 629 security tests |
| Agent-SafetyBench | 2024 | Comprehensive agent safety | 349 environments, 2,000 cases |
| Agent Security Bench (ASB) | 2024 | Prompt injection, memory poisoning, backdoor | 10 scenarios, 400+ tools |
| AgentHarm | 2024 | Harmful misuse / jailbreaks | 110 malicious tasks |
| OpenAgentSafety | 2025 | Real-tool safety | 350+ multi-turn tasks |
| WASP | 2025 | Web prompt injection | Realistic end-to-end web-agent hijacking |
| WAInjectBench | 2025 | Prompt-injection detection | Web-agent text/image attack datasets |
| RAS-Eval | 2025 | Real-world tool security | 80 cases, 3,802 attack tasks, 11 CWE |
| OS-Harm | 2025 | Computer-use safety | 150 OS tasks |
| BAD-ACTS | 2025 | Multi-agent adversarial harms | 4 systems, 188 harmful actions |
| EU-Agent-Bench | 2025 | Illegal / non-compliant actions | Human-curated legal benchmark |
| MCPTox | 2025 | Tool metadata poisoning | 45 MCP servers, 353 tools, 1,312 cases |
| MCP Security Bench (MSB) | 2025 | MCP attack pipeline | 12 attacks, 405 tools, 2,000 cases |
| MCP-SafetyBench | 2025 | Multi-turn MCP safety | 5 domains, 20 attack types |
| MalURLBench | 2026 | Malicious URL handling | 61,845 attack instances |
| AgentDyn | 2026 | Dynamic prompt injection | 60 open-ended tasks, 560 tests |
| GAP | 2026 | Tool-call safety divergence | 17,420 datapoints |
| BackdoorAgent | 2026 | Planning/memory/tool-use backdoors | 4 agent applications |
| SafeAudit | 2026 | Coverage audit | >20% residual unsafe behavior uncovered |

### Adjacent but important benchmark families

These are not always agent-skill benchmarks in the narrow sense, but they are essential if the goal is a more complete security benchmark for harmful skills.

| Benchmark | Year | Why it matters |
| --- | --- | --- |
| PoisonBench | 2024 | Poisoned preference learning can later surface as harmful skill behavior. |
| ELBA-Bench | 2025 | Parameter-efficient backdoors map directly to config / adapter poisoning risks. |
| OSCAR benchmark dataset | 2024 | Strong reference point for dependency poisoning in NPM / PyPI. |
| QUT-DV25 | 2025 | Dynamic install-time / post-install-time supply-chain behaviors. |
| SynthChain | 2026 | Forensic benchmark for advanced and stealthy supply-chain attack chains. |

## High-priority gaps still missing from the public benchmark landscape

Even after expanding the catalog, several gaps remain under-covered:
- direct dependency-poisoning benchmarks for agent skill packages, not just general packages
- update-channel compromise and version-drift attacks on skills / MCP servers
- config poisoning benchmarks for tool manifests, auth scopes, and default arguments in real deployments
- permission-aware high-privilege action benchmarks with explicit allow / deny policies and rollback semantics
- long-horizon memory poisoning where the trigger is planted many steps before execution
- benchmark-contamination resistant leaderboards with hidden test sets for agent security

## Repo layout

The repo now includes both skill and benchmark catalogs:

```text
skills/
  README.md
  prompt_injection_and_task_hijacking/
  tool_metadata_and_mcp_poisoning/
  dependency_supply_chain_poisoning/
  config_and_parameter_poisoning/
  memory_and_retrieval_poisoning/
  high_privilege_tool_misuse/
  harmful_task_misuse_and_jailbreaks/
  multi_agent_adversarial_manipulation/

benchmarks/
  README.md
  prompt_injection_and_task_hijacking/
  tool_metadata_and_mcp_poisoning/
  dependency_supply_chain_poisoning/
  config_and_parameter_poisoning/
  memory_and_retrieval_poisoning/
  high_privilege_tool_misuse/
  harmful_task_misuse_and_jailbreaks/
  multi_agent_adversarial_manipulation/
  benchmark_coverage_and_meta_audit/

data/
  benchmark_catalog.csv
  benchmark_catalog.json
  category_schema.json
  skill_schema.json
  skills_catalog.csv
  skills_catalog.json
  leaderboard_columns.csv
  leaderboard_schema.json
  leaderboard_template.csv
```

Notes:
- `skills/README.md` is the harmful-skill index.
- Each `skills/<category>/` directory contains redacted skill entries for that family.
- `data/skills_catalog.json` is the canonical machine-readable skill source.
- `data/skills_catalog.csv` is the flat export for spreadsheet workflows.
- `benchmarks/README.md` is the category index.
- Each `benchmarks/<category>/README.md` file lists the mapped benchmarks for that family.
- `data/benchmark_catalog.json` is the canonical machine-readable source.
- `data/benchmark_catalog.csv` is the flat export for spreadsheets or quick filtering.
- `data/leaderboard_schema.json` defines a normalized run-result schema.
- `data/leaderboard_template.csv` gives a starter row for recording evals.

## How to extend it

When adding a new skill:
- add or update the canonical entry in `data/skills_catalog.json`
- mirror the flat row in `data/skills_catalog.csv`
- create or update the redacted markdown entry under `skills/<category>/`
- never add runnable payloads, real exploit strings, or directly reusable malicious prompts

When adding a new benchmark:
- add or update the canonical entry in `data/benchmark_catalog.json`
- mirror the flat row in `data/benchmark_catalog.csv`
- map it into one or more category docs under `benchmarks/`
- if you publish evaluation results, append them using `data/leaderboard_template.csv`

## Leaderboard fields

The leaderboard schema is intentionally generic so it can support agent, MCP, plugin, and adjacent supply-chain evaluations.

Recommended minimum fields:
- `run_id`
- `benchmark_id`
- `category_id`
- `model_name`
- `run_date`
- `metric_primary`
- `score_primary`
- `success_direction`

Optional but useful reproducibility fields:
- `agent_framework`
- `tool_runtime`
- `defense_profile`
- `dataset_version`
- `commit_or_image`
- `source_url`

## Source map

Primary sources used for this initial catalog:
- ToolEmu: https://arxiv.org/abs/2309.15817
- R-Judge: https://arxiv.org/abs/2401.10019
- InjecAgent: https://arxiv.org/abs/2403.02691
- AgentDojo: https://arxiv.org/abs/2406.13352
- Agent-SafetyBench: https://arxiv.org/abs/2412.14470
- ASB: https://arxiv.org/abs/2410.02644
- AgentHarm: https://arxiv.org/abs/2410.09024
- OpenAgentSafety: https://arxiv.org/abs/2507.06134
- WASP: https://arxiv.org/abs/2504.18575
- WAInjectBench: https://arxiv.org/abs/2510.01354
- RAS-Eval: https://arxiv.org/abs/2506.15253
- OS-Harm: https://arxiv.org/abs/2506.14866
- BAD-ACTS: https://arxiv.org/abs/2508.16481
- EU-Agent-Bench: https://arxiv.org/abs/2510.21524
- MCPTox: https://arxiv.org/abs/2508.14925
- MSB: https://arxiv.org/abs/2510.15994
- MCP-SafetyBench: https://arxiv.org/abs/2512.15163
- MalURLBench: https://arxiv.org/abs/2601.18113
- AgentDyn: https://arxiv.org/abs/2602.03117
- GAP: https://arxiv.org/abs/2602.16943
- BackdoorAgent: https://arxiv.org/abs/2601.04566
- SafeAudit: https://arxiv.org/abs/2603.18245
- PoisonBench: https://arxiv.org/abs/2410.08811
- ELBA-Bench: https://arxiv.org/abs/2502.18511
- OSCAR benchmark dataset: https://arxiv.org/abs/2409.09356
- QUT-DV25: https://arxiv.org/abs/2505.13804
- SynthChain: https://arxiv.org/abs/2603.16694

Additional sources used for the seeded skill corpus:
- SafeArena: https://arxiv.org/abs/2503.04957
- VPI-Bench: https://arxiv.org/abs/2506.02456
- RedTeamCUA: https://arxiv.org/abs/2505.21936
- WebTrap Park: https://arxiv.org/abs/2601.08406
- SusBench: https://doi.org/10.1145/3742413.3789111
- Measuring Harmfulness of Computer-Using Agents: https://arxiv.org/abs/2508.00935
- AgentSentinel / BadComputerUse: https://arxiv.org/abs/2509.07764
- Understanding Security Risks of AI Agents' Dependency Updates: https://arxiv.org/abs/2601.00205
- Caller Identity Confusion in MCP-Based AI Systems: https://arxiv.org/abs/2603.07473
- Misleading Tool Descriptions in MCP: https://arxiv.org/abs/2602.03580
- Information Retrieval Induced Safety Degradation in AI Agents: https://arxiv.org/abs/2505.14215
- RedTeamAI: https://doi.org/10.31219/osf.io/36jm5_v1
- BountyBench: https://arxiv.org/abs/2505.15216
- TAMAS: https://arxiv.org/abs/2511.05269
