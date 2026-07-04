---
title: 'Module: tests/unit/languages/test_java_element_extractor_traverse.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_element_extractor_traverse.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_element_extractor_traverse`/TestJavaElementExtractorTraverse#
symbols:
  TestJavaElementExtractorTraverse.test_traverse_and_extract_iterative: test_traverse_and_extract_iterative().
  TestJavaElementExtractorTraverse.mock_field_extractor: mock_field_extractor().
  TestJavaElementExtractorTraverse.test_traverse_and_extract_iterative_with_caching: test_traverse_and_extract_iterative_with_caching().
  TestJavaElementExtractorTraverse.test_process_field_batch_with_caching: test_process_field_batch_with_caching().
  TestJavaElementExtractorTraverse.extractor: extractor().
  TestJavaElementExtractorTraverse.test_traverse_and_extract_iterative_field_batching: test_traverse_and_extract_iterative_field_batching().
  TestJavaElementExtractorTraverse.test_process_field_batch: test_process_field_batch().
  TestJavaElementExtractorTraverse: ''
  TestJavaElementExtractorTraverse.test_traverse_and_extract_iterative_max_depth: test_traverse_and_extract_iterative_max_depth().
---
# Module: [`tests/unit/languages/test_java_element_extractor_traverse.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py)

## Classes
### `TestJavaElementExtractorTraverse`
- def: [`tests/unit/languages/test_java_element_extractor_traverse.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L11)
- doc: Test Java element extractor traverse and batch processing.
- signature: `class TestJavaElementExtractorTraverse:`
- members:
  - `extractor(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L15)
  - `mock_field_extractor(node)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L106)
  - `test_process_field_batch(self, extractor)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L126) — Test field batch processing
  - `test_process_field_batch_with_caching(self, extractor)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L153) — Test field batch processing with caching
  - `test_traverse_and_extract_iterative(self, extractor)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L18) — Test iterative traversal and extraction
  - `test_traverse_and_extract_iterative_field_batching(self, extractor)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L93) — Test field batching in iterative traversal
  - `test_traverse_and_extract_iterative_max_depth(self, extractor)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L181) — Test max depth protection in traversal
  - `test_traverse_and_extract_iterative_with_caching(self, extractor)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_traverse.py#L63) — Test iterative traversal with caching
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor)

