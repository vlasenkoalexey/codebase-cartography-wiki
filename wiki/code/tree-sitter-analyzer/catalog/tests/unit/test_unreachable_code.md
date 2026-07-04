---
title: 'Module: tests/unit/test_unreachable_code.py'
type: catalog
provenance: extracted
module: tests/unit/test_unreachable_code.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_unreachable_code`/
symbols:
  TestUnreachableBlockDataclass.test_defaults: TestUnreachableBlockDataclass#test_defaults().
  TestUnreachableBlockDataclass.test_custom_severity: TestUnreachableBlockDataclass#test_custom_severity().
  TestUnreachableCodeResultDataclass.test_to_dict_counts_match: TestUnreachableCodeResultDataclass#test_to_dict_counts_match().
  TestAnalyzeFileUnreachable.test_clean_file_returns_no_blocks: TestAnalyzeFileUnreachable#test_clean_file_returns_no_blocks().
  TestUnreachableCodeResultDataclass.test_default_fields: TestUnreachableCodeResultDataclass#test_default_fields().
  _write_py: _write_py().
  TestAnalyzeFileUnreachable.test_code_after_return_is_flagged: TestAnalyzeFileUnreachable#test_code_after_return_is_flagged().
  TestAnalyzeFileUnreachable.test_code_after_raise_is_flagged: TestAnalyzeFileUnreachable#test_code_after_raise_is_flagged().
  TestAnalyzeFileUnreachable.test_if_false_branch_is_flagged: TestAnalyzeFileUnreachable#test_if_false_branch_is_flagged().
  TestAnalyzeFileUnreachable.test_if_true_else_is_flagged: TestAnalyzeFileUnreachable#test_if_true_else_is_flagged().
  TestAnalyzeFileUnreachable.test_language_override: TestAnalyzeFileUnreachable#test_language_override().
  TestAnalyzeFileUnreachable.test_unreachable_block_to_dict_schema: TestAnalyzeFileUnreachable#test_unreachable_block_to_dict_schema().
  TestAnalyzeFileUnreachable.test_multiple_functions_all_analyzed: TestAnalyzeFileUnreachable#test_multiple_functions_all_analyzed().
  TestAnalyzeFileUnreachable.test_nested_function_detected: TestAnalyzeFileUnreachable#test_nested_function_detected().
  TestAnalyzeFileUnreachable.test_severity_is_warning_for_after_return: TestAnalyzeFileUnreachable#test_severity_is_warning_for_after_return().
  TestAnalyzeFileUnreachable.test_unknown_extension_returns_error: TestAnalyzeFileUnreachable#test_unknown_extension_returns_error().
  TestAnalyzeFileUnreachable.test_result_to_dict_schema: TestAnalyzeFileUnreachable#test_result_to_dict_schema().
  TestAnalyzeProjectUnreachable.test_project_with_dead_code_returns_results: TestAnalyzeProjectUnreachable#test_project_with_dead_code_returns_results().
  TestAnalyzeFileUnreachable.test_nonexistent_file_returns_error: TestAnalyzeFileUnreachable#test_nonexistent_file_returns_error().
  TestAnalyzeProjectUnreachable.test_clean_project_returns_no_results: TestAnalyzeProjectUnreachable#test_clean_project_returns_no_results().
  TestAnalyzeProjectUnreachable.test_max_files_respected: TestAnalyzeProjectUnreachable#test_max_files_respected().
  TestIsFalseLiteral.test_python_false: TestIsFalseLiteral#test_python_false().
  TestIsFalseLiteral.test_js_false: TestIsFalseLiteral#test_js_false().
  TestIsFalseLiteral.test_null_is_false: TestIsFalseLiteral#test_null_is_false().
  TestIsFalseLiteral.test_none_node_returns_false: TestIsFalseLiteral#test_none_node_returns_false().
  TestIsFalseLiteral.test_truthy_value_returns_false: TestIsFalseLiteral#test_truthy_value_returns_false().
  TestIsTrueLiteral.test_python_true: TestIsTrueLiteral#test_python_true().
  TestIsTrueLiteral.test_js_true: TestIsTrueLiteral#test_js_true().
  TestIsTrueLiteral.test_integer_one: TestIsTrueLiteral#test_integer_one().
  TestIsTrueLiteral.test_none_node_returns_false: TestIsTrueLiteral#test_none_node_returns_false().
  TestIsTrueLiteral.test_false_value_returns_false: TestIsTrueLiteral#test_false_value_returns_false().
  TestAnalyzeProjectUnreachable.test_empty_project_returns_empty: TestAnalyzeProjectUnreachable#test_empty_project_returns_empty().
  TestAnalyzeProjectUnreachable.test_test_files_excluded_by_default: TestAnalyzeProjectUnreachable#test_test_files_excluded_by_default().
  TestAnalyzeProjectUnreachable.test_test_files_included_when_opted_in: TestAnalyzeProjectUnreachable#test_test_files_included_when_opted_in().
  TestAnalyzeProjectUnreachable.test_excludes_dot_dirs: TestAnalyzeProjectUnreachable#test_excludes_dot_dirs().
  TestIsFalseLiteral: TestIsFalseLiteral#
  TestIsTrueLiteral: TestIsTrueLiteral#
  TestAnalyzeFileUnreachable: TestAnalyzeFileUnreachable#
  TestAnalyzeProjectUnreachable: TestAnalyzeProjectUnreachable#
  TestUnreachableBlockDataclass: TestUnreachableBlockDataclass#
  TestUnreachableCodeResultDataclass: TestUnreachableCodeResultDataclass#
---
# Module: [`tests/unit/test_unreachable_code.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py)

