# Tool Metadata and MCP Poisoning

Attacks that poison tool descriptions, MCP metadata, manifests, names, or response channels before or during tool selection and invocation.

## Skill entries

| Skill | Phase | Surface | Evidence |
| --- | --- | --- | --- |
| [MCP Tool Description Poisoning](mcp_tool_description_poisoning.md) | tool discovery and selection | tool descriptions, manifests, metadata fields | direct |
| [MCP Caller Identity Confusion](mcp_caller_identity_confusion.md) | authorization and routing | identity fields, caller metadata, cross-server context | direct |

## Safety note

- These entries are intentionally redacted and defensive in purpose.
- Do not add runnable exploit payloads, live malicious prompts, or weaponizable scripts.
- If a public paper includes dangerous details, summarize the pattern instead of copying it.
