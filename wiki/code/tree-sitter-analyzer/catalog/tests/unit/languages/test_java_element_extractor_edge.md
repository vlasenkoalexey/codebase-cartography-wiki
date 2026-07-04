---
title: 'Module: tests/unit/languages/test_java_element_extractor_edge.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_element_extractor_edge.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_element_extractor_edge`/TestJavaElementExtractor#
symbols:
  TestJavaElementExtractor.mock_extract_method: mock_extract_method().
  TestJavaElementExtractor.extractor: extractor().
  TestJavaElementExtractor.test_performance_with_large_codebase: test_performance_with_large_codebase().
  TestJavaElementExtractor: ''
  TestJavaElementExtractor.mock_tree: mock_tree().
  TestJavaElementExtractor.sample_java_code: sample_java_code().
  TestJavaElementExtractor.test_extract_imports_fallback_static_imports: test_extract_imports_fallback_static_imports().
  TestJavaElementExtractor.test_extract_imports_fallback_normal_imports: test_extract_imports_fallback_normal_imports().
  TestJavaElementExtractor.test_memory_usage_with_caching: test_memory_usage_with_caching().
  TestJavaElementExtractor.test_error_handling_in_extraction: test_error_handling_in_extraction().
  TestJavaElementExtractor.test_extract_class_optimized_error_handling: test_extract_class_optimized_error_handling().
  TestJavaElementExtractor.test_extract_class_optimized_with_exception: test_extract_class_optimized_with_exception().
  TestJavaElementExtractor.test_extract_method_optimized_error_handling: test_extract_method_optimized_error_handling().
  TestJavaElementExtractor.test_extract_method_optimized_with_exception: test_extract_method_optimized_with_exception().
  TestJavaElementExtractor.test_extract_field_optimized_error_handling: test_extract_field_optimized_error_handling().
  TestJavaElementExtractor.test_extract_field_optimized_with_exception: test_extract_field_optimized_with_exception().
---
# Module: [`tests/unit/languages/test_java_element_extractor_edge.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py)

## Classes
### `TestJavaElementExtractor`
- def: [`tests/unit/languages/test_java_element_extractor_edge.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L11)
- doc: Test Java element extractor — edge cases and performance
- signature: `class TestJavaElementExtractor:`
- members:
  - `extractor(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L15) — Create a Java element extractor instance
  - `mock_extract_method(node)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L421)
  - `mock_tree(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L20) — Create a mock tree-sitter tree
  - `sample_java_code(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L28) — Sample Java code for testing
  - `test_error_handling_in_extraction(self, extractor)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L478) — Test error handling during extraction
  - `test_extract_class_optimized_error_handling(self, extractor)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L495) — Test error handling in class extraction
  - `test_extract_class_optimized_with_exception(self, extractor)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L507) — Test class extraction when an exception occurs
  - `test_extract_field_optimized_error_handling(self, extractor)` — [`L548`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L548) — Test error handling in field extraction
  - `test_extract_field_optimized_with_exception(self, extractor)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L564) — Test field extraction when an exception occurs
  - `test_extract_imports_fallback_normal_imports(self, extractor)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L369) — Test fallback import extraction for normal imports
  - `test_extract_imports_fallback_static_imports(self, extractor)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L344) — Test fallback import extraction for static imports
  - `test_extract_method_optimized_error_handling(self, extractor)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L521) — Test error handling in method extraction
  - `test_extract_method_optimized_with_exception(self, extractor)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L535) — Test method extraction when an exception occurs
  - `test_memory_usage_with_caching(self, extractor)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L441) — Test memory usage with caching
  - `test_performance_with_large_codebase(self, extractor)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_edge.py#L394) — Test performance with large codebase simulation
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor)

