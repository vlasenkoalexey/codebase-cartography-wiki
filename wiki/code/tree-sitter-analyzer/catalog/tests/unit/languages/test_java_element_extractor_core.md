---
title: 'Module: tests/unit/languages/test_java_element_extractor_core.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_element_extractor_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_element_extractor_core`/TestJavaElementExtractor#
symbols:
  TestJavaElementExtractor.extractor: extractor().
  TestJavaElementExtractor: ''
  TestJavaElementExtractor.mock_tree: mock_tree().
  TestJavaElementExtractor.sample_java_code: sample_java_code().
  TestJavaElementExtractor.test_initialization: test_initialization().
  TestJavaElementExtractor.test_reset_caches: test_reset_caches().
  TestJavaElementExtractor.test_extract_functions_basic: test_extract_functions_basic().
  TestJavaElementExtractor.test_extract_classes_basic: test_extract_classes_basic().
  TestJavaElementExtractor.test_extract_classes_with_package_extraction: test_extract_classes_with_package_extraction().
  TestJavaElementExtractor.test_extract_variables_basic: test_extract_variables_basic().
  TestJavaElementExtractor.test_extract_imports_basic: test_extract_imports_basic().
  TestJavaElementExtractor.test_extract_imports_with_fallback: test_extract_imports_with_fallback().
  TestJavaElementExtractor.test_extract_packages_basic: test_extract_packages_basic().
  TestJavaElementExtractor.test_extract_annotations_basic: test_extract_annotations_basic().
  TestJavaElementExtractor.test_get_node_text_optimized_caching: test_get_node_text_optimized_caching().
  TestJavaElementExtractor.test_get_node_text_optimized_fallback: test_get_node_text_optimized_fallback().
---
# Module: [`tests/unit/languages/test_java_element_extractor_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py)

## Classes
### `TestJavaElementExtractor`
- def: [`tests/unit/languages/test_java_element_extractor_core.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L10)
- doc: Test Java element extractor — core functionality
- signature: `class TestJavaElementExtractor:`
- members:
  - `extractor(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L14) — Create a Java element extractor instance
  - `mock_tree(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L19) — Create a mock tree-sitter tree
  - `sample_java_code(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L27) — Sample Java code for testing
  - `test_extract_annotations_basic(self, extractor, mock_tree, sample_java_code)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L532) — Test basic annotation extraction
  - `test_extract_classes_basic(self, extractor, mock_tree, sample_java_code)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L408) — Test basic class extraction
  - `test_extract_classes_with_package_extraction(self, extractor, mock_tree, sample_java_code)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L429) — Test class extraction with automatic package extraction
  - `test_extract_functions_basic(self, extractor, mock_tree, sample_java_code)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L387) — Test basic method extraction
  - `test_extract_imports_basic(self, extractor, mock_tree, sample_java_code)` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L480) — Test basic import extraction
  - `test_extract_imports_with_fallback(self, extractor, mock_tree)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L502) — Test import extraction with regex fallback
  - `test_extract_packages_basic(self, extractor, mock_tree, sample_java_code)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L519) — Test basic package extraction
  - `test_extract_variables_basic(self, extractor, mock_tree, sample_java_code)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L459) — Test basic field extraction
  - `test_get_node_text_optimized_caching(self, extractor)` — [`L551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L551) — Test node text extraction with caching
  - `test_get_node_text_optimized_fallback(self, extractor)` — [`L582`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L582) — Test node text extraction fallback mechanism
  - `test_initialization(self, extractor)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L343) — Test extractor initialization
  - `test_reset_caches(self, extractor)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_core.py#L358) — Test cache reset functionality.
- uses (calls/refs, reference-scoped): [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor)

