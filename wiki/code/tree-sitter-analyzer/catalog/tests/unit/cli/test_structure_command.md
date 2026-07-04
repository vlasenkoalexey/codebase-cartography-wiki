---
title: 'Module: tests/unit/cli/test_structure_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_structure_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_structure_command`/
symbols:
  TestR37aaStructureCanonicalEnvelope.test_method_row_class_name_uses_parent_class_field: TestR37aaStructureCanonicalEnvelope#test_method_row_class_name_uses_parent_class_field().
  TestStructureCommandInit.test_init_with_args: TestStructureCommandInit#test_init_with_args().
  TestStructureCommandConvertToLegacyFormat.test_convert_to_legacy_format_statistics: TestStructureCommandConvertToLegacyFormat#test_convert_to_legacy_format_statistics().
  command: command().
  TestStructureCommandInit.test_init: TestStructureCommandInit#test_init().
  TestStructureCommandConvertToLegacyFormat.test_convert_to_legacy_format_with_classes: TestStructureCommandConvertToLegacyFormat#test_convert_to_legacy_format_with_classes().
  TestStructureCommandConvertToLegacyFormat.test_convert_to_legacy_format_with_methods: TestStructureCommandConvertToLegacyFormat#test_convert_to_legacy_format_with_methods().
  TestStructureCommandConvertToLegacyFormat.test_convert_to_legacy_format_method_has_class_name_and_is_method: TestStructureCommandConvertToLegacyFormat#test_convert_to_legacy_format_method_has_class_name_and_is_method().
  TestStructureCommandConvertToLegacyFormat.test_convert_to_legacy_format_with_fields: TestStructureCommandConvertToLegacyFormat#test_convert_to_legacy_format_with_fields().
  mock_args: mock_args().
  TestStructureCommandInit: TestStructureCommandInit#
  TestStructureCommandExecuteAsync: TestStructureCommandExecuteAsync#
  TestStructureCommandExecuteAsync.test_execute_async_success: TestStructureCommandExecuteAsync#test_execute_async_success().
  TestStructureCommandExecuteAsync.test_execute_async_no_analysis_result: TestStructureCommandExecuteAsync#test_execute_async_no_analysis_result().
  TestStructureCommandExecuteAsync.test_execute_async_calls_output_structure_analysis: TestStructureCommandExecuteAsync#test_execute_async_calls_output_structure_analysis().
  TestStructureCommandConvertToLegacyFormat: TestStructureCommandConvertToLegacyFormat#
  TestStructureCommandConvertToLegacyFormat.test_convert_to_legacy_format_empty_elements: TestStructureCommandConvertToLegacyFormat#test_convert_to_legacy_format_empty_elements().
  TestStructureCommandConvertToLegacyFormat.test_convert_to_legacy_format_metadata: TestStructureCommandConvertToLegacyFormat#test_convert_to_legacy_format_metadata().
  TestStructureCommandOutputStructureAnalysis: TestStructureCommandOutputStructureAnalysis#
  TestStructureCommandOutputStructureAnalysis.test_output_structure_analysis_text: TestStructureCommandOutputStructureAnalysis#test_output_structure_analysis_text().
  TestStructureCommandOutputStructureAnalysis.test_output_structure_analysis_json: TestStructureCommandOutputStructureAnalysis#test_output_structure_analysis_json().
  TestStructureCommandOutputStructureAnalysis.test_output_structure_analysis_toon: TestStructureCommandOutputStructureAnalysis#test_output_structure_analysis_toon().
  TestStructureCommandOutputTextFormat: TestStructureCommandOutputTextFormat#
  TestStructureCommandOutputTextFormat.test_output_text_format_basic: TestStructureCommandOutputTextFormat#test_output_text_format_basic().
  TestStructureCommandOutputTextFormat.test_output_text_format_with_package: TestStructureCommandOutputTextFormat#test_output_text_format_with_package().
  TestStructureCommandOutputTextFormat.test_output_text_format_with_classes: TestStructureCommandOutputTextFormat#test_output_text_format_with_classes().
  TestStructureCommandOutputTextFormat.test_output_text_format_with_methods: TestStructureCommandOutputTextFormat#test_output_text_format_with_methods().
  TestStructureCommandOutputTextFormat.test_output_text_format_with_fields: TestStructureCommandOutputTextFormat#test_output_text_format_with_fields().
  TestR37aaStructureCanonicalEnvelope: TestR37aaStructureCanonicalEnvelope#
  TestR37aaStructureCanonicalEnvelope.test_structure_emits_canonical_envelope: TestR37aaStructureCanonicalEnvelope#test_structure_emits_canonical_envelope().
  TestR37aaStructureCanonicalEnvelope.test_structure_success_key_present: TestR37aaStructureCanonicalEnvelope#test_structure_success_key_present().
