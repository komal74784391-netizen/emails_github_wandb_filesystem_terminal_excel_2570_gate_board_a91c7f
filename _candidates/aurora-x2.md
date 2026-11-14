---
candidate_id: aurora-x2
model_family: aurora
eval_split: holdout-2026q4
status: active
gate_score: 0.612
gate_decision: retest
reviewed_on: 2026-10-30
reviewer: l.mensah
---
# Aurora X2

## Scope
Cross-encoder reranker for the product search surface.

## Serving notes
- Primary deployment: search-rerank-canary
- Fallback: legacy-biencoder-v4
- Latency budget: 45 ms p95

## Review history
Previous cycle showed uneven gains on long-tail queries; the team
tightened the negative sampling mix before this evaluation.
