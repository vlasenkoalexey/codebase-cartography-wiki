---
title: 'Module: tests/unit/mcp/test_mcp_file_metrics_unification.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_file_metrics_unification.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_file_metrics_unification`/
symbols:
  py_file: py_file().
  test_file_metrics_cache_invalidates_on_content_change: test_file_metrics_cache_invalidates_on_content_change().
  _spy_line_metrics: _spy_line_metrics().
  test_file_metrics_cache_hit_avoids_recompute: test_file_metrics_cache_hit_avoids_recompute().
  test_file_metrics_schema_contains_required_fields: test_file_metrics_schema_contains_required_fields().
  _INITIAL_CONTENT: _INITIAL_CONTENT.
  _CHANGED_CONTENT: _CHANGED_CONTENT.
  _spy_line_metrics._spy: _spy_line_metrics()._spy().
---
# Module: [`tests/unit/mcp/test_mcp_file_metrics_unification.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py)

## Functions
- `_spy(content, language)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L26)
- `_spy_line_metrics(monkeypatch)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L19) — Patch _compute_line_metrics to count invocations; returns a [count] list.
- `py_file(tmp_path)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L11) — A fresh cache + a minimal Python test file.
- `test_file_metrics_cache_hit_avoids_recompute(py_file, tmp_path, monkeypatch)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L51)
- `test_file_metrics_cache_invalidates_on_content_change(py_file, tmp_path, monkeypatch)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L60)
- `test_file_metrics_schema_contains_required_fields(py_file, tmp_path)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L35)

## Module values
- `_CHANGED_CONTENT` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L7)
- `_INITIAL_CONTENT` — [`L6`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_file_metrics_unification.py#L6)

