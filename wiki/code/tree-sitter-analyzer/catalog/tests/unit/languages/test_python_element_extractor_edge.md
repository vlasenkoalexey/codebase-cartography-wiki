---
title: 'Module: tests/unit/languages/test_python_element_extractor_edge.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_element_extractor_edge.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_element_extractor_edge`/TestPythonElementExtractor#
symbols:
  TestPythonElementExtractor.test_traverse_and_extract_iterative: test_traverse_and_extract_iterative().
  TestPythonElementExtractor.mock_extract_function: mock_extract_function().
  TestPythonElementExtractor.test_traverse_and_extract_iterative_with_caching: test_traverse_and_extract_iterative_with_caching().
  TestPythonElementExtractor.extractor: extractor().
  TestPythonElementExtractor.test_performance_with_large_codebase: test_performance_with_large_codebase().
  TestPythonElementExtractor.test_concurrent_extraction: test_concurrent_extraction().
  TestPythonElementExtractor.extract_worker: extract_worker().
  TestPythonElementExtractor: ''
  TestPythonElementExtractor.mock_tree: mock_tree().
  TestPythonElementExtractor.sample_python_code: sample_python_code().
  TestPythonElementExtractor.test_traverse_and_extract_iterative_max_depth: test_traverse_and_extract_iterative_max_depth().
  TestPythonElementExtractor.test_memory_usage_with_caching: test_memory_usage_with_caching().
  TestPythonElementExtractor.test_error_handling_in_extraction: test_error_handling_in_extraction().
  TestPythonElementExtractor.test_unicode_handling: test_unicode_handling().
---
# Module: [`tests/unit/languages/test_python_element_extractor_edge.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py)

## Classes
### `TestPythonElementExtractor`
- def: [`tests/unit/languages/test_python_element_extractor_edge.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L12)
- doc: Test Python element extractor functionality
- signature: `class TestPythonElementExtractor:`
- members:
  - `extract_worker()` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L348)
  - `extractor(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L16) — Create a Python element extractor instance
  - `mock_extract_function(node)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L233)
  - `mock_tree(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L21) — Create a mock tree-sitter tree
  - `sample_python_code(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L29) — Sample Python code for testing
  - `test_concurrent_extraction(self, extractor)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L337) — Test concurrent extraction operations
  - `test_error_handling_in_extraction(self, extractor)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L290) — Test error handling during extraction
  - `test_memory_usage_with_caching(self, extractor)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L253) — Test memory usage with caching
  - `test_performance_with_large_codebase(self, extractor)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L209) — Test performance with large codebase simulation
  - `test_traverse_and_extract_iterative(self, extractor)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L91) — Test iterative traversal and extraction
  - `test_traverse_and_extract_iterative_max_depth(self, extractor)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L172) — Test max depth protection in traversal
  - `test_traverse_and_extract_iterative_with_caching(self, extractor)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L138) — Test iterative traversal with caching
  - `test_unicode_handling(self, extractor)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_edge.py#L307) — Test Unicode character handling
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor)

