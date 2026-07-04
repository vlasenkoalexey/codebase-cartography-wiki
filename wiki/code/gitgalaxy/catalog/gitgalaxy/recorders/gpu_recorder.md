---
title: 'Module: gitgalaxy/recorders/gpu_recorder.py'
type: catalog
provenance: extracted
module: gitgalaxy/recorders/gpu_recorder.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.recorders.gpu_recorder`/GPURecorder#
symbols:
  GPURecorder.record_mission: record_mission().
  GPURecorder._intern: _intern().
  GPURecorder: ''
  GPURecorder.logger: logger.
  GPURecorder.archetype_lookup: archetype_lookup.
  GPURecorder.save_minified: save_minified().
  GPURecorder.lang_lookup: lang_lookup.
  GPURecorder.author_lookup: author_lookup.
  GPURecorder.proof_lookup: proof_lookup.
  GPURecorder.purpose_lookup: purpose_lookup.
  GPURecorder.reason_lookup: reason_lookup.
  GPURecorder.ext_lookup: ext_lookup.
  GPURecorder.import_lookup: import_lookup.
  GPURecorder.texture_lookup: texture_lookup.
  GPURecorder.dir_group_lookup: dir_group_lookup.
  GPURecorder.RISK_SCHEMA: RISK_SCHEMA.
  GPURecorder.HIT_SCHEMA: HIT_SCHEMA.
  GPURecorder.FUNCTION_SCHEMA: FUNCTION_SCHEMA.
  GPURecorder.__init__: __init__().
  GPURecorder.version: version.
---
# Module: [`gitgalaxy/recorders/gpu_recorder.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py)

## Classes
### `GPURecorder`
- def: [`gitgalaxy/recorders/gpu_recorder.py:25`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L25)
- doc: GPU Telemetry Recorder (WebGL Payload Generator).
- signature: `class GPURecorder:`
- members:
  - `_intern(self, val: str, registry: List[str])` — [`L379`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L379) — Minifies payload footprints by mapping repetitive strings to integer IDs.
  - `record_mission(self, parsed_files: List[Dict], unparsable_files: List[Dict], summary: Dict, forensic_report: Dict, repo_name: str, commit_hash: str = "untracked_local", branch_name: str = "unknown_branch")` — [`L67`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L67) — Orchestrates the synthesis and implementation of Destructive RAM Eviction. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `save_minified(self, payload: Dict[str, Any], filename: str)` — [`L385`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L385) — Serializes with maximum JSON compression to the provided output path.
  - `FUNCTION_SCHEMA` — [`L65`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L65)
  - `HIT_SCHEMA` — [`L64`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L64)
  - `RISK_SCHEMA` — [`L63`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L63)
  - `archetype_lookup` — [`L60`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L60)
  - `author_lookup` — [`L52`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L52)
  - `dir_group_lookup` — [`L59`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L59)
  - `ext_lookup` — [`L56`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L56)
  - `import_lookup` — [`L57`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L57)
  - `lang_lookup` — [`L51`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L51)
  - `logger` — [`L44`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L44)
  - `proof_lookup` — [`L53`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L53)
  - `purpose_lookup` — [`L54`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L54)
  - `reason_lookup` — [`L55`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L55)
  - `texture_lookup` — [`L58`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L58)
  - `version` — [`L43`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L43)
- protocol/private: `__init__`[`L42`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/gpu_recorder.py#L42)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`gpu_recorder`](../galaxyscope.md#Orchestrator.gpu_recorder)  (1 test-only)

