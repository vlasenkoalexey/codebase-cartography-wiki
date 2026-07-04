---
title: 'Module: tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_class_hierarchy_and_dep_matrix_cli`/
symbols:
  _args: _args().
  test_class_hierarchy_summary_cli: test_class_hierarchy_summary_cli().
  test_code_similarity_cli_passes_path_filter: test_code_similarity_cli_passes_path_filter().
  test_class_hierarchy_subclasses_cli: test_class_hierarchy_subclasses_cli().
  test_class_hierarchy_impact_cli: test_class_hierarchy_impact_cli().
  test_dependency_matrix_summary_cli: test_dependency_matrix_summary_cli().
  test_dependency_matrix_hotspots_cli: test_dependency_matrix_hotspots_cli().
  test_dependency_matrix_unstable_cli: test_dependency_matrix_unstable_cli().
  test_dependency_matrix_file_cli: test_dependency_matrix_file_cli().
  test_symbol_lineage_empty_string_returns_error_not_usage_dump: test_symbol_lineage_empty_string_returns_error_not_usage_dump().
  test_symbol_lineage_whitespace_only_returns_error: test_symbol_lineage_whitespace_only_returns_error().
  test_symbol_search_empty_string_returns_error_not_file_path_fallback: test_symbol_search_empty_string_returns_error_not_file_path_fallback().
  test_symbol_search_whitespace_only_returns_error: test_symbol_search_whitespace_only_returns_error().
  test_class_hierarchy_summary_cli.FakeClassHierarchyTool: test_class_hierarchy_summary_cli().FakeClassHierarchyTool#
  test_code_similarity_cli_passes_path_filter.FakeCodeGraphSimilarityTool: test_code_similarity_cli_passes_path_filter().FakeCodeGraphSimilarityTool#
  test_class_hierarchy_subclasses_cli.FakeClassHierarchyTool: test_class_hierarchy_subclasses_cli().FakeClassHierarchyTool#
  test_class_hierarchy_impact_cli.FakeClassHierarchyTool: test_class_hierarchy_impact_cli().FakeClassHierarchyTool#
  test_dependency_matrix_summary_cli.FakeDependencyMatrixTool: test_dependency_matrix_summary_cli().FakeDependencyMatrixTool#
  test_dependency_matrix_hotspots_cli.FakeDependencyMatrixTool: test_dependency_matrix_hotspots_cli().FakeDependencyMatrixTool#
  test_dependency_matrix_unstable_cli.FakeDependencyMatrixTool: test_dependency_matrix_unstable_cli().FakeDependencyMatrixTool#
  test_dependency_matrix_file_cli.FakeDependencyMatrixTool: test_dependency_matrix_file_cli().FakeDependencyMatrixTool#
  test_class_hierarchy_summary_cli.FakeClassHierarchyTool.__init__: test_class_hierarchy_summary_cli().FakeClassHierarchyTool#__init__().
  test_class_hierarchy_summary_cli.FakeClassHierarchyTool.execute: test_class_hierarchy_summary_cli().FakeClassHierarchyTool#execute().
  test_code_similarity_cli_passes_path_filter.FakeCodeGraphSimilarityTool.__init__: test_code_similarity_cli_passes_path_filter().FakeCodeGraphSimilarityTool#__init__().
  test_code_similarity_cli_passes_path_filter.FakeCodeGraphSimilarityTool.execute: test_code_similarity_cli_passes_path_filter().FakeCodeGraphSimilarityTool#execute().
  test_class_hierarchy_subclasses_cli.FakeClassHierarchyTool.__init__: test_class_hierarchy_subclasses_cli().FakeClassHierarchyTool#__init__().
  test_class_hierarchy_subclasses_cli.FakeClassHierarchyTool.execute: test_class_hierarchy_subclasses_cli().FakeClassHierarchyTool#execute().
  test_class_hierarchy_impact_cli.FakeClassHierarchyTool.__init__: test_class_hierarchy_impact_cli().FakeClassHierarchyTool#__init__().
  test_class_hierarchy_impact_cli.FakeClassHierarchyTool.execute: test_class_hierarchy_impact_cli().FakeClassHierarchyTool#execute().
  test_dependency_matrix_summary_cli.FakeDependencyMatrixTool.__init__: test_dependency_matrix_summary_cli().FakeDependencyMatrixTool#__init__().
  test_dependency_matrix_summary_cli.FakeDependencyMatrixTool.execute: test_dependency_matrix_summary_cli().FakeDependencyMatrixTool#execute().
  test_dependency_matrix_hotspots_cli.FakeDependencyMatrixTool.__init__: test_dependency_matrix_hotspots_cli().FakeDependencyMatrixTool#__init__().
  test_dependency_matrix_hotspots_cli.FakeDependencyMatrixTool.execute: test_dependency_matrix_hotspots_cli().FakeDependencyMatrixTool#execute().
  test_dependency_matrix_unstable_cli.FakeDependencyMatrixTool.__init__: test_dependency_matrix_unstable_cli().FakeDependencyMatrixTool#__init__().
  test_dependency_matrix_unstable_cli.FakeDependencyMatrixTool.execute: test_dependency_matrix_unstable_cli().FakeDependencyMatrixTool#execute().
  test_dependency_matrix_file_cli.FakeDependencyMatrixTool.__init__: test_dependency_matrix_file_cli().FakeDependencyMatrixTool#__init__().
  test_dependency_matrix_file_cli.FakeDependencyMatrixTool.execute: test_dependency_matrix_file_cli().FakeDependencyMatrixTool#execute().
