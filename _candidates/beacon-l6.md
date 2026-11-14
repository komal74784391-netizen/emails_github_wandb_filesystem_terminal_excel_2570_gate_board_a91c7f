---
candidate_id: beacon-l6
model_family: beacon
eval_split: holdout-2026q4
status: active
gate_score: 0.588
gate_decision: retest
reviewed_on: 2026-10-02
reviewer: s.park
---
# Beacon L6

## Scope
Late-interaction retriever used by the knowledge-base search API.

## Serving notes
- Primary deployment: kb-search-a
- Replica: kb-search-b (same revision)
- Index refresh cadence: every 6 hours

## Review history
The previous revision regressed on multi-hop questions. A hard-negative
mining pass was added for this cycle.
