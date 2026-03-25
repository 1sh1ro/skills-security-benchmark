# Prompt Injection and Task Hijacking

Malicious instructions embedded in web pages, tool outputs, emails, URLs, or third-party content redirect the agent away from the user objective.

## Skill entries

| Skill | Phase | Surface | Evidence |
| --- | --- | --- | --- |
| [Indirect Prompt Injection via Web Content](indirect_prompt_injection_web_content.md) | context ingestion | web pages, documents, emails, rendered content | direct |
| [Malicious URL and Redirect Processing](malicious_url_redirect_skill.md) | navigation and browsing | URLs, redirects, landing pages, preview content | direct |
| [Visual Prompt Injection Overlay](visual_prompt_injection_overlay.md) | screen perception and grounding | screenshots, UI overlays, rendered images | direct |
| [Dark-Pattern Workflow Manipulation](dark_pattern_workflow_manipulation.md) | interactive workflow execution | web forms, consent dialogs, deceptive page layouts | direct |

## Safety note

- These entries are intentionally redacted and defensive in purpose.
- Do not add runnable exploit payloads, live malicious prompts, or weaponizable scripts.
- If a public paper includes dangerous details, summarize the pattern instead of copying it.
