---
title: 'Module: gitgalaxy/core/spatial_mapper.py'
type: catalog
provenance: extracted
module: gitgalaxy/core/spatial_mapper.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.core.spatial_mapper`/SpatialMapper#
symbols:
  SpatialMapper.map_repository: map_repository().
  SpatialMapper._hash_jitter: _hash_jitter().
  SpatialMapper.logger: logger.
  SpatialMapper: ''
  SpatialMapper._get_magnitude: _get_magnitude().
  SpatialMapper.CORE_EXCLUSION_RADIUS: CORE_EXCLUSION_RADIUS.
  SpatialMapper.MACRO_STEP_FACTOR: MACRO_STEP_FACTOR.
  SpatialMapper.JITTER_MAGNITUDE: JITTER_MAGNITUDE.
  SpatialMapper._calculate_spatial_clearance: _calculate_spatial_clearance().
  SpatialMapper.MICRO_SPACING: MICRO_SPACING.
  SpatialMapper.MICRO_GOLDEN_ANGLE: MICRO_GOLDEN_ANGLE.
  SpatialMapper.MAX_TILT_DEG: MAX_TILT_DEG.
  SpatialMapper.__init__: __init__().
  SpatialMapper.MACRO_GOLDEN_ANGLE: MACRO_GOLDEN_ANGLE.
---
# Module: [`gitgalaxy/core/spatial_mapper.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py)

## Classes
### `SpatialMapper`
- def: [`gitgalaxy/core/spatial_mapper.py:19`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L19)
- doc: Transforms a flat list of artifacts into a deterministic 3D Cartesian coordinate map.
- signature: `class SpatialMapper:`
- members:
  - `_calculate_spatial_clearance(self, magnitude: float)` — [`L57`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L57) — Determines the required tight clearance radius for a node based on its structural magnitude.
  - `_get_magnitude(self, node: Dict[str, Any])` — [`L228`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L228) — Safely extracts structural magnitude regardless of which JSON version the pipeline is using.
  - `_hash_jitter(self, seed: str, amplitude: float)` — [`L64`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L64) — Applies a deterministic pseudo-random jitter based on a filename hash.
  - `map_repository(self, parsed_files: List[Dict[str, Any]])` — [`L77`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L77) — Injects 3D coordinates using a Ray-Casting Dynamic Mask. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `CORE_EXCLUSION_RADIUS` — [`L54`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L54)
  - `JITTER_MAGNITUDE` — [`L55`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L55)
  - `MACRO_GOLDEN_ANGLE` — [`L48`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L48)
  - `MACRO_STEP_FACTOR` — [`L52`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L52)
  - `MAX_TILT_DEG` — [`L53`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L53)
  - `MICRO_GOLDEN_ANGLE` — [`L45`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L45)
  - `MICRO_SPACING` — [`L51`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L51)
  - `logger` — [`L36`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L36)
- protocol/private: `__init__`[`L33`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/spatial_mapper.py#L33)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`spatial_mapper`](../galaxyscope.md#Orchestrator.spatial_mapper)  (3 test-only)