## Classes
### `TestAnalyzeFileUnreachable`
- def: [`tests/unit/test_unreachable_code.py:102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L102)
- doc: Tests for analyze_file_unreachable() using real temporary source files.
- signature: `class TestAnalyzeFileUnreachable:`
- members:
  - `test_clean_file_returns_no_blocks(self, tmp_path)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L105)
  - `test_code_after_raise_is_flagged(self, tmp_path)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L136)
  - `test_code_after_return_is_flagged(self, tmp_path)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L120)
  - `test_if_false_branch_is_flagged(self, tmp_path)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L149)
  - `test_if_true_else_is_flagged(self, tmp_path)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L166)
  - `test_language_override(self, tmp_path)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L194)
  - `test_multiple_functions_all_analyzed(self, tmp_path)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L245)
  - `test_nested_function_detected(self, tmp_path)` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L263)
  - `test_nonexistent_file_returns_error(self, tmp_path)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L190)
  - `test_result_to_dict_schema(self, tmp_path)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L207)
  - `test_severity_is_warning_for_after_return(self, tmp_path)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L281)
  - `test_unknown_extension_returns_error(self, tmp_path)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L183)
  - `test_unreachable_block_to_dict_schema(self, tmp_path)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L225)
- uses (calls/refs, reference-scoped): [`analyze_file_unreachable`](../../tree_sitter_analyzer/unreachable_code.md#analyze_file_unreachable), [`unreachable_blocks`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.unreachable_blocks), [`to_dict`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.to_dict), [`UnreachableCodeResult`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult), [`to_dict`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.to_dict), [`errors`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.errors), [`reason`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.reason), [`language`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.language), [`functions_analyzed`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.functions_analyzed), [`severity`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.severity)  (1 test-only)

### `TestAnalyzeProjectUnreachable`
- def: [`tests/unit/test_unreachable_code.py:296`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L296)
- doc: Tests for analyze_project_unreachable() — directory walk.
- signature: `class TestAnalyzeProjectUnreachable:`
- members:
  - `test_clean_project_returns_no_results(self, tmp_path)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L303)
  - `test_empty_project_returns_empty(self, tmp_path)` — [`L299`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L299)
  - `test_excludes_dot_dirs(self, tmp_path)` — [`L375`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L375)
  - `test_max_files_respected(self, tmp_path)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L360)
  - `test_project_with_dead_code_returns_results(self, tmp_path)` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L315)
  - `test_test_files_excluded_by_default(self, tmp_path)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L329)
  - `test_test_files_included_when_opted_in(self, tmp_path)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L345)
- uses (calls/refs, reference-scoped): [`unreachable_blocks`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.unreachable_blocks), [`analyze_project_unreachable`](../../tree_sitter_analyzer/unreachable_code.md#analyze_project_unreachable)  (1 test-only)

### `TestIsFalseLiteral`
- def: [`tests/unit/test_unreachable_code.py:39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L39)
- signature: `class TestIsFalseLiteral:`
- members:
  - `test_js_false(self, mocker)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L46)
  - `test_none_node_returns_false(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L58)
  - `test_null_is_false(self, mocker)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L52)
  - `test_python_false(self, mocker)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L40)
  - `test_truthy_value_returns_false(self, mocker)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L61)
- uses (calls/refs, reference-scoped): [`_is_false_literal`](../../tree_sitter_analyzer/unreachable_code.md#_is_false_literal)

### `TestIsTrueLiteral`
- def: [`tests/unit/test_unreachable_code.py:68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L68)
- signature: `class TestIsTrueLiteral:`
- members:
  - `test_false_value_returns_false(self, mocker)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L90)
  - `test_integer_one(self, mocker)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L81)
  - `test_js_true(self, mocker)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L75)
  - `test_none_node_returns_false(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L87)
  - `test_python_true(self, mocker)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L69)
- uses (calls/refs, reference-scoped): [`_is_true_literal`](../../tree_sitter_analyzer/unreachable_code.md#_is_true_literal)

### `TestUnreachableBlockDataclass`
- def: [`tests/unit/test_unreachable_code.py:392`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L392)
- signature: `class TestUnreachableBlockDataclass:`
- members:
  - `test_custom_severity(self)` — [`L404`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L404)
  - `test_defaults(self)` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L393)
- uses (calls/refs, reference-scoped): [`UnreachableBlock`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock), [`to_dict`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.to_dict), [`reason`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.reason), [`severity`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.severity), [`end_line`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.end_line), [`function_name`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.function_name), [`start_line`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.start_line), [`file_path`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock.file_path)

### `TestUnreachableCodeResultDataclass`
- def: [`tests/unit/test_unreachable_code.py:416`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L416)
- signature: `class TestUnreachableCodeResultDataclass:`
- members:
  - `test_default_fields(self)` — [`L417`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L417)
  - `test_to_dict_counts_match(self)` — [`L423`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L423)
- uses (calls/refs, reference-scoped): [`unreachable_blocks`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.unreachable_blocks), [`UnreachableBlock`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableBlock), [`to_dict`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.to_dict), [`UnreachableCodeResult`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult), [`errors`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.errors), [`language`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.language), [`file_path`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.file_path), [`functions_analyzed`](../../tree_sitter_analyzer/unreachable_code.md#UnreachableCodeResult.functions_analyzed)

## Functions
- `_write_py(tmp_path: Path, name: str, code: str)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_unreachable_code.py#L27) — Write a Python source file and return its str path.

