---
title: 'Module: tests/unit/languages/test_yaml_plugin_features.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_plugin_features.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_plugin_features`/
symbols:
  get_tree_for_code: get_tree_for_code().
  SCALAR_TYPES_CODE: SCALAR_TYPES_CODE.
  TestYAMLComplexStructures.test_extract_services_structure: TestYAMLComplexStructures#test_extract_services_structure().
  TestYAMLComplexStructures.test_extract_volumes: TestYAMLComplexStructures#test_extract_volumes().
  TestYAMLComplexStructures.test_extract_networks: TestYAMLComplexStructures#test_extract_networks().
  TestYAMLScalarTypes.test_extract_string_scalar: TestYAMLScalarTypes#test_extract_string_scalar().
  TestYAMLScalarTypes.test_extract_integer_scalar: TestYAMLScalarTypes#test_extract_integer_scalar().
  TestYAMLScalarTypes.test_extract_float_scalar: TestYAMLScalarTypes#test_extract_float_scalar().
  TestYAMLScalarTypes.test_extract_null_scalar: TestYAMLScalarTypes#test_extract_null_scalar().
  TestYAMLScalarTypes.test_extract_scientific_notation: TestYAMLScalarTypes#test_extract_scientific_notation().
  TestYAMLScalarTypes.test_extract_hexadecimal: TestYAMLScalarTypes#test_extract_hexadecimal().
  TestYAMLScalarTypes.test_extract_timestamp: TestYAMLScalarTypes#test_extract_timestamp().
  TestYAMLQueryAccuracy.test_key_value_query_accuracy: TestYAMLQueryAccuracy#test_key_value_query_accuracy().
  TestYAMLQueryAccuracy.test_no_false_positives: TestYAMLQueryAccuracy#test_no_false_positives().
  TestYAMLQueryAccuracy.test_line_number_accuracy: TestYAMLQueryAccuracy#test_line_number_accuracy().
  TestYAMLQueryAccuracy.test_value_type_accuracy: TestYAMLQueryAccuracy#test_value_type_accuracy().
  TestYAMLComplexStructures.test_extract_nested_services: TestYAMLComplexStructures#test_extract_nested_services().
  TestYAMLComplexStructures.test_extract_environment_variables: TestYAMLComplexStructures#test_extract_environment_variables().
  TestYAMLMultiDocument.test_extract_multiple_documents: TestYAMLMultiDocument#test_extract_multiple_documents().
  TestYAMLMultiDocument.test_document_indices: TestYAMLMultiDocument#test_document_indices().
  TestYAMLScalarTypes.test_extract_boolean_scalar: TestYAMLScalarTypes#test_extract_boolean_scalar().
  TestYAMLCommentRecognition.test_extract_comment: TestYAMLCommentRecognition#test_extract_comment().
  TestYAMLCommentRecognition.test_extract_inline_comment: TestYAMLCommentRecognition#test_extract_inline_comment().
  TestYAMLCommentRecognition.test_extract_block_comment: TestYAMLCommentRecognition#test_extract_block_comment().
  TestYAMLQueryAccuracy.test_list_query_accuracy: TestYAMLQueryAccuracy#test_list_query_accuracy().
  TestYAMLQueryAccuracy.test_nested_structure_query_accuracy: TestYAMLQueryAccuracy#test_nested_structure_query_accuracy().
  TestYAMLQueryAccuracy.test_anchor_alias_query_accuracy: TestYAMLQueryAccuracy#test_anchor_alias_query_accuracy().
  TestYAMLQueryAccuracy.test_multi_document_query_accuracy: TestYAMLQueryAccuracy#test_multi_document_query_accuracy().
  TestYAMLQueryAccuracy.test_scalar_type_query_accuracy: TestYAMLQueryAccuracy#test_scalar_type_query_accuracy().
  TestYAMLQueryAccuracy.test_no_false_negatives: TestYAMLQueryAccuracy#test_no_false_negatives().
  TestYAMLComplexStructures.test_extract_complex_structure: TestYAMLComplexStructures#test_extract_complex_structure().
  TestYAMLMultiDocument.test_extract_document_content: TestYAMLMultiDocument#test_extract_document_content().
  COMPLEX_YAML_CODE: COMPLEX_YAML_CODE.
  KEY_VALUE_CODE: KEY_VALUE_CODE.
  MULTI_DOCUMENT_CODE: MULTI_DOCUMENT_CODE.
  COMMENT_CODE: COMMENT_CODE.
  TestYAMLComplexStructures: TestYAMLComplexStructures#
  TestYAMLMultiDocument: TestYAMLMultiDocument#
  TestYAMLScalarTypes: TestYAMLScalarTypes#
  TestYAMLCommentRecognition: TestYAMLCommentRecognition#
  TestYAMLQueryAccuracy: TestYAMLQueryAccuracy#
  LIST_CODE: LIST_CODE.
  NESTED_STRUCTURE_CODE: NESTED_STRUCTURE_CODE.
  ANCHOR_ALIAS_CODE: ANCHOR_ALIAS_CODE.
