---
title: 'Module: gitgalaxy/recorders/record_keeper.py'
type: catalog
provenance: extracted
module: gitgalaxy/recorders/record_keeper.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.recorders.record_keeper`/RecordKeeper#
symbols:
  RecordKeeper.record_mission: record_mission().
  RecordKeeper.SIGNAL_SCHEMA: SIGNAL_SCHEMA.
  RecordKeeper.RISK_SCHEMA: RISK_SCHEMA.
  RecordKeeper.logger: logger.
  RecordKeeper: ''
  RecordKeeper.SHORT_KEY_MAP: SHORT_KEY_MAP.
  RecordKeeper.__init__: __init__().
---
# Module: [`gitgalaxy/recorders/record_keeper.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py)

## Classes
### `RecordKeeper`
- def: [`gitgalaxy/recorders/record_keeper.py:19`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py#L19)
- doc: SQLite Telemetry Recorder.
- signature: `class RecordKeeper:`
- members:
  - `record_mission(self, parsed_files: List[Dict], unparsable_files: List[Dict], summary: Dict, session_meta: Dict, output_path: str)` — [`L120`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py#L120) — Builds the formal relational SQLite database directly from pipeline RAM state. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `RISK_SCHEMA` — [`L32`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py#L32)
  - `SHORT_KEY_MAP` — [`L36`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py#L36)
  - `SIGNAL_SCHEMA` — [`L33`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py#L33)
  - `logger` — [`L29`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py#L29) — documented in [gitgalaxy-standards-analysis_lens](../../../concepts/gitgalaxy-standards-analysis_lens.md)
- protocol/private: `__init__`[`L28`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/record_keeper.py#L28)
- uses (calls/refs, reference-scoped): [`RECORDING_SCHEMAS`](../standards/analysis_lens.md#RECORDING_SCHEMAS)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`execute_incremental_scan`](../galaxyscope.md#Orchestrator.execute_incremental_scan), [`db_recorder`](../galaxyscope.md#Orchestrator.db_recorder)  (1 test-only)

