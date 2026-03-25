# Payment and Wallet Transaction Abuse

- `id`: `payment_and_wallet_transaction_abuse`
- `category_id`: `high_privilege_tool_misuse`
- `execution_phase`: `financial execution and transfers`
- `target_surface`: crypto wallets, exchanges, Stripe, brokerage and payment APIs
- `attacker_position`: malicious user prompt or hijacked downstream workflow
- `artifact`: payment requests, wallet transfers, trade orders, invoices
- `privileges_sought`: unauthorized transfer, trading, or purchase activity
- `evidence_basis`: public_catalog_inference
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Finance-facing skills expose direct economic side effects, so even a small planning failure can become a real transfer, trade, or payment mutation.

## Representative behaviors

- wallet transfer initiation
- exchange order placement
- billing or subscription mutation

## Related benchmarks

- `eu_agent_bench`
- `gap`

## References

- https://clawhub-skills.com/
- https://github.com/sundial-org/awesome-openclaw-skills

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
