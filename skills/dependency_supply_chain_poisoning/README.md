# Dependency and Supply Chain Poisoning

Malicious packages, dependency confusion, poisoned updates, build-time compromise, or install-time payloads affecting skills, plugins, or agent runtimes.

## Skill entries

| Skill | Phase | Surface | Evidence |
| --- | --- | --- | --- |
| [Dependency Confusion Skill Package](dependency_confusion_skill_package.md) | installation and dependency resolution | package registries and dependency manifests | adjacent |
| [Risky Dependency Update Skill](risky_dependency_update_agent.md) | maintenance and automated updates | dependency upgrade pull requests and version selection | direct |

## Safety note

- These entries are intentionally redacted and defensive in purpose.
- Do not add runnable exploit payloads, live malicious prompts, or weaponizable scripts.
- If a public paper includes dangerous details, summarize the pattern instead of copying it.
