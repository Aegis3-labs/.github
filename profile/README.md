# Aegis3

Token-launch integrity analysis that produces **deterministic, auditable evidence** instead of opaque model scores.

## How it works
- **Sybil clustering:** hub-pruned Louvain community detection over wallet graphs
- **Behavioural similarity:** Jaccard similarity on contract-call patterns
- **Cash-out tracing:** detects wallets converging on the same CEX deposit address
- **Temporal signals:** decay and burst weighting to flag synchronized funding loops
- **Risk score:** multi-signal scorer, 0-100, with tiered verdicts
- **Tamper evidence:** a SHA-256 manifest seals inputs and reports so changes are detectable

## Principle
Every verdict traces back to inputs and rules a reviewer can re-run. If a result can't be reproduced, it doesn't count.

## Repositories
- [Aegis3](https://github.com/Aegis3-labs/Aegis3): core detection engine and evidence pipeline