---
# Module: [`tests/unit/languages/test_yaml_plugin_features.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py)

## Classes
### `TestYAMLCommentRecognition`
- def: [`tests/unit/languages/test_yaml_plugin_features.py:446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L446)
- doc: Test YAML comment recognition and extraction.
- signature: `class TestYAMLCommentRecognition:`
- members:
  - `test_extract_block_comment(self)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L467) — Test extraction of block comment.
  - `test_extract_comment(self)` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L449) — Test extraction of comment.
  - `test_extract_inline_comment(self)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L458) — Test extraction of inline comment.
- uses (calls/refs, reference-scoped): [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor)  (2 test-only)

### `TestYAMLComplexStructures`
- def: [`tests/unit/languages/test_yaml_plugin_features.py:266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L266)
- doc: Test extraction of complex YAML structures.
- signature: `class TestYAMLComplexStructures:`
- members:
  - `test_extract_complex_structure(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L269) — Test extraction of complex YAML structure.
  - `test_extract_environment_variables(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L298) — Test extraction of environment variables.
  - `test_extract_nested_services(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L287) — Test extraction of nested services.
  - `test_extract_networks(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L317) — Test extraction of networks.
  - `test_extract_services_structure(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L277) — Test extraction of services structure.
  - `test_extract_volumes(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L307) — Test extraction of volumes.
- uses (calls/refs, reference-scoped): [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key)  (2 test-only)

### `TestYAMLMultiDocument`
- def: [`tests/unit/languages/test_yaml_plugin_features.py:329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L329)
- doc: Test YAML multi-document recognition and extraction.
- signature: `class TestYAMLMultiDocument:`
- members:
  - `test_document_indices(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L349) — Test that document indices are captured.
  - `test_extract_document_content(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L341) — Test extraction of document content.
  - `test_extract_multiple_documents(self)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L332) — Test extraction of multiple documents.
- uses (calls/refs, reference-scoped): [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`document_index`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.document_index)  (2 test-only)

### `TestYAMLQueryAccuracy`
- def: [`tests/unit/languages/test_yaml_plugin_features.py:478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L478)
- doc: Test accuracy of YAML queries.
- signature: `class TestYAMLQueryAccuracy:`
- members:
  - `test_anchor_alias_query_accuracy(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L508) — Test that anchor/alias query is accurate.
  - `test_key_value_query_accuracy(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L481) — Test that key-value query accurately identifies pairs.
  - `test_line_number_accuracy(self)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L560) — Test that line numbers are accurate.
  - `test_list_query_accuracy(self)` — [`L490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L490) — Test that list query accurately identifies lists.
  - `test_multi_document_query_accuracy(self)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L519) — Test that multi-document query is accurate.
  - `test_nested_structure_query_accuracy(self)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L499) — Test that nested structure query is accurate.
  - `test_no_false_negatives(self)` — [`L549`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L549) — Test that queries don't miss elements.
  - `test_no_false_positives(self)` — [`L538`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L538) — Test that queries don't produce false positives.
  - `test_scalar_type_query_accuracy(self)` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L528) — Test that scalar type query is accurate.
  - `test_value_type_accuracy(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L569) — Test that value types are accurately identified.
- uses (calls/refs, reference-scoped): [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key), [`value_type`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value_type), [`nesting_level`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.nesting_level)  (7 test-only)

### `TestYAMLScalarTypes`
- def: [`tests/unit/languages/test_yaml_plugin_features.py:360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L360)
- doc: Test YAML scalar type recognition and extraction.
- signature: `class TestYAMLScalarTypes:`
- members:
  - `test_extract_boolean_scalar(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L393) — Test extraction of boolean scalar.
  - `test_extract_float_scalar(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L383) — Test extraction of float scalar.
  - `test_extract_hexadecimal(self)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L424) — Test extraction of hexadecimal value.
  - `test_extract_integer_scalar(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L373) — Test extraction of integer scalar.
  - `test_extract_null_scalar(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L404) — Test extraction of null scalar.
  - `test_extract_scientific_notation(self)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L414) — Test extraction of scientific notation.
  - `test_extract_string_scalar(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L363) — Test extraction of string scalar.
  - `test_extract_timestamp(self)` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L434) — Test extraction of timestamp value.
- uses (calls/refs, reference-scoped): [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`extract_yaml_elements`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_yaml_elements), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`extractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.extractor), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key), [`value_type`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value_type), [`value`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value)  (2 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: YAMLPlugin)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L250) — Helper to parse YAML code and return tree.

## Module values
- `ANCHOR_ALIAS_CODE` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L99)
- `COMMENT_CODE` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L226)
- `COMPLEX_YAML_CODE` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L139)
- `KEY_VALUE_CODE` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L10)
- `LIST_CODE` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L34)
- `MULTI_DOCUMENT_CODE` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L184)
- `NESTED_STRUCTURE_CODE` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L68)
- `SCALAR_TYPES_CODE` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin_features.py#L196)

