# Config and Parameter Poisoning

Poisoning system prompts, tool schemas, argument defaults, preference-learning data, PEFT adapters, or hidden backdoor triggers that alter downstream behavior.

## Skill entries

| Skill | Phase | Surface | Evidence |
| --- | --- | --- | --- |
| [System Prompt and Policy Override](system_prompt_policy_override.md) | configuration and planning | system prompts, policy files, agent config | direct |
| [Argument and Schema Poisoning](argument_schema_poisoning.md) | tool argument construction | function schemas, default args, parameter hints | direct |
| [Adapter or Parameter Backdoor Trigger](adapter_backdoor_trigger.md) | model loading and inference | fine-tuned weights, adapters, poisoned training preferences | adjacent |

## Safety note

- These entries are intentionally redacted and defensive in purpose.
- Do not add runnable exploit payloads, live malicious prompts, or weaponizable scripts.
- If a public paper includes dangerous details, summarize the pattern instead of copying it.
