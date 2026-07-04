---
title: 'Module: tests/unit/languages/test_rust_plugin_integration.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_rust_plugin_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_rust_plugin_integration`/
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
# Module: [`tests/unit/languages/test_rust_plugin_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py)

## Classes
### `TestRustIntegration`
- def: [`tests/unit/languages/test_rust_plugin_integration.py:160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L160)
- signature: `class TestRustIntegration:`
- members:
  - `test_async_function_detection(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L297)
  - `test_enum_trait_extraction(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L220)
  - `test_extract_elements_full(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L344) — Test extract_elements directly with parsed tree.
  - `test_field_extraction(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L275)
  - `test_full_flow(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L162)
  - `test_impl_block_extraction(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L253)
  - `test_import_extraction(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L200)
  - `test_visibility_extraction(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L317)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`analyze_file`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustPlugin.analyze_file), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async), [`RustPlugin`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustPlugin), [`extract_elements`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustPlugin.extract_elements), [`modules`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.modules)  (2 test-only)

### `TestRustPlugin`
- def: [`tests/unit/languages/test_rust_plugin_integration.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L22)
- signature: `class TestRustPlugin:`
- members:
  - `test_analyze_file_exception(self, mock_log, rust_plugin)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L100)
  - `test_analyze_file_integration(self, mock_parser_cls, rust_plugin)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L114)
  - `test_analyze_file_no_language(self, rust_plugin)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L86)
  - `test_count_tree_nodes_none(self, rust_plugin)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L23)
  - `test_count_tree_nodes_with_children(self, rust_plugin)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L26)
  - `test_extract_elements_error(self, mock_log, rust_plugin)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L75)
  - `test_extract_elements_none_tree(self, rust_plugin)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L70)
  - `test_get_tree_sitter_language_cached(self, rust_plugin)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L38)
  - `test_get_tree_sitter_language_exception(self, mock_log, rust_plugin)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L50)
  - `test_get_tree_sitter_language_import_error(self, rust_plugin)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L43)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success)

## Functions
- `_parse_rust(code: str)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L146) — Parse Rust code with tree-sitter-rust. Returns tree or None.
- `rust_extractor()` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L18)
- `rust_plugin()` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L13)

## Module values
- `_TS_RUST_AVAILABLE` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_plugin_integration.py#L137)

