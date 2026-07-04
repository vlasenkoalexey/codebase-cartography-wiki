---
title: 'Module: tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_safe_to_edit_dependency_view`/
symbols:
  _write: _write().
  test_build_file_dependency_view_finds_python_imports_and_importers: test_build_file_dependency_view_finds_python_imports_and_importers().
  test_file_dependency_view_sorts_edges_and_supports_suffix_lookup: test_file_dependency_view_sorts_edges_and_supports_suffix_lookup().
  test_build_file_dependency_view_finds_typescript_imports: test_build_file_dependency_view_finds_typescript_imports().
  test_build_file_dependency_view_finds_java_imports: test_build_file_dependency_view_finds_java_imports().
  test_build_file_dependency_view_detects_package_init_importers: test_build_file_dependency_view_detects_package_init_importers().
  test_target_dependencies_returns_empty_for_unreadable_target: test_target_dependencies_returns_empty_for_unreadable_target().
  test_target_dependents_skips_unreadable_importers: test_target_dependents_skips_unreadable_importers().
  test_safe_graph_lookup_tolerates_graph_exceptions: test_safe_graph_lookup_tolerates_graph_exceptions().
  test_safe_graph_lookup_does_not_match_partial_basename_suffix: test_safe_graph_lookup_does_not_match_partial_basename_suffix().
  test_target_dependents_returns_empty_without_import_needles: test_target_dependents_returns_empty_without_import_needles().
  test_iter_dependency_source_files_skips_hidden_files: test_iter_dependency_source_files_skips_hidden_files().
  test_import_spec_helpers_cover_unsupported_and_unresolved_cases: test_import_spec_helpers_cover_unsupported_and_unresolved_cases().
  test_safe_graph_lookup_tolerates_graph_exceptions.BrokenGraph: test_safe_graph_lookup_tolerates_graph_exceptions().BrokenGraph#
  test_target_dependencies_returns_empty_for_unreadable_target.flaky_read_text: test_target_dependencies_returns_empty_for_unreadable_target().flaky_read_text().
  test_target_dependents_skips_unreadable_importers.flaky_read_text: test_target_dependents_skips_unreadable_importers().flaky_read_text().
  test_safe_graph_lookup_tolerates_graph_exceptions.BrokenGraph._nodes: test_safe_graph_lookup_tolerates_graph_exceptions().BrokenGraph#_nodes.
  test_safe_graph_lookup_tolerates_graph_exceptions.BrokenGraph.dependencies_of: test_safe_graph_lookup_tolerates_graph_exceptions().BrokenGraph#dependencies_of().
---
# Module: [`tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py)

## Classes
### `BrokenGraph`
- def: [`tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py:38`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L38)
- signature: `class BrokenGraph:`
- members:
  - `dependencies_of(self, _file_rel: str)` — [`L41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L41)
- protocol/private: `_nodes`[`L39`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L39)
- used by: (1 test-only callers)

## Functions
- `_write(root: Path, rel_path: str, body: str)` — [`L19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L19)
- `flaky_read_text(path: Path, *args, **kwargs)` — [`L129`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L129)
- `flaky_read_text(path: Path, *args, **kwargs)` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L147)
- `test_build_file_dependency_view_detects_package_init_importers(tmp_path: Path)` — [`L112`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L112)
- `test_build_file_dependency_view_finds_java_imports(tmp_path: Path)` — [`L97`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L97)
- `test_build_file_dependency_view_finds_python_imports_and_importers(tmp_path: Path)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L58)
- `test_build_file_dependency_view_finds_typescript_imports(tmp_path: Path)` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L83)
- `test_file_dependency_view_sorts_edges_and_supports_suffix_lookup()` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L26)
- `test_import_spec_helpers_cover_unsupported_and_unresolved_cases(tmp_path: Path)` — [`L181`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L181)
- `test_iter_dependency_source_files_skips_hidden_files(tmp_path: Path)` — [`L171`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L171)
- `test_safe_graph_lookup_does_not_match_partial_basename_suffix()` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L47)
- `test_safe_graph_lookup_tolerates_graph_exceptions()` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L37)
- `test_target_dependencies_returns_empty_for_unreadable_target(tmp_path: Path, monkeypatch)` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L123)
- `test_target_dependents_returns_empty_without_import_needles(tmp_path: Path, monkeypatch)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L157)
- `test_target_dependents_skips_unreadable_importers(tmp_path: Path, monkeypatch)` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_safe_to_edit_dependency_view.py#L139)

