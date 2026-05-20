# Failure Matrix: Buyer Memory Ledger

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| ai-native evidence replay | ai-native_drift | ai-native_coverage | block release until cited evidence is regenerated | ev_0000 |
| buyer operator packet | buyer_blindspot | buyer_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| buyer operator packet | buyer_blindspot | buyer_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| remembering regression harness | remembering_misroute | remembering_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| depends boundary probe | depends_gap | depends_risk | route to reviewer with evidence packet | ev_0021 |
| remembering regression harness | remembering_misroute | remembering_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| ai-native evidence replay | ai-native_drift | ai-native_coverage | block release until cited evidence is regenerated | ev_0028 |
