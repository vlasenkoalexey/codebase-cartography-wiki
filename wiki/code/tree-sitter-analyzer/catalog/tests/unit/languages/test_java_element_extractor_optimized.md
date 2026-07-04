---
title: 'Module: tests/unit/languages/test_java_element_extractor_optimized.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_element_extractor_optimized.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_element_extractor_optimized`/
symbols:
  _assert_method_extracted: _assert_method_extracted().
  _assert_class_extracted: _assert_class_extracted().
  _assert_field_extracted: _assert_field_extracted().
  TestJavaElementExtractor.test_extract_method_optimized_constructor: TestJavaElementExtractor#test_extract_method_optimized_constructor().
  TestJavaElementExtractor.test_extract_field_optimized_multiple_variables: TestJavaElementExtractor#test_extract_field_optimized_multiple_variables().
  TestJavaElementExtractor.test_extract_class_optimized_complete: TestJavaElementExtractor#test_extract_class_optimized_complete().
  TestJavaElementExtractor.extractor: TestJavaElementExtractor#extractor().
  TestJavaElementExtractor.test_extract_method_optimized_complete: TestJavaElementExtractor#test_extract_method_optimized_complete().
  TestJavaElementExtractor.test_extract_field_optimized_complete: TestJavaElementExtractor#test_extract_field_optimized_complete().
  _build_class_mock_node: _build_class_mock_node().
  TestJavaElementExtractor: TestJavaElementExtractor#
  TestJavaElementExtractor.mock_tree: TestJavaElementExtractor#mock_tree().
  TestJavaElementExtractor.sample_java_code: TestJavaElementExtractor#sample_java_code().
---
# Module: [`tests/unit/languages/test_java_element_extractor_optimized.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py)

## Classes
### `TestJavaElementExtractor`
- def: [`tests/unit/languages/test_java_element_extractor_optimized.py:107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L107)
- doc: Test Java element extractor — optimized extraction
- signature: `class TestJavaElementExtractor:`
- members:
  - `extractor(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L111) — Create a Java element extractor instance
  - `mock_tree(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L116) — Create a mock tree-sitter tree
  - `sample_java_code(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L124) — Sample Java code for testing
  - `test_extract_class_optimized_complete(self, extractor)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L440) — Test complete class extraction
  - `test_extract_field_optimized_complete(self, extractor)` — [`L583`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L583) — Test complete field extraction
  - `test_extract_field_optimized_multiple_variables(self, extractor)` — [`L625`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L625) — Test field extraction with multiple variables in one declaration
  - `test_extract_method_optimized_complete(self, extractor)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L481) — Test complete method extraction
  - `test_extract_method_optimized_constructor(self, extractor)` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L533) — Test constructor extraction
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`variable_type`](../../../tree_sitter_analyzer/models/base.md#Variable.variable_type), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Variable.visibility), [`is_constructor`](../../../tree_sitter_analyzer/models/base.md#Function.is_constructor), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Variable.modifiers)  (4 test-only)

## Functions
- `_assert_class_extracted(result)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L42) — Assert _extract_class_optimized result for the UserService fixture.
- `_assert_field_extracted(result)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L86) — Assert _extract_field_optimized result for the userRepository fixture.
- `_assert_method_extracted(result)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L61) — Assert _extract_method_optimized result for the findById fixture.
- `_build_class_mock_node()` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_element_extractor_optimized.py#L12) — Build a mock class_declaration AST node for extraction tests.