---
# Module: [`tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py)

## Classes
### `FakeClassHierarchyTool`
- def: [`tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py:187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L187)
- signature: `class FakeClassHierarchyTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L75)
  - `execute(self, arguments: dict[str, Any])` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L154)
  - `execute(self, arguments: dict[str, Any])` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L191)
- protocol/private: `__init__`[`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L72), `__init__`[`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L151), `__init__`[`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L188)
- used by: (1 test-only callers)

### `FakeCodeGraphSimilarityTool`
- def: [`tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py:103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L103)
- signature: `class FakeCodeGraphSimilarityTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L107)
- protocol/private: `__init__`[`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L104)
- used by: (1 test-only callers)

### `FakeDependencyMatrixTool`
- def: [`tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py:340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L340)
- signature: `class FakeDependencyMatrixTool:`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L220)
  - `execute(self, arguments: dict[str, Any])` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L255)
  - `execute(self, arguments: dict[str, Any])` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L286)
  - `execute(self, arguments: dict[str, Any])` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L344)
- protocol/private: `__init__`[`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L217), `__init__`[`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L252), `__init__`[`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L283), `__init__`[`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L341)
- used by: (1 test-only callers)

## Functions
- `_args(**overrides: Any)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L11)
- `test_class_hierarchy_impact_cli(monkeypatch)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L184)
- `test_class_hierarchy_subclasses_cli(monkeypatch)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L147)
- `test_class_hierarchy_summary_cli(monkeypatch)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L68)
- `test_code_similarity_cli_passes_path_filter(monkeypatch)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L100)
- `test_dependency_matrix_file_cli(monkeypatch)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L337)
- `test_dependency_matrix_hotspots_cli(monkeypatch)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L248)
- `test_dependency_matrix_summary_cli(monkeypatch)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L213)
- `test_dependency_matrix_unstable_cli(monkeypatch)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L279)
- `test_symbol_lineage_empty_string_returns_error_not_usage_dump()` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L310) — #863: --symbol-lineage "" must emit a clean validation error, not a usage dump.
- `test_symbol_lineage_whitespace_only_returns_error()` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L324) — #863: --symbol-lineage '   ' is treated the same as empty.
- `test_symbol_search_empty_string_returns_error_not_file_path_fallback()` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L368) — #738: --symbol-search "" must emit a clean validation error, not 'File path not specified'.
- `test_symbol_search_whitespace_only_returns_error()` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_class_hierarchy_and_dep_matrix_cli.py#L383) — #738: --symbol-search '   ' is treated the same as empty.

