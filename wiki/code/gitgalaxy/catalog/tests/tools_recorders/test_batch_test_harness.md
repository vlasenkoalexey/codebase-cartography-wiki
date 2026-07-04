---
title: 'Module: tests/tools_recorders/test_batch_test_harness.py'
type: catalog
provenance: extracted
module: tests/tools_recorders/test_batch_test_harness.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.tools_recorders.test_batch_test_harness`/
symbols:
  test_happy_path: test_happy_path().
  test_maven_failure_path: test_maven_failure_path().
  test_timeout_path: test_timeout_path().
  mock_env: mock_env().
---
# Module: [`tests/tools_recorders/test_batch_test_harness.py`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_batch_test_harness.py)

## Functions
- `mock_env(tmp_path)` — [`L11`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_batch_test_harness.py#L11) — Sets up a fake directory structure in the OS temp folder.
- `test_happy_path(mock_run, mock_env)` — [`L31`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_batch_test_harness.py#L31) — Simulates a flawless run where Refractor, Java Forge, and Maven all succeed.
- `test_maven_failure_path(mock_run, mock_env)` — [`L58`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_batch_test_harness.py#L58) — Simulates Steps 1 & 2 succeeding, but Step 3 (Maven) failing with a compile error.
- `test_timeout_path(mock_run, mock_env)` — [`L85`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_batch_test_harness.py#L85) — Simulates the external script hanging and triggering the 5-minute kill switch.

