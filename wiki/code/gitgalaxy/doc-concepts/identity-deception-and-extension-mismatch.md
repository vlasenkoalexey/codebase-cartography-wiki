---
title: Identity deception — the Identity Crisis Trap and the Extension Deception Sensor
type: doc-concept
provenance: doc
source: docs/wiki/02-05-language-lens.md
updated: 2026-07-04
status: fresh
---
# Identity deception — the Identity Crisis Trap and the Extension Deception Sensor

## Definition
Two docs describe two independent, layered defenses against a file lying about what it is.
The Language Lens doc's "Identity Crisis Trap" (Security Integration): if a file claims to be
Python (`.py`) but opens with a Bash shebang, the Lens does not average or prefer one signal —
it flags an "Identity Masking" anomaly, caches it for the Security module, and forces the file
into Tier 5 Absolute Distrust (`undeterminable`). The same doc's "Code Shield" defends the
opposite direction: a hostile file named `README.cpp` must not be treated as prose just
because its stem looks like documentation — a known executable extension strictly bypasses
prose-anchor checks. The Signal Processing doc adds a second, downstream layer: the
"Extension Deception Sensor," which punishes a file claiming an inert data extension (`.txt`,
`.json`) but evaluated as executable code, flagging a `sec_extension_mismatch` violation.

## In gitgalaxy (grounded)
All three mechanisms are real, and two of them live in the same method:
- **Identity Crisis Trap.** Inside [`LanguageDetector.inspect`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.inspect),
  reading the pinned source directly: when an extension-based language guess and a
  shebang-based guess disagree, the code logs `"IDENTITY CONFLICT: Ext '...' contradicts
  Shebang '...'"` and appends a message to the result's
  [`anomaly_flags`](../catalog/gitgalaxy/standards/language_lens.md#DetectorResult) list
  (a field on `DetectorResult`, "Security RAM Cache for conflicting identity indicators," per
  its own inline comment) rather than picking a side.
- **The Code Shield.** The same `inspect` method carries an inline comment reading
  "DEFENSIVE GUARD: The Executable Shield ... Do not allow textual anchor hijacking (e.g., a
  file named README.sh) if it has an executable extension" — a known code extension
  (anything in [`extension_map`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.extension_map)
  besides `.txt`/`.md`/`.log`) short-circuits the prose-anchor check before it ever runs.
- **Extension Deception Sensor.** Reading the pinned source directly, this check is
  implemented *twice*, independently: once inside
  [`calculate_risk_vector`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor.calculate_risk_vector)
  itself (a file with an "inert disguise" extension whose detected `lang_id` is one of a
  hardcoded set of executable languages sets `raw_signals["sec_extension_mismatch"] = 1`,
  logging "🚨 SPOOFING DETECTED"), and again inside `gitgalaxy/security/security_lens.py`'s own
  threat-flagging logic (outside this doc-concept's assigned packet, so not linked further
  here) — the same suspicion is checked by two separate modules rather than computed once and
  shared.

## Why it matters / when it applies
This is a three-layer defense-in-depth against the same underlying threat model — a file
whose stated identity and actual content disagree — implemented at three different points in
the pipeline (language classification, prose-vs-code routing, and risk scoring) rather than
one central "verify identity" gate. The doc frames this as protecting against "AI-generated
code and automated refactoring" where "single-point metadata is no longer a source of absolute
truth"; grounding it in source shows the protection is not a single check but a layered set of
independent tripwires, any one of which can catch a mismatch the others miss.

## Connections
- Code concepts: [Language lens](../concepts/gitgalaxy-standards-language_lens.md) — owns the
  Identity Crisis Trap and Code Shield; [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md) —
  owns the Extension Deception Sensor's risk-scoring side; [SecurityLens](../concepts/gitgalaxy-security-security_lens.md) —
  the security-module consumer the Lens's `anomaly_flags` are cached for, and the second,
  independent place the deception check is re-implemented.
- Module catalogs: [language_lens](../catalog/gitgalaxy/standards/language_lens.md),
  [signal_processor](../catalog/gitgalaxy/metrics/signal_processor.md).
- Related doc-concepts: [language-lens-bayesian-trust-tiers](language-lens-bayesian-trust-tiers.md).

## Source
Extracted from `docs/wiki/02-05-language-lens.md` ("The Identity Crisis Trap" section) and
`docs/wiki/02-09-signal-processing.md` ("The Infrastructure Shields" section), both kept in
place.
