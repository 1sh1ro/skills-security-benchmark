# Retrieval Corpus Contamination

- `id`: `retrieval_corpus_contamination`
- `category_id`: `memory_and_retrieval_poisoning`
- `execution_phase`: `retrieval and grounding`
- `target_surface`: RAG corpora, search results, retrieved files
- `attacker_position`: content publisher or indexing adversary
- `artifact`: retrieved snippet, indexed document, search result
- `privileges_sought`: unsafe guidance via trusted retrieval
- `evidence_basis`: direct
- `payload_included`: `false`
- `live_code_included`: `false`

## Redacted summary

Retrieved content is treated as trustworthy context and quietly degrades safety by biasing plans, actions, or approvals.

## Representative behaviors

- unsafe retrieval grounding
- context poisoning
- trusted-source abuse

## References

- https://arxiv.org/abs/2505.14215
- https://arxiv.org/abs/2506.15253

## Handling rule

- Preserve only metadata, taxonomy, and defensive analysis.
- Do not store runnable prompts, exploit strings, or live malicious code here.
