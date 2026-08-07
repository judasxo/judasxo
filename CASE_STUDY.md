# Fail-Closed Trading System

**Auditable quantitative research and paper-operations controls**

> Can a system reject weak evidence, preserve failure, and execute safely without silently loosening its controls?

## At a glance

| Evidence | Result |
|---|---:|
| Pre-registered hypotheses rejected | 2 |
| Data defects sufficient to block admission | 3 |
| Unchanged reliability thresholds passed | 9/9 |
| Offline public regression tests | 15 |

## Research: the primary question stayed primary

- The turn-of-month claim failed at **-2.62 bp per cycle**, with a one-sided lower bound of **-23.90 bp**.
- A positive secondary strategy-versus-cash result (**+23.44 bp**, lower bound **+3.93 bp**) was not promoted into a win because it did not answer the pre-registered anomaly question.
- An attractive quarter-end subgroup was declined and shown underpowered on its own terms: **+3.83 bp** observed versus a **75.30 bp** illustrative MDE.

## Data: aggregate cleanliness did not override frozen gates

A price source matched the comparison source to the cent on **99.94%** of sessions. It was still rejected because two rows had impossible OHLC geometry and one close differed by **$0.20**, violating thresholds frozen before inspection.

That decision blocked progress. The cost is what makes it meaningful evidence of discipline.

## Operations: failed states stayed visible

- Bounded equity and crypto paper canaries completed and reconciled cleanly.
- Reliability V1 failed after the host slept, producing a **10,836-second** heartbeat gap.
- V2 changed instrumentation, not acceptance criteria, and passed all nine unchanged thresholds over a genuine 24-hour run.
- The measured crypto round-trip cost floor was **59.75 bp median** and **63.63 bp p95**, before slippage.

## Fail-closed control path

`freeze claim + threshold` -> `validate data + state` -> `record intent` -> `perform bounded mutation` -> `reconcile with direct evidence`

## What the public repository proves

The credential-free, network-free demo replays five operational situations. One deliberately sabotages intent-before-entry and proves the regression suite catches the bypass. A bidirectional SHA-256 manifest rejects both missing and unlisted files.

**No profitable-edge or live-readiness claim is made.** The evidence is the judgment: weak hypotheses stayed dead, unsafe states halted, and failed runs remained visible.

[Repository](https://github.com/judasxo/fail-closed-trading-system) | [Run the demo](https://github.com/judasxo/fail-closed-trading-system#try-the-synthetic-demo) | [Release v1.0.0](https://github.com/judasxo/fail-closed-trading-system/releases/tag/v1.0.0)
