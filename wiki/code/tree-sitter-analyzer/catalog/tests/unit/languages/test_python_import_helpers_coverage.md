---
title: 'Module: tests/unit/languages/test_python_import_helpers_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_import_helpers_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_import_helpers_coverage`/
symbols:
  TestExtractImportsFromTree.test_no_language_returns_empty: TestExtractImportsFromTree#test_no_language_returns_empty().
  TestExtractImportsFromTree.test_query_returns_empty_on_bad_language: TestExtractImportsFromTree#test_query_returns_empty_on_bad_language().
  TestQueryClassBodyNodes.test_no_language_returns_empty: TestQueryClassBodyNodes#test_no_language_returns_empty().
  TestQueryClassBodyNodes.test_query_exception_returns_empty: TestQueryClassBodyNodes#test_query_exception_returns_empty().
  TestImportNodeContext.test_creates_context: TestImportNodeContext#test_creates_context().
  _child_from_source: _child_from_source().
  TestParseSimpleImport.test_single_import: TestParseSimpleImport#test_single_import().
  TestParseSimpleImport.test_dotted_name_import: TestParseSimpleImport#test_dotted_name_import().
  TestParseSimpleImport.test_skips_import_keyword: TestParseSimpleImport#test_skips_import_keyword().
  TestParseSimpleImport.test_multiple_children: TestParseSimpleImport#test_multiple_children().
  TestParseFromImport.test_from_import_with_import_list: TestParseFromImport#test_from_import_with_import_list().
  TestParseFromImport.test_from_import_with_dotted_name_as_item: TestParseFromImport#test_from_import_with_dotted_name_as_item().
  _mock_node: _mock_node().
  TestParseSimpleImport.test_skips_other_types: TestParseSimpleImport#test_skips_other_types().
  TestParseFromImport.test_from_import_no_module: TestParseFromImport#test_from_import_no_module().
  TestImportNodeContext.test_node_without_start_byte: TestImportNodeContext#test_node_without_start_byte().
  TestImportNodeContext: TestImportNodeContext#
  TestParseSimpleImport: TestParseSimpleImport#
  TestParseFromImport: TestParseFromImport#
  TestQueryClassBodyNodes: TestQueryClassBodyNodes#
  TestExtractImportsFromTree: TestExtractImportsFromTree#
---
# Module: [`tests/unit/languages/test_python_import_helpers_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py)

## Classes
### `TestExtractImportsFromTree`
- def: [`tests/unit/languages/test_python_import_helpers_coverage.py:183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L183)
- signature: `class TestExtractImportsFromTree:`
- members:
  - `test_no_language_returns_empty(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L184)
  - `test_query_returns_empty_on_bad_language(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L198)
- uses (calls/refs, reference-scoped): [`extract_imports_from_tree`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#extract_imports_from_tree), [`ImportExtractionRuntime`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime), [`tree`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime.tree), [`extract_imports_manual`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime.extract_imports_manual), [`source_code`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime.source_code), [`extract_import_info`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime.extract_import_info), [`import_query`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime.import_query), [`log_debug_fn`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime.log_debug_fn), [`log_warning_fn`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportExtractionRuntime.log_warning_fn)

### `TestImportNodeContext`
- def: [`tests/unit/languages/test_python_import_helpers_coverage.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L48)
- signature: `class TestImportNodeContext:`
- members:
  - `test_creates_context(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L49)
  - `test_node_without_start_byte(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L56)
- uses (calls/refs, reference-scoped): [`import_node_context`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#import_node_context), [`raw_text`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportNodeContext.raw_text), [`end_line`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportNodeContext.end_line), [`start_line`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportNodeContext.start_line)  (1 test-only)

### `TestParseFromImport`
- def: [`tests/unit/languages/test_python_import_helpers_coverage.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L118)
- signature: `class TestParseFromImport:`
- members:
  - `test_from_import_no_module(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L136)
  - `test_from_import_with_dotted_name_as_item(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L144)
  - `test_from_import_with_import_list(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L119)
- uses (calls/refs, reference-scoped): [`parse_from_import`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#parse_from_import), [`ImportNodeContext`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportNodeContext)  (2 test-only)

### `TestParseSimpleImport`
- def: [`tests/unit/languages/test_python_import_helpers_coverage.py:64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L64)
- signature: `class TestParseSimpleImport:`
- members:
  - `test_dotted_name_import(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L75)
  - `test_multiple_children(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L104)
  - `test_single_import(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L65)
  - `test_skips_import_keyword(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L85)
  - `test_skips_other_types(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L94)
- uses (calls/refs, reference-scoped): [`parse_simple_import`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#parse_simple_import), [`ImportNodeContext`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ImportNodeContext)  (2 test-only)

### `TestQueryClassBodyNodes`
- def: [`tests/unit/languages/test_python_import_helpers_coverage.py:157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L157)
- signature: `class TestQueryClassBodyNodes:`
- members:
  - `test_no_language_returns_empty(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L158)
  - `test_query_exception_returns_empty(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L169)
- uses (calls/refs, reference-scoped): [`query_class_body_nodes`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#query_class_body_nodes), [`ClassBodyQueryRuntime`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ClassBodyQueryRuntime), [`tree`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ClassBodyQueryRuntime.tree), [`class_query`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ClassBodyQueryRuntime.class_query), [`log_debug_fn`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ClassBodyQueryRuntime.log_debug_fn), [`log_warning_fn`](../../../tree_sitter_analyzer/languages/python_plugin/_import_helpers.md#ClassBodyQueryRuntime.log_warning_fn)

## Functions
- `_child_from_source(source_code: str, text: str, node_type="identifier")` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L36)
- `_mock_node(source_code: str, node_type="import_statement", start_point=(0, 0), end_point=None, children=None)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_import_helpers_coverage.py#L17)

