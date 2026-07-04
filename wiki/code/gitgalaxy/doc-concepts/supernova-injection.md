---
title: Supernova injection — forcing dangerous artifacts back onto the map
type: doc-concept
provenance: doc
source: docs/wiki/02-01-pipeline-overview.md, docs/wiki/02-02-optical-orchestration.md, docs/wiki/02-03-aperture-filter.md
updated: 2026-07-04
status: fresh
---
# Supernova injection — forcing dangerous artifacts back onto the map

## Definition
Across all three docs, GitGalaxy's authors describe a consistent exception to "filtered means
invisible": a small set of dangerous artifact classes — leaked credentials, weaponized binaries, and
large AI model weight files — are deliberately **forced back onto the 3D visualization** as a
"Supernova" even though they would otherwise be excluded or shunted to "Dark Matter" by the normal
scope/threat pipeline. `02-02-optical-orchestration.md`'s own framing: "the Orchestrator checks the
'Dark Matter' pile. If the `NeuralAuditor` or `SecurityLens` flagged a filtered file ... the chassis
artificially injects a 'Supernova' onto the map — forcing the massive localized threat to render in
the UI despite being structurally inert." `02-03-aperture-filter.md`'s Data Classification Matrix
names the same idea from the filter's side: "Quarantine (Radioactive)" and "X-Ray Anomalies" are the
two rows marked "Forced onto 3D map as a Supernova," in contrast to every other excluded row, which is
simply "Not Rendered" or sent to the "Dark Matter Singularity."

## In gitgalaxy (grounded)
This is not just visualization framing — it maps onto a real, deliberate control-flow inversion
already documented on the [Aperture Filter](../concepts/gitgalaxy-core-aperture.md) page: a file whose
[`evaluate_path_integrity`](../catalog/gitgalaxy/core/aperture.md#ApertureFilter.evaluate_path_integrity)
result names a `"CRITICAL LEAK"` is technically `is_valid=False` (blocked from normal structural
parsing), yet [`is_in_scope`](../catalog/gitgalaxy/core/aperture.md#ApertureFilter.is_in_scope)
explicitly re-checks that exact reason string and forces `is_in_scope=True` — "invisible unless
dangerous," in that page's own words. That is the "Secrets Supernova" the docs describe, grounded to
the exact method that performs the override.

The docs name two other classes of Supernova the Aperture Filter's own subgraph does not implement
itself:
- **"X-Ray Anomalies"** (weaponized/malware binaries and AI model weights caught by header/entropy
  inspection) are produced by [`run_xray_audit`](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md#run_xray_audit)
  in `binary_anomaly_detector.py` — see [X-Ray binary inspection](xray-binary-inspection.md) for how
  this maps onto the doc's "X-Ray Binary Sensor" framing inside the Aperture Filter doc itself.
- **The "Neural Supernova"** (AI model-weight metadata extraction) is
  [`TensorScanner`](../catalog/gitgalaxy/metrics/tensor_scanner.md#TensorScanner), invoked from
  [`_calculate_risk_exposures`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator._calculate_risk_exposures) —
  not a `neural_auditor.py` module, despite that being the name used in the pipeline-overview doc's
  table (see [The optical pipeline metaphor](optical-pipeline-metaphor.md) for the full doc-vs-code
  naming table).

The actual "force it back onto the map" mechanism at the `Orchestrator` level — the code that reads
the Dark Matter/rejection pile and re-injects a flagged entry — is not itself a separately named
symbol inside this packet's subgraph; the only concretely grounded half of "Supernova injection" is
the Aperture Filter's own `is_in_scope` override for secrets. The rendering-side injection the docs
describe for X-Ray/Neural anomalies is consistent with, but not directly cited to, a symbol in
`galaxyscope.py` beyond the general Phase 10 ecosystem-audit calls already documented on the
[GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) page.

## Why it matters / when it applies
This is the clearest first-party statement of gitgalaxy's actual security philosophy: **noise
reduction and threat surfacing are different axes**, not one continuum from "safe to ignore" to
"unsafe to ignore." A file can be excluded from the *structural* graph (no function/class extraction,
no risk-vector contribution) while still being forced into the *visual/threat* output, because the
tool's purpose is auditing an entire repository's risk posture, not just producing a clean symbol
graph. This is a meaningfully different posture from the survey's SCIP-grounded tools, which have no
comparable "exclude from the index but surface as a critical finding anyway" path — a symbol either
resolves or it doesn't.

## Connections
- Code concepts: [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md) — implements the
  Secrets Supernova override directly; [SecurityLens](../concepts/gitgalaxy-security-security_lens.md) —
  the other flagger the docs name; [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) —
  Phase 10's ecosystem security audits, one source of X-Ray/Neural findings.
- Module catalogs: [aperture](../catalog/gitgalaxy/core/aperture.md), [binary_anomaly_detector](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md),
  [tensor_scanner](../catalog/gitgalaxy/metrics/tensor_scanner.md).
- Related doc-concepts: [optical-pipeline-metaphor](optical-pipeline-metaphor.md), [xray-binary-inspection](xray-binary-inspection.md).

## Source
Extracted from `docs/wiki/02-01-pipeline-overview.md`, `docs/wiki/02-02-optical-orchestration.md`, and
`docs/wiki/02-03-aperture-filter.md`, kept in place.
