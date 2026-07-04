---
title: 'Module: tests/core_engine/test_chronometer_timeout.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_chronometer_timeout.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_chronometer_timeout`/TestChronometerTimeout#
symbols:
  TestChronometerTimeout.test_zombie_process_kill_switch: test_zombie_process_kill_switch().
  TestChronometerTimeout.infinite_git_log: infinite_git_log().
  TestChronometerTimeout: ''
---
# Module: [`tests/core_engine/test_chronometer_timeout.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer_timeout.py)

## Classes
### `TestChronometerTimeout`  ·  implements/extends TestCase
- def: [`tests/core_engine/test_chronometer_timeout.py:10`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer_timeout.py#L10)
- signature: `class TestChronometerTimeout(unittest.TestCase):`
- members:
  - `infinite_git_log()` — [`L23`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer_timeout.py#L23)
  - `test_zombie_process_kill_switch(self, mock_calibrate, mock_popen)` — [`L15`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_chronometer_timeout.py#L15) — Simulates an infinite, hanging Git stream.
- uses (calls/refs, reference-scoped): [`_stream_git_log`](../../gitgalaxy/metrics/chronometer.md#Chronometer._stream_git_log), [`Chronometer`](../../gitgalaxy/metrics/chronometer.md#Chronometer)

