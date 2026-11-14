---
candidate_id: cinder-r4
model_family: cinder
eval_split: holdout-2026q4
status: active
gate_score: 0.5
gate_decision: reject
reviewed_on: 2026-11-13
reviewer: d.okonkwo
---
# Cinder R4

## Scope
Sparse-dense hybrid retriever for the archive search workload.

## Serving notes
- Primary deployment: archive-search
- Query fan-out: 3 shards per request
- Warm cache: 20 minutes

## Review history
Recall on the archive workload has been drifting downward for three
cycles. The team is evaluating a vocabulary rebuild.
