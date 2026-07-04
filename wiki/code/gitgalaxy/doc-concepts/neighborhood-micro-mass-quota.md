---
title: The Neighborhood Micro-Mass Quota — a census-time scope filter that lives outside ApertureFilter
type: doc-concept
provenance: doc
source: docs/wiki/02-03-aperture-filter.md, docs/wiki/02-02-optical-orchestration.md
updated: 2026-07-04
status: fresh
---
# The Neighborhood Micro-Mass Quota — a census-time scope filter that lives outside ApertureFilter

## Definition
`02-03-aperture-filter.md` describes a per-directory density check as part of the "Solar Shield":
"To prevent 'space dust' from cluttering the visual map, the filter tracks the density of micro-files
(< 50 bytes) within individual folders. If a neighborhood exceeds its grace limit of micro-debris,
subsequent tiny files are evaporated. (Legacy mainframe files like COBOL copybooks are explicitly
exempted from this quota.)" The doc's own prose files this under "the filter" — i.e. groups it with
the [Aperture Filter](../concepts/gitgalaxy-core-aperture.md)'s other exclusion tiers.

## In gitgalaxy (grounded)
This is real and precisely as described, but it is **not** implemented inside `ApertureFilter` — it
lives in the `Orchestrator` class in `galaxyscope.py`, one layer up. Three instance attributes set in
`Orchestrator.__init__` carry the state: `MICRO_MASS_BYTES` (50, matching the doc's "< 50 bytes"),
`MICRO_MASS_GRACE_LIMIT` (15), and a `defaultdict(int)` named `neighborhood_tracker`, keyed by
directory path. The check itself is duplicated in both census paths —
[`_build_file_census`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator._build_file_census) (the
primary `git ls-files`-driven walk) and [`_fallback_filesystem_walk`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator._fallback_filesystem_walk)
(the non-git fallback) — each incrementing `neighborhood_tracker[dir_path]` for every file under
`MICRO_MASS_BYTES` and rejecting the file with the reason `"Excluded: Neighborhood Micro-Mass Limit
Exceeded"` once that directory's count passes `MICRO_MASS_GRACE_LIMIT`, unless the file's extension is
in the COBOL-family exempt set (`.cpy`, `.cbl`, `.cob`, `.jcl`) — matching the doc's parenthetical
exemption exactly.

Because both census methods, not `ApertureFilter.evaluate_path_integrity`/`is_in_scope`, own this
check, it is order-dependent in the same *shape* the [Aperture Filter](../concepts/gitgalaxy-core-aperture.md)
page already documents for `dynamic_ignore_dirs` — a directory's micro-files are only rejected once
enough of them have already been *seen* in this same census pass, so the first `MICRO_MASS_GRACE_LIMIT`
tiny files in a directory always survive regardless of how many more follow. It is a third, independent
scope-narrowing mechanism sitting alongside `ApertureFilter`'s own gates, evaluated at
census time rather than inside the filter class the doc's own prose implies it belongs to.

## Why it matters / when it applies
The doc's framing ("the filter tracks...") reads as if this is one more tier of `ApertureFilter`'s
`_check_artifact_integrity`/`_check_ignore_rules` cascade, but the pinned source draws the boundary
differently: `ApertureFilter` decides per-file scope from a file's own bytes and path, while this quota
is a *cross-file, stateful* accumulator that only the `Orchestrator` doing the census can maintain
(it needs to have already seen every prior file in the same directory). That distinction matters for
anyone trying to reuse `ApertureFilter` standalone — as the [Aperture Filter](../concepts/gitgalaxy-core-aperture.md)
page notes, `vault_sentinel.py` and `binary_anomaly_detector.py` already do call `ApertureFilter`
directly outside the main pipeline — because the Micro-Mass Quota will simply not apply to those
callers; it is wired only into the two `Orchestrator` census paths.

## Connections
- Code concepts: [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md) — the class the doc
  attributes this quota to, and whose `dynamic_ignore_dirs` shares the same order-dependent,
  census-scoped statefulness; [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) — the
  class that actually owns `MICRO_MASS_BYTES`/`MICRO_MASS_GRACE_LIMIT`/`neighborhood_tracker` and both
  census methods.
- Module catalogs: [galaxyscope](../catalog/gitgalaxy/galaxyscope.md).
- Related doc-concepts: [optical-pipeline-metaphor](optical-pipeline-metaphor.md), [domain-dialect-patching](domain-dialect-patching.md).

## Source
Extracted from `docs/wiki/02-03-aperture-filter.md` and `docs/wiki/02-02-optical-orchestration.md`,
kept in place.
