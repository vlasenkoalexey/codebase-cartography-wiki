---
title: The systemic bottleneck taxonomy — network centrality cross-multiplied with risk
type: doc-concept
provenance: doc
source: docs/wiki/02-09-signal-processing.md
updated: 2026-07-04
status: fresh
---
# The systemic bottleneck taxonomy — network centrality cross-multiplied with risk

## Definition
In its final synthesis stage, the doc says the engine identifies "Systemic Bottlenecks" by
cross-multiplying a file's *local* risk exposure against *global* network-graph-theory metrics
supplied by the NetworkRiskSensor, and names three specific combinations: **Contagious
Mutation** (`Betweenness * State Flux` — files that structurally bridge components while also
holding volatile, mutating state, so their side-effects propagate unpredictably to
downstream consumers), **House of Cards** (`Closeness * Error Risk` — files only 1-2 hops from
the whole codebase that also carry high error exposure, so a runtime exception there cascades
instantly), and **Blind Bottleneck** (`Blast Radius * Doc Risk` — "God Nodes" the ecosystem
depends on that lack documentation, making them impossible to modify safely). It also notes an
"Active Logic Mask" that excludes structural assets (JSON, Markdown) from these rankings so
only true executable code competes for the highest-risk slots.

## In gitgalaxy (grounded)
Reading [`SignalProcessor.generate_forensic_report`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor.generate_forensic_report)
directly confirms all three named bottlenecks as real, if under plainer internal names than
the doc's narrative labels:
- The method first applies the "Active Logic Filter" the doc names: it excludes any file whose
  `lang_id` is in `asset_masks`'s `STRUCTURAL_ASSETS` set from `active_files` before any
  ranking runs (falling back to the unfiltered list only if a repo is *entirely* structural
  assets, so the report never comes back empty).
- It then resolves three risk-schema indices — `flux_idx` for `"state_flux"`, `err_idx` for
  `"safety_score"`, `doc_idx` for `"documentation"` — and, per file, reads
  `betweenness_score`, `closeness_score`, and `normalized_blast_radius` out of
  `telemetry.network_metrics` (populated upstream by
  [`NetworkRiskSensor.build_dependency_graph`](../catalog/gitgalaxy/core/network_risk_sensor.md#NetworkRiskSensor.build_dependency_graph),
  read directly from the pinned source and confirmed real; not previously cited in this
  silo's doc-concepts). It buckets results into three real dictionary keys —
  `cascading_state_mutation` (Contagious Mutation), `fragile_dependency_chain` (House of
  Cards), and `undocumented_critical_path` (Blind Bottleneck) — each scored by exactly the
  multiplication the doc names (e.g. `pr * doc_risk` for the Blind Bottleneck score) and
  sorted descending before the top 5 of each are returned.
- "Error Risk" in the doc's House of Cards formula is, concretely, the *inverse* of
  `safety_score` (a low safety score is read as high error exposure) — the doc's plain-English
  label maps onto the existing `safety_score` risk dimension rather than a separately-named
  one.

## Why it matters / when it applies
This is the one place in the pipeline where a purely topological signal (how central is this
file in the import graph, computed by graph-theory algorithms with no awareness of the file's
actual risk content) is deliberately combined with a purely heuristic signal (how risky does
this file's regex-counted content look, with no awareness of its position in the graph) —
neither signal alone would catch "a highly central file that also happens to be dangerous";
the cross-multiplication is what surfaces it. It is also, per
[Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md)'s own "Zero-Dependency
Mode" note, gracefully degraded rather than broken when the optional `networkx` dependency is
absent — network metrics fall back to zeroed defaults rather than crashing the report.

## Connections
- Code concepts: [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md) — owns
  `generate_forensic_report`; [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) —
  Phase 4 (`build_dependency_graph`) and Phase 8 (`generate_forensic_report`) are where the two
  inputs to this cross-multiplication are respectively produced and combined.
- Module catalogs: [signal_processor](../catalog/gitgalaxy/metrics/signal_processor.md),
  [network_risk_sensor](../catalog/gitgalaxy/core/network_risk_sensor.md),
  [galaxyscope](../catalog/gitgalaxy/galaxyscope.md).
- Related doc-concepts: [linguistic-trust-tiers-and-biaxial-drift](linguistic-trust-tiers-and-biaxial-drift.md),
  [risk-exposure-physics](risk-exposure-physics.md) — the generated LLM-facing report where these
  same bottleneck rankings (§7-§12) are actually printed for a human or agent to read.

## Source
Extracted from `docs/wiki/02-09-signal-processing.md` ("The Physics Engine: N-Dimensional
Systemic Bottlenecks" section), kept in place.
