---
title: The Cartographer — deterministic 3D galaxy positioning via ray-casting and hash jitter
type: doc-concept
provenance: doc
source: docs/wiki/02-08-the-detector.md
updated: 2026-07-04
status: fresh
---
# The Cartographer — deterministic 3D galaxy positioning via ray-casting and hash jitter

## Definition
The doc describes "the Cartographer" as the stage that turns a flat file list into a
deterministic 3D star map for GitGalaxy's WebGPU visualization, using a collision-aware
packing algorithm rather than a naive spiral. It breaks the layout into three problems: **Hull
Calculation** — group files by directory ("Constellation"), designate the highest-mass file
the "Sun," and size the constellation's bounding radius from the Sun's footprint plus
`sqrt(star_count) * spacing`; **the Ray-Casting Dynamic Mask** — to avoid an O(N²) collision
check across thousands of folders, bucket the 360-degree map into one-degree angular bins, and
when placing a new constellation, cast a ray down its angle and solve a quadratic
ray-circle intersection only against the handful of previously-placed circles that ray could
plausibly hit, pushing outward only as far as the nearest positive intersection root; and
**Organic Entropy** — jitter every node's position by an amount derived from an MD5 hash of
its filename, so the placement looks organic rather than mechanically perfect, while remaining
exactly reproducible run over run because the seed is the filename itself.

## In gitgalaxy (grounded)
The Cartographer is implemented as [`SpatialMapper`](../catalog/gitgalaxy/core/spatial_mapper.md#SpatialMapper)
in `gitgalaxy/core/spatial_mapper.py` — a module name and class the doc's own "Cartographer"
narrative never states directly, and which, at the time of this doc-concept, has no dedicated
code-concept page of its own in this silo (it is currently referenced only in passing, as
Phase 7 of [GalaxyScope](../concepts/gitgalaxy-galaxyscope.md)'s orchestration). Reading the
pinned source directly confirms the doc's numbers and mechanism precisely:
- **The hull formula matches exactly.** [`SpatialMapper.map_repository`](../catalog/gitgalaxy/core/spatial_mapper.md#SpatialMapper.map_repository)
  computes `hull_radius = central_footprint + (math.sqrt(len(items)) * self.MICRO_SPACING)`,
  where [`MICRO_SPACING`](../catalog/gitgalaxy/core/spatial_mapper.md#SpatialMapper.MICRO_SPACING)
  is a real instance constant set to `250.0` in `__init__` — the doc's stated baseline spacing
  value, letter for letter.
- **The ray-casting collision avoidance is a real angular hash, not a metaphor.** The same
  method buckets a `360`-entry `spatial_grid` array, and for each new constellation only
  queries the 3 bins (`ray_deg - 1`, `ray_deg`, `ray_deg + 1`) its casting ray could intersect,
  then solves the quadratic `disc = b**2 - 4*c` intersection the doc describes, pushing the
  placement to `max_r_intersect + sec_radius`. The doc's `CORE_EXCLUSION_RADIUS` of `600.0`
  and `MACRO_STEP_FACTOR` of `1.5` are both real instance constants (`self.CORE_EXCLUSION_RADIUS`,
  `self.MACRO_STEP_FACTOR`) read verbatim from the same `__init__`.
- **The Golden Angle and jitter are exact.** [`MICRO_GOLDEN_ANGLE`](../catalog/gitgalaxy/core/spatial_mapper.md#SpatialMapper.MICRO_GOLDEN_ANGLE)
  is computed as `math.pi * (3.0 - math.sqrt(5.0))` (≈2.39996 rad, ≈137.5°), matching the
  doc's Fibonacci angle claim precisely rather than being a hardcoded approximation.
  [`SpatialMapper._hash_jitter`](../catalog/gitgalaxy/core/spatial_mapper.md#SpatialMapper._hash_jitter)
  hashes a seed string via MD5, takes its first 8 hex characters as an integer, and normalizes
  it to `[-1.0, 1.0]` before scaling by an amplitude — the doc's "MD5 Seed Logic" exactly. The
  Z-axis jitter is deliberately `4x` the X/Y jitter magnitude (`JITTER_MAGNITUDE * 4`,
  confirmed in `map_repository`), matching the doc's claim that "the Z-axis receives a 4x
  multiplier to aggressively deepen the volumetric layering."

## Why it matters / when it applies
This subsystem has nothing to do with structural analysis or risk scoring — it exists purely
so a human exploring the visualization at gitgalaxy.io can build a stable mental map of a
repository's shape: the same file always renders at the same jittered coordinate, so a
developer's spatial memory of "the risky files cluster over there" stays valid across repeated
audits of the same codebase. It is also a clean example of a genuinely orthogonal concern (3D
UI layout) getting the same deterministic-by-construction design discipline (hash-seeded, not
random-seeded) that this survey's other doc-concepts find applied to the analysis engine
itself — determinism as a house style, not just an analysis-correctness requirement.

## Connections
- Code concepts: [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) — Phase 7 of
  `execute_pipeline` calls `SpatialMapper.map_repository`; no dedicated Detector/Prism/Signal
  Processor concept page covers `SpatialMapper` directly, so this doc-concept is this silo's
  most detailed grounding of it to date.
- Module catalogs: [spatial_mapper](../catalog/gitgalaxy/core/spatial_mapper.md),
  [galaxyscope](../catalog/gitgalaxy/galaxyscope.md).
- Related doc-concepts: [satellite-physics-and-naming-shields](satellite-physics-and-naming-shields.md) —
  the per-function `Magnitude` this module's `_get_magnitude` reads to pick each Sun and size
  each footprint.

## Source
Extracted from `docs/wiki/02-08-the-detector.md` ("The Cartographer: Fractal Fibonacci
Positioning" section); the near-duplicate `docs/wiki/02-07-the-prism.md` carries a shorter
earlier draft of the same section (see [atomic-literal-shield](atomic-literal-shield.md)'s
Source note). Both kept in place.
