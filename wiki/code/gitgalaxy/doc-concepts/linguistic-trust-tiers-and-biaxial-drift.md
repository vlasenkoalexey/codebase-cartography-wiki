---
title: Linguistic trust tiers and Biaxial Weaponization — two ways Signal Processor discounts context
type: doc-concept
provenance: doc
source: docs/wiki/02-09-signal-processing.md
updated: 2026-07-04
status: fresh
---
# Linguistic trust tiers and Biaxial Weaponization — two ways Signal Processor discounts context

## Definition
The doc describes two related-but-distinct normalizations the Signal Processor applies before
trusting a raw signal count. The first, "the Tiered Physics Model": because an explicit
language (Rust, Go, Swift, Java) "broadcasts" its safety guarantees while an implicit one
(Shell, SQL, Assembly) hides its risks in ways a regex counter can't see, files are sorted into
three "spectral classes" — Tier 1 Explicit (signals trusted at face value, zero baseline
risk), Tier 2 Structured (Python/JS/C++, a minor "Opacity Tax"), and Tier 3 Implicit (a "Fog of
War" penalty that adds baseline phantom risk regardless of what was actually counted). The
second, "Biaxial Weaponization": the engine measures a file's archetype drift twice — once
against the whole repository's behavior, once against only files in its own language — and
when a file blends in globally but is a local outlier for its language, it triggers a "Trojan
Spike": an exponential multiplier is applied to that file's `logic_bomb` and `obscured_payload`
scores, because a file that looks ordinary next to the whole repo but abnormal next to its own
peers is the specific pattern of something disguising itself as normal.

## In gitgalaxy (grounded)
Both mechanisms are real and match the doc's numbers and framing closely:
- **The trust tiers.** [`SignalProcessor._get_tier`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor._get_tier)
  sorts languages into exactly the three buckets the doc names — `tier1 = {rust, go, swift,
  java, typescript, csharp, dart}`, `tier2 = {python, javascript, cpp, c, ruby, kotlin, php}`,
  everything else falls to `tier3` by default (which is how Shell, SQL, and Assembly land
  there without being listed explicitly). [`SignalProcessor.TIER_VARS`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor.TIER_VARS)
  gives Tier 1 a Fidelity Coefficient (`fc`) of `1.0` and an Implicit Risk Constant (`irc`) of
  `0`, Tier 2 `fc=0.85`/`irc=2`, and Tier 3 `fc=0.60`/`irc=5` — a strictly declining trust
  curve matching the doc's Explicit → Structured → Implicit framing exactly.
- **Biaxial Weaponization is a named block in the actual source.** Reading
  [`calculate_risk_vector`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor.calculate_risk_vector)
  directly: the code carries an inline comment reading literally `# ---> BIAXIAL
  WEAPONIZATION <---` immediately above the calls that pass both `global_drift` and
  `local_drift` into
  [`_calc_obscured_payload`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor._calc_obscured_payload)
  and [`_calc_logic_bomb`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor._calc_logic_bomb) —
  this is the tool's own internal name for the mechanism, not a name the doc invented.
- **The Trojan Spike's exact trigger.** Inside `_calc_logic_bomb`, when both drifts are
  positive, the code computes `drift_delta = local_drift / global_drift` and, if
  `drift_delta > 1.5`, multiplies the sabotage mass by that ratio — a concrete, cited
  threshold (1.5x local-vs-global disagreement) that grounds the doc's "cross-multiplies these
  two drift scores" claim in an exact number.

## Why it matters / when it applies
Both mechanisms are answers to the same underlying problem from two different angles: a raw
regex hit count means something different depending on *what kind* of language it came from
(the tier system) and *what that file looks like relative to its own peers* (the biaxial
drift). Neither requires understanding what the code actually does — both are calibration
layers over the same 60-point signal count, consistent with
[Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md)'s broader framing as
"you don't infer meaning, you count keyword-shaped evidence and calibrate the arithmetic."

## Connections
- Code concepts: [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md) — owns
  `_get_tier`, `TIER_VARS`, `_classify_archetype`, and the Biaxial Weaponization block inside
  `calculate_risk_vector`.
- Module catalogs: [signal_processor](../catalog/gitgalaxy/metrics/signal_processor.md).
- Related doc-concepts: [systemic-bottleneck-taxonomy](systemic-bottleneck-taxonomy.md),
  [identity-deception-and-extension-mismatch](identity-deception-and-extension-mismatch.md).

## Source
Extracted from `docs/wiki/02-09-signal-processing.md` ("Standardization: The Tiered Physics
Model" and "Biaxial Weaponization" sections), kept in place.
