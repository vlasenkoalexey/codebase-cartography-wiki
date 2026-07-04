---
title: 'Module: tests/unit/cli/test_summary_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_summary_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_summary_command`/
symbols:
  TestSummarySQLParameterSerialization.test_sql_method_parameters_are_json_safe_dicts: TestSummarySQLParameterSerialization#test_sql_method_parameters_are_json_safe_dicts().
  TestSummaryCommandOutputSummaryAnalysis.test_output_summary_analysis_all_types: TestSummaryCommandOutputSummaryAnalysis#test_output_summary_analysis_all_types().
  TestSummaryCommandInit.test_init_with_args: TestSummaryCommandInit#test_init_with_args().
  TestSummaryCommandOutputSummaryAnalysis.test_output_summary_analysis_default_types: TestSummaryCommandOutputSummaryAnalysis#test_output_summary_analysis_default_types().
  TestSummaryCommandOutputSummaryAnalysis.test_output_summary_analysis_custom_types: TestSummaryCommandOutputSummaryAnalysis#test_output_summary_analysis_custom_types().
  command: command().
  TestSummaryCommandInit.test_init: TestSummaryCommandInit#test_init().
  mock_args: mock_args().
  TestSummaryCommandInit: TestSummaryCommandInit#
  TestSummaryCommandExecuteAsync: TestSummaryCommandExecuteAsync#
  TestSummaryCommandExecuteAsync.test_execute_async_success: TestSummaryCommandExecuteAsync#test_execute_async_success().
  TestSummaryCommandExecuteAsync.test_execute_async_no_analysis_result: TestSummaryCommandExecuteAsync#test_execute_async_no_analysis_result().
  TestSummaryCommandExecuteAsync.test_execute_async_calls_output_summary_analysis: TestSummaryCommandExecuteAsync#test_execute_async_calls_output_summary_analysis().
  TestSummaryCommandOutputSummaryAnalysis: TestSummaryCommandOutputSummaryAnalysis#
  TestSummaryCommandOutputSummaryAnalysis.test_output_summary_analysis_text: TestSummaryCommandOutputSummaryAnalysis#test_output_summary_analysis_text().
  TestSummaryCommandOutputSummaryAnalysis.test_output_summary_analysis_json: TestSummaryCommandOutputSummaryAnalysis#test_output_summary_analysis_json().
  TestSummaryCommandOutputSummaryAnalysis.test_output_summary_analysis_toon: TestSummaryCommandOutputSummaryAnalysis#test_output_summary_analysis_toon().
  TestSummaryCommandOutputTextFormat: TestSummaryCommandOutputTextFormat#
  TestSummaryCommandOutputTextFormat.test_output_text_format_basic: TestSummaryCommandOutputTextFormat#test_output_text_format_basic().
  TestSummaryCommandOutputTextFormat.test_output_text_format_with_classes: TestSummaryCommandOutputTextFormat#test_output_text_format_with_classes().
  TestSummaryCommandOutputTextFormat.test_output_text_format_with_methods: TestSummaryCommandOutputTextFormat#test_output_text_format_with_methods().
  TestSummaryCommandOutputTextFormat.test_output_text_format_with_fields: TestSummaryCommandOutputTextFormat#test_output_text_format_with_fields().
  TestSummaryCommandOutputTextFormat.test_output_text_format_with_imports: TestSummaryCommandOutputTextFormat#test_output_text_format_with_imports().
  TestSummaryCommandOutputTextFormat.test_output_text_format_multiple_types: TestSummaryCommandOutputTextFormat#test_output_text_format_multiple_types().
  TestSummaryCommandOutputTextFormat.test_output_text_format_empty_elements: TestSummaryCommandOutputTextFormat#test_output_text_format_empty_elements().
  TestR37zSummaryCanonicalEnvelope: TestR37zSummaryCanonicalEnvelope#
  TestR37zSummaryCanonicalEnvelope.test_summary_emits_canonical_envelope: TestR37zSummaryCanonicalEnvelope#test_summary_emits_canonical_envelope().
  TestR37zSummaryCanonicalEnvelope.test_summary_success_key_present: TestR37zSummaryCanonicalEnvelope#test_summary_success_key_present().
  TestSummarySQLParameterSerialization: TestSummarySQLParameterSerialization#
---
# Module: [`tests/unit/cli/test_summary_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py)

