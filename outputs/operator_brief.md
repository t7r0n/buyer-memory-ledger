# Operator Brief: DealFlowAgent

DealFlowAgent gets a local, deterministic pressure test around ai-native, depends, and remembering. The useful part is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- ai-native evidence replay -> block release until cited evidence is regenerated (ai-native_coverage, evidence ev_0044).
- buyer operator packet -> accept only if decision claims cite fixture evidence (depends_risk, evidence ev_0099).
- remembering regression harness -> open a regression issue with trace and benchmark delta (remembering_precision, evidence ev_0110).
- depends boundary probe -> route to reviewer with evidence packet (buyer_latency, evidence ev_0121).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
