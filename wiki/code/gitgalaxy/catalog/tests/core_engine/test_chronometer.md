---
title: 'Module: tests/core_engine/test_chronometer.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_chronometer.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_chronometer`/test_
symbols:
  test_get_file_history_metrics: get_file_history_metrics().
  test_scan_git_history_and_stream: scan_git_history_and_stream().
  test_chronometer_no_git_fallback: chronometer_no_git_fallback().
  test_chronometer_git_boundaries: chronometer_git_boundaries().
  test_load_ignored_revs: load_ignored_revs().
  test_chronometer_git_boundaries.git_side_effect: chronometer_git_boundaries().git_side_effect().
---
# Module: [`tests/core_engine/test_chronometer.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer.py)

## Functions
- `git_side_effect(cmd, **kwargs)` — [`L42`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer.py#L42)
- `test_chronometer_git_boundaries(mock_run, tmp_path)` — [`L36`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer.py#L36) — Proves the boundary scanner correctly extracts min/max times from git logs.
- `test_chronometer_no_git_fallback(mock_getmtime, mock_walk, mock_run, tmp_path)` — [`L13`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer.py#L13) — Proves the chronometer gracefully falls back to OS Walk if Git is missing.
- `test_get_file_history_metrics(mock_getmtime, tmp_path)` — [`L133`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer.py#L133) — Proves the Handover method returns cache hits and falls back cleanly. — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
- `test_load_ignored_revs(tmp_path)` — [`L71`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer.py#L71) — Proves the sensor strips cosmetic commits from the churn math.
- `test_scan_git_history_and_stream(mock_popen, mock_run, tmp_path)` — [`L91`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer.py#L91) — Proves the Popen stream handles quoted paths, skipped hashes, and empty lines. — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)

