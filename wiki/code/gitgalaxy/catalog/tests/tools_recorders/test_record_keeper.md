---
title: 'Module: tests/tools_recorders/test_record_keeper.py'
type: catalog
provenance: extracted
module: tests/tools_recorders/test_record_keeper.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.tools_recorders.test_record_keeper`/
symbols:
  keeper: keeper().
  mock_pipeline_state: mock_pipeline_state().
  test_record_keeper_schema_creation: test_record_keeper_schema_creation().
  test_record_keeper_data_insertion: test_record_keeper_data_insertion().
  test_record_keeper_idempotency: test_record_keeper_idempotency().
  test_record_keeper_empty_state: test_record_keeper_empty_state().
---
# Module: [`tests/tools_recorders/test_record_keeper.py`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_record_keeper.py)

## Functions
- `keeper()` — [`L8`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_record_keeper.py#L8) — Initializes the RecordKeeper with a controlled schema for deterministic testing.
- `mock_pipeline_state()` — [`L19`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_record_keeper.py#L19) — Provides a comprehensive, standardized pipeline state for the DB recorder.
- `test_record_keeper_data_insertion(keeper, mock_pipeline_state, tmp_path)` — [`L175`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_record_keeper.py#L175) — Proves data flows cleanly from the complex RAM dictionary into relational tables.
- `test_record_keeper_empty_state(keeper, tmp_path)` — [`L261`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_record_keeper.py#L261) — Proves the SQLite generator survives a completely empty repository without math faults.
- `test_record_keeper_idempotency(keeper, mock_pipeline_state, tmp_path)` — [`L231`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_record_keeper.py#L231) — Proves that running the recorder twice for the same commit does not duplicate data.
- `test_record_keeper_schema_creation(keeper, mock_pipeline_state, tmp_path)` — [`L138`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_record_keeper.py#L138) — Proves the SQLite database generates the correct DevSecOps tables and columns.

