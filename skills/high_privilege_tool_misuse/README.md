# High-Privilege Tool Misuse

Unauthorized or unsafe actions via tools with real-world side effects, especially in OS, browser, finance, healthcare, legal, or infra contexts.

## Skill entries

| Skill | Phase | Surface | Evidence |
| --- | --- | --- | --- |
| [Browser Session Account Takeover](browser_session_account_takeover.md) | browser automation and session reuse | logged-in browser sessions, forms, anti-bot bypass browsers | public_catalog_inference |
| [Camera and Sensor Surveillance Abuse](camera_and_sensor_surveillance_abuse.md) | device and sensor access | RTSP or ONVIF cameras, local peripherals, captured media | public_catalog_inference |
| [Cloud Deploy and DNS Mutation](cloud_deploy_and_dns_mutation.md) | deployment and infrastructure administration | Cloudflare, Vercel, DNS, edge workers, cloud CLIs | public_catalog_inference |
| [Communication Impersonation and History Mining](communication_impersonation_and_history_mining.md) | messaging and communications access | Slack, Discord, WhatsApp, email, chat history, outbound messaging | public_catalog_inference |
| [Computer-Use Data Exfiltration Chain](computer_use_data_exfiltration_chain.md) | cross-app execution | browser, clipboard, filesystem, messaging, cloud drives | direct |
| [Credential Vault Secret Exfiltration](credential_vault_secret_exfiltration.md) | secret retrieval and command execution | password managers, secret vaults, injected env vars | public_catalog_inference |
| [Interactive Terminal Session Hijack](interactive_terminal_session_hijack.md) | interactive CLI control | tmux sessions, long-running terminals, background agent panes | public_catalog_inference |
| [Overprivileged OS Action Chain](overprivileged_os_action_chain.md) | tool execution | desktop, filesystem, browser, shell, admin actions | direct |
| [Payment and Wallet Transaction Abuse](payment_and_wallet_transaction_abuse.md) | financial execution and transfers | crypto wallets, exchanges, Stripe, brokerage and payment APIs | public_catalog_inference |
| [Regulated-Domain Action Abuse](regulated_domain_action_abuse.md) | decision and execution | finance, healthcare, legal, government, enterprise tools | direct |
| [Source Control and CI Mutation](source_control_and_ci_mutation.md) | repo administration and workflow automation | GitHub repositories, pull requests, Actions workflows, CI logs | public_catalog_inference |
| [Workspace Document Bulk Export](workspace_document_bulk_export.md) | workspace and knowledge-base access | Google Workspace, Notion, Apple Notes, document stores, email-linked files | public_catalog_inference |

## Safety note

- These entries are intentionally redacted and defensive in purpose.
- Do not add runnable exploit payloads, live malicious prompts, or weaponizable scripts.
- If a public paper includes dangerous details, summarize the pattern instead of copying it.
