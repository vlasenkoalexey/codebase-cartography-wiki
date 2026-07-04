---
title: 'Module: tests/unit/languages/test_rust_plugin_basic.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_rust_plugin_basic.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_rust_plugin_basic`/
symbols:
  TestRustIntegration.test_full_flow: TestRustIntegration#test_full_flow().
  TestRustIntegration.test_impl_block_extraction: TestRustIntegration#test_impl_block_extraction().
  TestRustIntegration.test_enum_trait_extraction: TestRustIntegration#test_enum_trait_extraction().
  TestRustIntegration.test_async_function_detection: TestRustIntegration#test_async_function_detection().
  TestRustIntegration.test_visibility_extraction: TestRustIntegration#test_visibility_extraction().
  TestRustIntegration.test_import_extraction: TestRustIntegration#test_import_extraction().
  TestRustIntegration.test_field_extraction: TestRustIntegration#test_field_extraction().
  TestRustIntegration.test_extract_elements_full: TestRustIntegration#test_extract_elements_full().
  _TS_RUST_AVAILABLE: _TS_RUST_AVAILABLE.
  TestRustPlugin.test_analyze_file_no_language: TestRustPlugin#test_analyze_file_no_language().
  TestRustPlugin.test_analyze_file_exception: TestRustPlugin#test_analyze_file_exception().
  _parse_rust: _parse_rust().
  rust_plugin: rust_plugin().
  rust_extractor: rust_extractor().
  TestRustIntegration: TestRustIntegration#
  _mock_node: _mock_node().
  TestRustPlugin: TestRustPlugin#
  TestRustPlugin.test_count_tree_nodes_none: TestRustPlugin#test_count_tree_nodes_none().
  TestRustPlugin.test_count_tree_nodes_with_children: TestRustPlugin#test_count_tree_nodes_with_children().
  TestRustPlugin.test_get_tree_sitter_language_cached: TestRustPlugin#test_get_tree_sitter_language_cached().
  TestRustPlugin.test_get_tree_sitter_language_import_error: TestRustPlugin#test_get_tree_sitter_language_import_error().
  TestRustPlugin.test_get_tree_sitter_language_exception: TestRustPlugin#test_get_tree_sitter_language_exception().
  TestRustPlugin.test_extract_elements_none_tree: TestRustPlugin#test_extract_elements_none_tree().
  TestRustPlugin.test_extract_elements_error: TestRustPlugin#test_extract_elements_error().
  TestRustPlugin.test_analyze_file_integration: TestRustPlugin#test_analyze_file_integration().
---
# Module: [`tests/unit/languages/test_rust_plugin_basic.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py)

## Classes
### `TestRustIntegration`
- def: [`tests/unit/languages/test_rust_plugin_basic.py:194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L194)
- signature: `class TestRustIntegration:`
- members:
  - `test_async_function_detection(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L331)
  - `test_enum_trait_extraction(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L254)
  - `test_extract_elements_full(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L378) — Test extract_elements directly with parsed tree.
  - `test_field_extraction(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L309)
  - `test_full_flow(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L196)
  - `test_impl_block_extraction(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L287)
  - `test_import_extraction(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L234)
  - `test_visibility_extraction(self)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L351)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`analyze_file`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustPlugin.analyze_file), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async), [`RustPlugin`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustPlugin), [`extract_elements`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustPlugin.extract_elements), [`modules`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.modules)  (2 test-only)

### `TestRustPlugin`
- def: [`tests/unit/languages/test_rust_plugin_basic.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L56)
- signature: `class TestRustPlugin:`
- members:
  - `test_analyze_file_exception(self, mock_log, rust_plugin)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L134)
  - `test_analyze_file_integration(self, mock_parser_cls, rust_plugin)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L148)
  - `test_analyze_file_no_language(self, rust_plugin)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L120)
  - `test_count_tree_nodes_none(self, rust_plugin)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L57)
  - `test_count_tree_nodes_with_children(self, rust_plugin)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L60)
  - `test_extract_elements_error(self, mock_log, rust_plugin)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L109)
  - `test_extract_elements_none_tree(self, rust_plugin)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L104)
  - `test_get_tree_sitter_language_cached(self, rust_plugin)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L72)
  - `test_get_tree_sitter_language_exception(self, mock_log, rust_plugin)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L84)
  - `test_get_tree_sitter_language_import_error(self, rust_plugin)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L77)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success)

## Functions
- `_mock_node(type_name, start_byte=0, end_byte=50, start_point=(0, 0), end_point=(0, 10), children=None, text="mock", field_children=None)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L26) — Create a mock tree-sitter Node.
- `_parse_rust(code: str)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L180) — Parse Rust code with tree-sitter-rust. Returns tree or None.
- `rust_extractor()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L22)
- `rust_plugin()` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L17)

## Module values
- `_TS_RUST_AVAILABLE` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_basic.py#L171)

