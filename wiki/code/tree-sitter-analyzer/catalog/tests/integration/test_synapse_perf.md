---
title: 'Module: tests/integration/test_synapse_perf.py'
type: catalog
provenance: extracted
module: tests/integration/test_synapse_perf.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_synapse_perf`/
symbols:
  _run_index: _run_index().
  test_performance_index_regression_lt_30pct: test_performance_index_regression_lt_30pct().
  _TARGET_DIR: _TARGET_DIR.
  _OVERHEAD_BUDGET: _OVERHEAD_BUDGET.
  _REPO_ROOT: _REPO_ROOT.
  _RUNS: _RUNS.
---
# Module: [`tests/integration/test_synapse_perf.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_perf.py)

## Functions
- `_run_index(project_root: Path, db_dir: Path, monkeypatch: pytest.MonkeyPatch, *, enabled: bool)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_perf.py#L39) — One index pass; returns elapsed wall-clock seconds.
- `test_performance_index_regression_lt_30pct(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_perf.py#L72) — Resolver wall-clock <= 1.30 x baseline (median of 3 runs each).

## Module values
- `_OVERHEAD_BUDGET` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_perf.py#L36)
- `_REPO_ROOT` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_perf.py#L28)
- `_RUNS` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_perf.py#L35)
- `_TARGET_DIR` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_synapse_perf.py#L29)

