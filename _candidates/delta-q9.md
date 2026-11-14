---
candidate_id: delta-q9
model_family: delta
eval_split: holdout-2026q4
status: active
gate_score: 0.6182
gate_decision: retest
reviewed_on: 2026-11-13
reviewer: d.okonkwo
---
# Delta Q9

## Scope
Distilled reader-ranker pair for the support-document assistant.

## Serving notes
- Primary deployment: support-assistant-ranker
- Distillation teacher: aurora-x2 (cycle 12)
- Monitoring: ndcg@10 plus answer-anchor hit rate

## Review history
The distilled student is still catching up with its teacher on the
holdout split; this cycle adds a harder query set from support tickets.