---
# Module: [`tests/unit/cli/test_structure_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py)

## Classes
### `TestR37aaStructureCanonicalEnvelope`
- def: [`tests/unit/cli/test_structure_command.py:529`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L529)
- doc: r37aa (dogfood): CLI `--structure` was the third CLI surface
- signature: `class TestR37aaStructureCanonicalEnvelope:`
- members:
  - `test_method_row_class_name_uses_parent_class_field(self, command)` — [`L568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L568) — Codex P2 #742: real Function elements store owner in parent_class, not class_name.
  - `test_structure_emits_canonical_envelope(self, command)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L535)
  - `test_structure_success_key_present(self, command)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L555)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`StructureCommand`](../../../tree_sitter_analyzer/cli/commands/structure_command.md#StructureCommand), [`parent_class`](../../../tree_sitter_analyzer/models/base.md#Function.parent_class), [`_legacy_method_row`](../../../tree_sitter_analyzer/cli/commands/structure_command.md#StructureCommand._legacy_method_row)

### `TestStructureCommandConvertToLegacyFormat`
- def: [`tests/unit/cli/test_structure_command.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L123)
- doc: Tests for StructureCommand._convert_to_legacy_format method.
- signature: `class TestStructureCommandConvertToLegacyFormat:`
- members:
  - `test_convert_to_legacy_format_empty_elements(self, command)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L126) — Test _convert_to_legacy_format with empty elements.
  - `test_convert_to_legacy_format_metadata(self, command)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L297) — Test _convert_to_legacy_format includes metadata.
  - `test_convert_to_legacy_format_method_has_class_name_and_is_method(self, command)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L200) — #742: methods[] entries must carry class_name and is_method for --advanced parity.
  - `test_convert_to_legacy_format_statistics(self, command)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L257) — Test _convert_to_legacy_format includes statistics.
  - `test_convert_to_legacy_format_with_classes(self, command)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L148) — Test _convert_to_legacy_format with class elements.
  - `test_convert_to_legacy_format_with_fields(self, command)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L231) — Test _convert_to_legacy_format with field elements.
  - `test_convert_to_legacy_format_with_methods(self, command)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L174) — Test _convert_to_legacy_format with method elements.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE)

### `TestStructureCommandExecuteAsync`
- def: [`tests/unit/cli/test_structure_command.py:69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L69)
- doc: Tests for StructureCommand.execute_async method.
- signature: `class TestStructureCommandExecuteAsync:`
- members:
  - `test_execute_async_calls_output_structure_analysis(self, command)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L104) — Test execute_async calls _output_structure_analysis.
  - `test_execute_async_no_analysis_result(self, command)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L93) — Test execute_async returns 1 when no analysis result.
  - `test_execute_async_success(self, command)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L73) — Test execute_async returns 0 on success.

### `TestStructureCommandInit`
- def: [`tests/unit/cli/test_structure_command.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L54)
- doc: Tests for StructureCommand initialization.
- signature: `class TestStructureCommandInit:`
- members:
  - `test_init(self, command)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L57) — Test StructureCommand initialization.
  - `test_init_with_args(self, mock_args)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L63) — Test StructureCommand initialization with args.
- uses (calls/refs, reference-scoped): [`args`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.args), [`StructureCommand`](../../../tree_sitter_analyzer/cli/commands/structure_command.md#StructureCommand)

### `TestStructureCommandOutputStructureAnalysis`
- def: [`tests/unit/cli/test_structure_command.py:316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L316)
- doc: Tests for StructureCommand._output_structure_analysis method.
- signature: `class TestStructureCommandOutputStructureAnalysis:`
- members:
  - `test_output_structure_analysis_json(self, command)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L341) — Test _output_structure_analysis with JSON format.
  - `test_output_structure_analysis_text(self, command)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L319) — Test _output_structure_analysis with text format.
  - `test_output_structure_analysis_toon(self, command)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L359) — Test _output_structure_analysis with TOON format.

### `TestStructureCommandOutputTextFormat`
- def: [`tests/unit/cli/test_structure_command.py:388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L388)
- doc: Tests for StructureCommand._output_text_format method.
- signature: `class TestStructureCommandOutputTextFormat:`
- members:
  - `test_output_text_format_basic(self, command)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L391) — Test _output_text_format with basic structure.
  - `test_output_text_format_with_classes(self, command)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L444) — Test _output_text_format with classes.
  - `test_output_text_format_with_fields(self, command)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L500) — Test _output_text_format with fields.
  - `test_output_text_format_with_methods(self, command)` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L472) — Test _output_text_format with methods.
  - `test_output_text_format_with_package(self, command)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L417) — Test _output_text_format with package.

## Functions
- `command(mock_args)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L49) — Create StructureCommand instance for testing.
- `mock_args()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_structure_command.py#L15) — Create mock args for BaseCommand initialization.

