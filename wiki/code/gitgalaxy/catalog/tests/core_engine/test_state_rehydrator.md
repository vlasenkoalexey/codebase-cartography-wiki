---
title: 'Module: tests/core_engine/test_state_rehydrator.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_state_rehydrator.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_state_rehydrator`/
symbols:
  test_rehydrator_cold_start: test_rehydrator_cold_start().
  test_rehydrator_missing_repo: test_rehydrator_missing_repo().
  test_rehydrator_successful_load: test_rehydrator_successful_load().
  mock_db: mock_db().
---
# Module: [`tests/core_engine/test_state_rehydrator.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_state_rehydrator.py)

## Functions
- `mock_db(tmp_path)` — [`L13`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_state_rehydrator.py#L13) — Creates a temporary SQLite database populated with mock schema and data.
- `test_rehydrator_cold_start(tmp_path)` — [`L76`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_state_rehydrator.py#L76) — Proves the rehydrator safely returns None if the master DB is missing.
- `test_rehydrator_missing_repo(mock_db)` — [`L88`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_state_rehydrator.py#L88) — Proves the rehydrator safely returns None if the repo history is empty.
- `test_rehydrator_successful_load(mock_db)` — [`L99`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_state_rehydrator.py#L99) — Proves the rehydrator fetches the most recent commit based on time,

