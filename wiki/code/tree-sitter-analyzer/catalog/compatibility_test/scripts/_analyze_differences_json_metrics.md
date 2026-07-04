---
title: 'Module: compatibility_test/scripts/_analyze_differences_json_metrics.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/_analyze_differences_json_metrics.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts._analyze_differences_json_metrics`/
symbols:
  extract_performance_metrics: extract_performance_metrics().
  compare_performance_metrics: compare_performance_metrics().
  _performance_change: _performance_change().
  _is_performance_metric: _is_performance_metric().
---
# Module: [`compatibility_test/scripts/_analyze_differences_json_metrics.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_metrics.py)

## Functions
- `_is_performance_metric(key: str, value: Any)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_metrics.py#L54)
- `_performance_change(path: str, old_value: int | float, new_value: int | float)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_metrics.py#L38)
- `compare_performance_metrics(data_a: Any, data_b: Any)` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_metrics.py#L6) — Analyze changed performance metrics.
- `extract_performance_metrics(obj: Any, path: str = "")` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_metrics.py#L22) — Extract numeric performance-like fields from nested dictionaries.

