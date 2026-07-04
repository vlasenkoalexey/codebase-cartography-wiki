---
title: 'Module: tests/unit/languages/test_python_element_extractor_core.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_element_extractor_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_element_extractor_core`/TestPythonElementExtractor#
symbols:
  TestPythonElementExtractor.extractor: extractor().
  TestPythonElementExtractor.test_calculate_complexity_optimized: test_calculate_complexity_optimized().
  TestPythonElementExtractor._func_node: _func_node().
  TestPythonElementExtractor: ''
  TestPythonElementExtractor.mock_tree: mock_tree().
  TestPythonElementExtractor.sample_python_code: sample_python_code().
  TestPythonElementExtractor.test_initialization: test_initialization().
  TestPythonElementExtractor.test_reset_caches: test_reset_caches().
  TestPythonElementExtractor.test_detect_file_characteristics: test_detect_file_characteristics().
  TestPythonElementExtractor.test_extract_functions_basic: test_extract_functions_basic().
  TestPythonElementExtractor.test_extract_classes_basic: test_extract_classes_basic().
  TestPythonElementExtractor.test_extract_variables_basic: test_extract_variables_basic().
  TestPythonElementExtractor.test_get_node_text_optimized_caching: test_get_node_text_optimized_caching().
  TestPythonElementExtractor.test_get_node_text_optimized_fallback: test_get_node_text_optimized_fallback().
  TestPythonElementExtractor.test_parse_function_signature_optimized: test_parse_function_signature_optimized().
  TestPythonElementExtractor.test_parse_function_signature_async: test_parse_function_signature_async().
  TestPythonElementExtractor.test_extract_parameters_from_node_optimized: test_extract_parameters_from_node_optimized().
  TestPythonElementExtractor.test_extract_docstring_for_line_single_line: test_extract_docstring_for_line_single_line().
  TestPythonElementExtractor.test_extract_docstring_for_line_multi_line: test_extract_docstring_for_line_multi_line().
  TestPythonElementExtractor.test_extract_docstring_for_line_caching: test_extract_docstring_for_line_caching().
---
# Module: [`tests/unit/languages/test_python_element_extractor_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py)

## Classes
### `TestPythonElementExtractor`
- def: [`tests/unit/languages/test_python_element_extractor_core.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L10)
- doc: Test Python element extractor functionality
- signature: `class TestPythonElementExtractor:`
- members:
  - `extractor(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L14) — Create a Python element extractor instance
  - `mock_tree(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L19) — Create a mock tree-sitter tree
  - `sample_python_code(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L27) — Sample Python code for testing
  - `test_calculate_complexity_optimized(self, extractor)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L428) — Complexity is an AST-node walk over a real parse, not a text count.
  - `test_detect_file_characteristics(self, extractor, sample_python_code)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L126) — Test file characteristics detection
  - `test_extract_classes_basic(self, extractor, mock_tree, sample_python_code)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L176) — Test basic class extraction
  - `test_extract_docstring_for_line_caching(self, extractor)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L411) — Test docstring extraction caching
  - `test_extract_docstring_for_line_multi_line(self, extractor)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L396) — Test multi-line docstring extraction
  - `test_extract_docstring_for_line_single_line(self, extractor)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L385) — Test single-line docstring extraction
  - `test_extract_functions_basic(self, extractor, mock_tree, sample_python_code)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L152) — Test basic function extraction
  - `test_extract_parameters_from_node_optimized(self, extractor)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L337) — Test parameter extraction from node
  - `test_extract_variables_basic(self, extractor, mock_tree, sample_python_code)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L200) — Test basic variable extraction
  - `test_get_node_text_optimized_caching(self, extractor)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L214) — Test node text extraction with caching
  - `test_get_node_text_optimized_fallback(self, extractor)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L245) — Test node text extraction fallback mechanism
  - `test_initialization(self, extractor)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L89) — Test extractor initialization
  - `test_parse_function_signature_async(self, extractor)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L309) — Test async function signature parsing
  - `test_parse_function_signature_optimized(self, extractor)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L268) — Test function signature parsing
  - `test_reset_caches(self, extractor)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L107) — Test cache reset functionality
- protocol/private: `_func_node`[`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_element_extractor_core.py#L433)
- uses (calls/refs, reference-scoped): [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor)

