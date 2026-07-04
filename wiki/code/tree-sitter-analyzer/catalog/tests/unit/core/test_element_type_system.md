---
title: 'Module: tests/unit/core/test_element_type_system.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_element_type_system.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_element_type_system`/
symbols:
  TestElementTypeSystem.test_get_element_type_with_class_name: TestElementTypeSystem#test_get_element_type_with_class_name().
  MockElement.element_type: MockElement#element_type.
  TestElementTypeSystem.test_element_type_constants: TestElementTypeSystem#test_element_type_constants().
  TestCLIElementTypeConsistency.test_consistency_between_advanced_and_table: TestCLIElementTypeConsistency#test_consistency_between_advanced_and_table().
  _run_cli: _run_cli().
  TestCLIElementTypeConsistency.test_advanced_command_element_counts: TestCLIElementTypeConsistency#test_advanced_command_element_counts().
  TestCLIElementTypeConsistency.test_table_command_element_counts: TestCLIElementTypeConsistency#test_table_command_element_counts().
  TestElementTypeRegression.test_zero_element_counts_detection: TestElementTypeRegression#test_zero_element_counts_detection().
  _parse_table_class_info_counts: _parse_table_class_info_counts().
  _advanced_args: _advanced_args().
  _parse_advanced_counts: _parse_advanced_counts().
  _table_args: _table_args().
  _capture_table_count: _capture_table_count().
  TestElementTypeSystem.test_get_element_type_with_element_type_attribute.MockElement: TestElementTypeSystem#test_get_element_type_with_element_type_attribute().MockElement#
  TestElementTypeSystem.test_get_element_type_with_class_name.Class: TestElementTypeSystem#test_get_element_type_with_class_name().Class#
  TestElementTypeSystem.test_get_element_type_with_class_name.Function: TestElementTypeSystem#test_get_element_type_with_class_name().Function#
  TestElementTypeSystem.test_get_element_type_with_class_name.Variable: TestElementTypeSystem#test_get_element_type_with_class_name().Variable#
  TestElementTypeSystem.test_is_element_of_type.MockElement: TestElementTypeSystem#test_is_element_of_type().MockElement#
  TestElementTypeSystem: TestElementTypeSystem#
  TestElementTypeSystem.test_get_element_type_with_element_type_attribute: TestElementTypeSystem#test_get_element_type_with_element_type_attribute().
  TestElementTypeSystem.test_get_element_type_with_element_type_attribute.MockElement.__init__: TestElementTypeSystem#test_get_element_type_with_element_type_attribute().MockElement#__init__().
  TestElementTypeSystem.test_is_element_of_type: TestElementTypeSystem#test_is_element_of_type().
  TestElementTypeSystem.test_is_element_of_type.MockElement.__init__: TestElementTypeSystem#test_is_element_of_type().MockElement#__init__().
  TestCLIElementTypeConsistency: TestCLIElementTypeConsistency#
  TestCLIElementTypeConsistency.sample_java_file: TestCLIElementTypeConsistency#sample_java_file().
  TestElementTypeRegression: TestElementTypeRegression#
---
# Module: [`tests/unit/core/test_element_type_system.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py)

## Classes
### `Class`
- def: [`tests/unit/core/test_element_type_system.py:148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L148)
- signature: `class Class:`
- used by: (1 test-only callers)

### `Function`
- def: [`tests/unit/core/test_element_type_system.py:151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L151)
- signature: `class Function:`
- used by: (1 test-only callers)

### `MockElement`
- def: [`tests/unit/core/test_element_type_system.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L164)
- signature: `class MockElement:`
- members:
  - `element_type` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L137)
- protocol/private: `__init__`[`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L136), `__init__`[`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L165)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`is_element_of_type`](../../../tree_sitter_analyzer/constants.md#is_element_of_type), [`get_element_type`](../../../tree_sitter_analyzer/constants.md#get_element_type)  (1 test-only)

### `TestCLIElementTypeConsistency`
- def: [`tests/unit/core/test_element_type_system.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L173)
- doc: Test CLI commands use correct element type system
- signature: `class TestCLIElementTypeConsistency:`
- members:
  - `sample_java_file(self, tmp_path)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L177) — Create a sample Java file for testing
  - `test_advanced_command_element_counts(self, monkeypatch, sample_java_file)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L205) — Test that advanced command shows correct element counts
  - `test_consistency_between_advanced_and_table(self, monkeypatch, sample_java_file)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L237) — Test that advanced and table commands show consistent results
  - `test_table_command_element_counts(self, monkeypatch, sample_java_file)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L224) — Test that table command shows correct element counts
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestElementTypeRegression`
- def: [`tests/unit/core/test_element_type_system.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L257)
- doc: Test to prevent regression in element type system
- signature: `class TestElementTypeRegression:`
- members:
  - `test_zero_element_counts_detection(self, monkeypatch, tmp_path)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L260) — Test that zero element counts are detected and flagged
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestElementTypeSystem`
- def: [`tests/unit/core/test_element_type_system.py:121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L121)
- doc: Test the unified element type system
- signature: `class TestElementTypeSystem:`
- members:
  - `test_element_type_constants(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L124) — Test that element type constants are correctly defined
  - `test_get_element_type_with_class_name(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L145) — Test get_element_type with __class__.__name__ fallback
  - `test_get_element_type_with_element_type_attribute(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L132) — Test get_element_type with element_type attribute
  - `test_is_element_of_type(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L161) — Test is_element_of_type function
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE), [`ELEMENT_TYPE_IMPORT`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_IMPORT), [`get_element_type`](../../../tree_sitter_analyzer/constants.md#get_element_type), [`ELEMENT_TYPE_PACKAGE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_PACKAGE)  (3 test-only)

### `Variable`
- def: [`tests/unit/core/test_element_type_system.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L154)
- signature: `class Variable:`
- used by: (1 test-only callers)

## Functions
- `_advanced_args(sample_java_file: str)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L28)
- `_capture_table_count(table_counts: dict[str, int], line: str, label: str, key: str)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L106)
- `_parse_advanced_counts(output: str)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L64)
- `_parse_table_class_info_counts(output: str)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L85)
- `_run_cli(monkeypatch: pytest.MonkeyPatch, argv: list[str])` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L53)
- `_table_args(sample_java_file: str)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_element_type_system.py#L41)

