---
title: 'Module: tests/e2e/test_user_journeys.py'
type: catalog
provenance: extracted
module: tests/e2e/test_user_journeys.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.e2e.test_user_journeys`/
symbols:
  TestUserJourneys.run_cgc: TestUserJourneys#run_cgc().
  TestUserJourneys.test_first_time_user_workflow: TestUserJourneys#test_first_time_user_workflow().
  TestUserJourneys.test_clean_up: TestUserJourneys#test_clean_up().
  KUZU_AVAILABLE: KUZU_AVAILABLE.
  TestUserJourneys: TestUserJourneys#
---
# Module: [`tests/e2e/test_user_journeys.py`](../../../../../../raw/code/codegraphcontext/tests/e2e/test_user_journeys.py)

## Classes
### `TestUserJourneys`
- def: [`tests/e2e/test_user_journeys.py:15`](../../../../../../raw/code/codegraphcontext/tests/e2e/test_user_journeys.py#L15)
- doc: End-to-End User Journeys.
- signature: `class TestUserJourneys:`
- members:
  - `run_cgc(self, args, cwd=None, db_path=None)` — [`L22`](../../../../../../raw/code/codegraphcontext/tests/e2e/test_user_journeys.py#L22) — Helper to run cgc cli.
  - `test_clean_up(self, temp_test_dir)` — [`L66`](../../../../../../raw/code/codegraphcontext/tests/e2e/test_user_journeys.py#L66) — User wants to remove a repo.
  - `test_first_time_user_workflow(self, python_sample_project, temp_test_dir)` — [`L32`](../../../../../../raw/code/codegraphcontext/tests/e2e/test_user_journeys.py#L32) — Scenario:
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Module values
- `KUZU_AVAILABLE` — [`L10`](../../../../../../raw/code/codegraphcontext/tests/e2e/test_user_journeys.py#L10)

