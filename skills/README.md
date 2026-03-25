# Harmful Skill Corpus

This directory stores redacted harmful-skill entries for defensive research. Each entry captures the attack pattern, target surface, and source references without including runnable payloads.

| Category | Summary | Skill entries |
| --- | --- | --- |
| [Prompt Injection and Task Hijacking](prompt_injection_and_task_hijacking/README.md) | Malicious instructions embedded in web pages, tool outputs, emails, URLs, or third-party content redirect the agent away from the user objective. | 4 |
| [Tool Metadata and MCP Poisoning](tool_metadata_and_mcp_poisoning/README.md) | Attacks that poison tool descriptions, MCP metadata, manifests, names, or response channels before or during tool selection and invocation. | 2 |
| [Dependency and Supply Chain Poisoning](dependency_supply_chain_poisoning/README.md) | Malicious packages, dependency confusion, poisoned updates, build-time compromise, or install-time payloads affecting skills, plugins, or agent runtimes. | 3 |
| [Config and Parameter Poisoning](config_and_parameter_poisoning/README.md) | Poisoning system prompts, tool schemas, argument defaults, preference-learning data, PEFT adapters, or hidden backdoor triggers that alter downstream behavior. | 4 |
| [Memory and Retrieval Poisoning](memory_and_retrieval_poisoning/README.md) | Poisoned memories, RAG stores, prior plans, or retrieved artifacts persist across turns and influence future tool use. | 2 |
| [High-Privilege Tool Misuse](high_privilege_tool_misuse/README.md) | Unauthorized or unsafe actions via tools with real-world side effects, especially in OS, browser, finance, healthcare, legal, or infra contexts. | 12 |
| [Harmful Task Misuse and Jailbreaks](harmful_task_misuse_and_jailbreaks/README.md) | Benchmarks where the user or environment attempts to coerce the agent into harmful multi-step behavior while preserving capability. | 3 |
| [Multi-Agent Adversarial Manipulation](multi_agent_adversarial_manipulation/README.md) | One compromised agent or message channel manipulates peer agents to perform unsafe actions. | 1 |
| [Benchmark Coverage and Meta-Audit](benchmark_coverage_and_meta_audit/README.md) | Benchmarks or audit frameworks that test the completeness and blind spots of existing agent-safety suites. | 3 |
