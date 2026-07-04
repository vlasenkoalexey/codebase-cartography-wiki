---
title: 'Module: tests/unit/test_change_impact_cached_graph.py'
type: catalog
provenance: extracted
module: tests/unit/test_change_impact_cached_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_change_impact_cached_graph`/
symbols:
  test_cached_dependency_graph_methods_ignore_invalid_edges: test_cached_dependency_graph_methods_ignore_invalid_edges().
  test_cached_dependency_graph_resolves_python_relative_edges: test_cached_dependency_graph_resolves_python_relative_edges().
  test_cached_dependency_graph_resolves_js_relative_edges: test_cached_dependency_graph_resolves_js_relative_edges().
  test_add_cached_import_edges_normalizes_windows_resolver_paths: test_add_cached_import_edges_normalizes_windows_resolver_paths().
  _index_project: _index_project().
  test_add_cached_import_edges_ignores_unsupported_languages: test_add_cached_import_edges_ignores_unsupported_languages().
  test_cached_index_rows_handles_query_failure: test_cached_index_rows_handles_query_failure().
  test_cached_index_rows_handles_query_failure.BadCache.get_conn: test_cached_index_rows_handles_query_failure().BadCache#get_conn().
  test_load_cached_dependency_graph_returns_none_without_cache: test_load_cached_dependency_graph_returns_none_without_cache().
  test_cached_import_module_parsers_cover_supported_languages: test_cached_import_module_parsers_cover_supported_languages().
  test_iter_cached_import_modules_handles_invalid_json_and_dict_rows: test_iter_cached_import_modules_handles_invalid_json_and_dict_rows().
  test_cached_index_rows_handles_query_failure.BadCache._get_conn: test_cached_index_rows_handles_query_failure().BadCache#_get_conn().
  test_cached_index_rows_handles_query_failure.BadConn: test_cached_index_rows_handles_query_failure().BadConn#
  test_cached_index_rows_handles_query_failure.BadCache: test_cached_index_rows_handles_query_failure().BadCache#
  test_cached_index_rows_handles_query_failure.BadConn.execute: test_cached_index_rows_handles_query_failure().BadConn#execute().
---
# Module: [`tests/unit/test_change_impact_cached_graph.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py)

## Classes
### `BadCache`
- def: [`tests/unit/test_change_impact_cached_graph.py:122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L122)
- signature: `class BadCache:`
- members:
  - `get_conn(self)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L123)
- protocol/private: `_get_conn`[`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L126)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `BadConn`
- def: [`tests/unit/test_change_impact_cached_graph.py:118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L118)
- signature: `class BadConn:`
- members:
  - `execute(self, query)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L119)
- used by: (1 test-only callers)

## Functions
- `_index_project(root)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L12)
- `test_add_cached_import_edges_ignores_unsupported_languages(tmp_path)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L132)
- `test_add_cached_import_edges_normalizes_windows_resolver_paths(tmp_path, monkeypatch)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L144)
- `test_cached_dependency_graph_methods_ignore_invalid_edges(tmp_path)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L63)
- `test_cached_dependency_graph_resolves_js_relative_edges(tmp_path)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L43)
- `test_cached_dependency_graph_resolves_python_relative_edges(tmp_path)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L25)
- `test_cached_import_module_parsers_cover_supported_languages()` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L76)
- `test_cached_index_rows_handles_query_failure()` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L117)
- `test_iter_cached_import_modules_handles_invalid_json_and_dict_rows()` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L106)
- `test_load_cached_dependency_graph_returns_none_without_cache(tmp_path)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_cached_graph.py#L20)