## Classes
### `TestR37zSummaryCanonicalEnvelope`
- def: [`tests/unit/cli/test_summary_command.py:457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L457)
- doc: r37z (dogfood): CLI `--summary` was missing
- signature: `class TestR37zSummaryCanonicalEnvelope:`
- members:
  - `test_summary_emits_canonical_envelope(self, command)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L463)
  - `test_summary_success_key_present(self, command)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L493) — Even on an empty file, ``success: True`` must be set explicitly.

### `TestSummaryCommandExecuteAsync`
- def: [`tests/unit/cli/test_summary_command.py:69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L69)
- doc: Tests for SummaryCommand.execute_async method.
- signature: `class TestSummaryCommandExecuteAsync:`
- members:
  - `test_execute_async_calls_output_summary_analysis(self, command)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L104) — Test execute_async calls _output_summary_analysis.
  - `test_execute_async_no_analysis_result(self, command)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L93) — Test execute_async returns 1 when no analysis result.
  - `test_execute_async_success(self, command)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L73) — Test execute_async returns 0 on success.

### `TestSummaryCommandInit`
- def: [`tests/unit/cli/test_summary_command.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L54)
- doc: Tests for SummaryCommand initialization.
- signature: `class TestSummaryCommandInit:`
- members:
  - `test_init(self, command)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L57) — Test SummaryCommand initialization.
  - `test_init_with_args(self, mock_args)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L63) — Test SummaryCommand initialization with args.
- uses (calls/refs, reference-scoped): [`args`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.args), [`SummaryCommand`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand)

### `TestSummaryCommandOutputSummaryAnalysis`
- def: [`tests/unit/cli/test_summary_command.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L123)
- doc: Tests for SummaryCommand._output_summary_analysis method.
- signature: `class TestSummaryCommandOutputSummaryAnalysis:`
- members:
  - `test_output_summary_analysis_all_types(self, command)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L270) — Test _output_summary_analysis with all types.
  - `test_output_summary_analysis_custom_types(self, command)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L233) — Test _output_summary_analysis with custom types.
  - `test_output_summary_analysis_default_types(self, command)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L196) — Test _output_summary_analysis with default types.
  - `test_output_summary_analysis_json(self, command)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L149) — Test _output_summary_analysis with JSON format.
  - `test_output_summary_analysis_text(self, command)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L126) — Test _output_summary_analysis with text format.
  - `test_output_summary_analysis_toon(self, command)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L168) — Test _output_summary_analysis with TOON format.
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE), [`ELEMENT_TYPE_IMPORT`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_IMPORT)

### `TestSummaryCommandOutputTextFormat`
- def: [`tests/unit/cli/test_summary_command.py:318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L318)
- doc: Tests for SummaryCommand._output_text_format method.
- signature: `class TestSummaryCommandOutputTextFormat:`
- members:
  - `test_output_text_format_basic(self, command)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L321) — Test _output_text_format with basic summary.
  - `test_output_text_format_empty_elements(self, command)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L437) — Test _output_text_format with empty elements.
  - `test_output_text_format_multiple_types(self, command)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L416) — Test _output_text_format with multiple types.
  - `test_output_text_format_with_classes(self, command)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L338) — Test _output_text_format with classes.
  - `test_output_text_format_with_fields(self, command)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L376) — Test _output_text_format with fields.
  - `test_output_text_format_with_imports(self, command)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L396) — Test _output_text_format with imports.
  - `test_output_text_format_with_methods(self, command)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L357) — Test _output_text_format with methods.

### `TestSummarySQLParameterSerialization`
- def: [`tests/unit/cli/test_summary_command.py:513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L513)
- doc: Regression for #1015: --summary --format json crashed on SQL methods.
- signature: `class TestSummarySQLParameterSerialization:`
- members:
  - `test_sql_method_parameters_are_json_safe_dicts(self, command)` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L522) — Method params become plain dicts and the payload is JSON-serializable.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`SQLElementType`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`parameters`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.parameters), [`SQLParameter`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter), [`name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter.name), [`data_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter.data_type), [`sql_element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction.sql_element_type), [`FUNCTION`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType.FUNCTION), [`direction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter.direction)

## Functions
- `command(mock_args)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L49) — Create SummaryCommand instance for testing.
- `mock_args()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command.py#L15) — Create mock args for BaseCommand initialization.

