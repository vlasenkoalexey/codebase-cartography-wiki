---
title: 'Module: tests/unit/languages/test_typescript_extractor_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_extractor_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_extractor_comprehensive`/TestTypeScriptElementExtractorComprehensive#
symbols:
  TestTypeScriptElementExtractorComprehensive.extractor: extractor().
  TestTypeScriptElementExtractorComprehensive: ''
  TestTypeScriptElementExtractorComprehensive.mock_node: mock_node().
  TestTypeScriptElementExtractorComprehensive.test_get_node_text_optimized_cached: test_get_node_text_optimized_cached().
  TestTypeScriptElementExtractorComprehensive.test_get_node_text_optimized_fallback: test_get_node_text_optimized_fallback().
  TestTypeScriptElementExtractorComprehensive.test_get_node_text_optimized_error_handling: test_get_node_text_optimized_error_handling().
  TestTypeScriptElementExtractorComprehensive.test_parse_function_signature_optimized: test_parse_function_signature_optimized().
  TestTypeScriptElementExtractorComprehensive.test_parse_function_signature_optimized_generator: test_parse_function_signature_optimized_generator().
  TestTypeScriptElementExtractorComprehensive.test_parse_method_signature_optimized: test_parse_method_signature_optimized().
  TestTypeScriptElementExtractorComprehensive.test_parse_method_signature_optimized_constructor: test_parse_method_signature_optimized_constructor().
  TestTypeScriptElementExtractorComprehensive.test_parse_method_signature_optimized_getter_setter: test_parse_method_signature_optimized_getter_setter().
  TestTypeScriptElementExtractorComprehensive.test_extract_parameters_with_types: test_extract_parameters_with_types().
  TestTypeScriptElementExtractorComprehensive.test_extract_generics: test_extract_generics().
  TestTypeScriptElementExtractorComprehensive.test_extract_import_info_simple: test_extract_import_info_simple().
  TestTypeScriptElementExtractorComprehensive.test_extract_import_info_simple_type_import: test_extract_import_info_simple_type_import().
  TestTypeScriptElementExtractorComprehensive.test_extract_import_names: test_extract_import_names().
  TestTypeScriptElementExtractorComprehensive.test_extract_import_names_default: test_extract_import_names_default().
  TestTypeScriptElementExtractorComprehensive.test_extract_import_names_namespace: test_extract_import_names_namespace().
  TestTypeScriptElementExtractorComprehensive.test_extract_dynamic_import: test_extract_dynamic_import().
  TestTypeScriptElementExtractorComprehensive.test_extract_commonjs_requires: test_extract_commonjs_requires().
  TestTypeScriptElementExtractorComprehensive.test_extract_tsdoc_for_line: test_extract_tsdoc_for_line().
  TestTypeScriptElementExtractorComprehensive.test_extract_tsdoc_for_line_no_comment: test_extract_tsdoc_for_line_no_comment().
  TestTypeScriptElementExtractorComprehensive.test_extract_tsdoc_for_line_single_line_comment: test_extract_tsdoc_for_line_single_line_comment().
  TestTypeScriptElementExtractorComprehensive.test_traverse_and_extract_iterative_max_depth: test_traverse_and_extract_iterative_max_depth().
  TestTypeScriptElementExtractorComprehensive.test_traverse_and_extract_iterative_caching: test_traverse_and_extract_iterative_caching().
  TestTypeScriptElementExtractorComprehensive.test_traverse_and_extract_iterative_list_result: test_traverse_and_extract_iterative_list_result().
---
# Module: [`tests/unit/languages/test_typescript_extractor_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py)

## Classes
### `TestTypeScriptElementExtractorComprehensive`
- def: [`tests/unit/languages/test_typescript_extractor_comprehensive.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L17)
- doc: Comprehensive tests for TypeScriptElementExtractor
- signature: `class TestTypeScriptElementExtractorComprehensive:`
- members:
  - `extractor(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L21) — Create a TypeScriptElementExtractor instance for testing
  - `mock_node(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L26) — Create a mock tree-sitter node
  - `test_extract_commonjs_requires(self, extractor)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L501) — Test CommonJS require extraction
  - `test_extract_dynamic_import(self, extractor)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L463) — Test dynamic import extraction
  - `test_extract_generics(self, extractor)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L296) — Test generic type parameter extraction
  - `test_extract_import_info_simple(self, extractor)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L322) — Test simple import extraction
  - `test_extract_import_info_simple_type_import(self, extractor)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L357) — Test type-only import extraction
  - `test_extract_import_names(self, extractor)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L390) — Test import names extraction
  - `test_extract_import_names_default(self, extractor)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L423) — Test default import names extraction
  - `test_extract_import_names_namespace(self, extractor)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L441) — Test namespace import names extraction
  - `test_extract_parameters_with_types(self, extractor)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L252) — Test parameter extraction with types
  - `test_extract_tsdoc_for_line(self, extractor)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L553) — Test TSDoc extraction for specific line
  - `test_extract_tsdoc_for_line_no_comment(self, extractor)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L573) — Test TSDoc extraction when no comment exists
  - `test_extract_tsdoc_for_line_single_line_comment(self, extractor)` — [`L580`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L580) — Test TSDoc extraction for single line comment
  - `test_get_node_text_optimized_cached(self, extractor, mock_node)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L39) — Test node text extraction with caching
  - `test_get_node_text_optimized_error_handling(self, extractor, mock_node)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L66) — Test node text extraction error handling
  - `test_get_node_text_optimized_fallback(self, extractor, mock_node)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L54) — Test node text extraction fallback mechanism
  - `test_parse_function_signature_optimized(self, extractor)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L80) — Test function signature parsing
  - `test_parse_function_signature_optimized_generator(self, extractor)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L126) — Test generator function signature parsing
  - `test_parse_method_signature_optimized(self, extractor)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L139) — Test method signature parsing.
  - `test_parse_method_signature_optimized_constructor(self, extractor)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L217) — Test constructor method signature parsing
  - `test_parse_method_signature_optimized_getter_setter(self, extractor)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L231) — Test getter/setter method signature parsing
  - `test_traverse_and_extract_iterative_caching(self, extractor)` — [`L625`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L625) — Test iterative traversal with caching
  - `test_traverse_and_extract_iterative_list_result(self, extractor)` — [`L652`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L652) — Test iterative traversal with list result from extractor
  - `test_traverse_and_extract_iterative_max_depth(self, extractor)` — [`L593`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_extractor_comprehensive.py#L593) — Test iterative traversal with maximum depth limit
- uses (calls/refs, reference-scoped): [`TypeScriptElementExtractor`](../../../tree_sitter_analyzer/languages/typescript_plugin/extractor.md#TypeScriptElementExtractor)

