---
title: 'Module: tests/unit/languages/test_python_deep_nesting_779.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_deep_nesting_779.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_deep_nesting_779`/
symbols:
  _extract_function_names: _extract_function_names().
  _build_nested_source: _build_nested_source().
  TestDeepNestedFunctionExtraction.test_25_nested_functions_all_extracted: TestDeepNestedFunctionExtraction#test_25_nested_functions_all_extracted().
  TestDeepNestedFunctionExtraction.test_26_nested_functions_all_extracted: TestDeepNestedFunctionExtraction#test_26_nested_functions_all_extracted().
  TestDeepNestedFunctionExtraction.test_30_nested_functions_all_extracted: TestDeepNestedFunctionExtraction#test_30_nested_functions_all_extracted().
  TestDeepNestedFunctionExtraction.test_50_nested_functions_all_extracted: TestDeepNestedFunctionExtraction#test_50_nested_functions_all_extracted().
  TestDeepNestedFunctionExtraction.test_deepest_function_name_is_correct: TestDeepNestedFunctionExtraction#test_deepest_function_name_is_correct().
  TestMaxTraversalDepthConstant.test_max_traversal_depth_is_at_least_200: TestMaxTraversalDepthConstant#test_max_traversal_depth_is_at_least_200().
  pytestmark: pytestmark.
  TestMaxTraversalDepthConstant: TestMaxTraversalDepthConstant#
  TestDeepNestedFunctionExtraction: TestDeepNestedFunctionExtraction#
---
# Module: [`tests/unit/languages/test_python_deep_nesting_779.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py)

## Classes
### `TestDeepNestedFunctionExtraction`
- def: [`tests/unit/languages/test_python_deep_nesting_779.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L54)
- doc: Deeply nested Python functions must all be extracted without silent truncation.
- signature: `class TestDeepNestedFunctionExtraction:`
- members:
  - `test_25_nested_functions_all_extracted(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L57) — L0..L24 (25 levels) — the old threshold boundary.
  - `test_26_nested_functions_all_extracted(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L62) — L0..L25 (26 levels) — one beyond the old limit (#779 repro start).
  - `test_30_nested_functions_all_extracted(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L67) — L0..L29 (30 levels) — the exact repro from #779.
  - `test_50_nested_functions_all_extracted(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L75) — L0..L49 (50 levels) — well into territory that previously failed.
  - `test_deepest_function_name_is_correct(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L80) — The last extracted name must be the deepest level, not an earlier one.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestMaxTraversalDepthConstant`
- def: [`tests/unit/languages/test_python_deep_nesting_779.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L42)
- doc: The depth limit must support at least 99 Python nesting levels.
- signature: `class TestMaxTraversalDepthConstant:`
- members:
  - `test_max_traversal_depth_is_at_least_200(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L45)
- uses (calls/refs, reference-scoped): [`_MAX_TRAVERSAL_DEPTH`](../../../tree_sitter_analyzer/languages/python_plugin/_traversal_helpers.md#_MAX_TRAVERSAL_DEPTH)

## Functions
- `_build_nested_source(n: int)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L32) — Generate Python source with n deeply nested functions L0..L(n-1).
- `_extract_function_names(source: str)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L20) — Extract function names from Python source via PythonPlugin.

## Module values
- `pytestmark` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_deep_nesting_779.py#L17)

