---
title: 'Module: tests/unit/cli/test_summary_command_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_summary_command_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_summary_command_comprehensive`/Test
symbols:
  TestOutputSummaryAnalysis.test_output_summary_filters_elements_correctly: OutputSummaryAnalysis#test_output_summary_filters_elements_correctly().
  TestOutputSummaryAnalysis.side_effect: OutputSummaryAnalysis#side_effect().
  TestSummaryCommandInitialization.test_init_with_args: SummaryCommandInitialization#test_init_with_args().
  TestSummaryCommandInitialization.test_inherits_from_base_command: SummaryCommandInitialization#test_inherits_from_base_command().
  TestOutputSummaryAnalysis.test_output_summary_with_classes_and_methods: OutputSummaryAnalysis#test_output_summary_with_classes_and_methods().
  TestOutputSummaryAnalysis.test_output_summary_with_custom_types: OutputSummaryAnalysis#test_output_summary_with_custom_types().
  TestExecuteAsync.command: ExecuteAsync#command().
  TestExecuteAsync.test_execute_async_success: ExecuteAsync#test_execute_async_success().
  TestExecuteAsync.test_execute_async_calls_output_summary: ExecuteAsync#test_execute_async_calls_output_summary().
  TestOutputSummaryAnalysis.command: OutputSummaryAnalysis#command().
  TestOutputSummaryAnalysis.test_output_summary_with_json_format: OutputSummaryAnalysis#test_output_summary_with_json_format().
  TestOutputSummaryAnalysis.test_output_summary_with_empty_summary_types: OutputSummaryAnalysis#test_output_summary_with_empty_summary_types().
  TestOutputSummaryAnalysis.test_output_summary_with_none_summary_types: OutputSummaryAnalysis#test_output_summary_with_none_summary_types().
  TestOutputSummaryAnalysis.test_output_summary_with_whitespace_in_types: OutputSummaryAnalysis#test_output_summary_with_whitespace_in_types().
  TestOutputTextFormat.command: OutputTextFormat#command().
  TestEdgeCases.command: EdgeCases#command().
  TestEdgeCases.test_element_without_name_attribute: EdgeCases#test_element_without_name_attribute().
  TestEdgeCases.test_large_number_of_elements: EdgeCases#test_large_number_of_elements().
  TestEdgeCases.test_single_element_type_requested: EdgeCases#test_single_element_type_requested().
  TestSummaryCommandInitialization: SummaryCommandInitialization#
  TestExecuteAsync: ExecuteAsync#
  TestExecuteAsync.test_execute_async_with_none_result: ExecuteAsync#test_execute_async_with_none_result().
  TestOutputSummaryAnalysis: OutputSummaryAnalysis#
  TestOutputTextFormat: OutputTextFormat#
  TestOutputTextFormat.test_output_text_format_with_classes: OutputTextFormat#test_output_text_format_with_classes().
  TestOutputTextFormat.test_output_text_format_with_methods: OutputTextFormat#test_output_text_format_with_methods().
  TestOutputTextFormat.test_output_text_format_with_fields: OutputTextFormat#test_output_text_format_with_fields().
  TestOutputTextFormat.test_output_text_format_with_imports: OutputTextFormat#test_output_text_format_with_imports().
  TestOutputTextFormat.test_output_text_format_with_multiple_types: OutputTextFormat#test_output_text_format_with_multiple_types().
  TestOutputTextFormat.test_output_text_format_with_empty_elements: OutputTextFormat#test_output_text_format_with_empty_elements().
  TestOutputTextFormat.test_output_text_format_with_unknown_type: OutputTextFormat#test_output_text_format_with_unknown_type().
  TestOutputTextFormat.test_output_text_format_displays_counts: OutputTextFormat#test_output_text_format_displays_counts().
  TestEdgeCases: EdgeCases#
---
# Module: [`tests/unit/cli/test_summary_command_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py)

## Classes
### `TestEdgeCases`
- def: [`tests/unit/cli/test_summary_command_comprehensive.py:521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L521)
- doc: Test edge cases and error conditions.
- signature: `class TestEdgeCases:`
- members:
  - `command(self)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L525) — Create a SummaryCommand instance.
  - `test_element_without_name_attribute(self, command)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L532) — Test handling element without name attribute.
  - `test_large_number_of_elements(self, command)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L555) — Test handling large number of elements.
  - `test_single_element_type_requested(self, command)` — [`L580`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L580) — Test requesting only a single element type.
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`SummaryCommand`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand)

### `TestExecuteAsync`
- def: [`tests/unit/cli/test_summary_command_comprehensive.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L33)
- doc: Test execute_async method.
- signature: `class TestExecuteAsync:`
- members:
  - `command(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L37) — Create a SummaryCommand instance.
  - `test_execute_async_calls_output_summary(self, command)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L71) — Test that execute_async calls _output_summary_analysis.
  - `test_execute_async_success(self, command)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L45) — Test successful execute_async.
  - `test_execute_async_with_none_result(self, command)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L61) — Test execute_async when analyze_file returns None.
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`SummaryCommand`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand)

### `TestOutputSummaryAnalysis`
- def: [`tests/unit/cli/test_summary_command_comprehensive.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L87)
- doc: Test _output_summary_analysis method.
- signature: `class TestOutputSummaryAnalysis:`
- members:
  - `command(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L91) — Create a SummaryCommand instance.
  - `side_effect(element, element_type)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L119)
  - `test_output_summary_filters_elements_correctly(self, command)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L274) — Test that elements are filtered correctly by type.
  - `test_output_summary_with_classes_and_methods(self, command)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L98) — Test outputting summary with classes and methods.
  - `test_output_summary_with_custom_types(self, command)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L154) — Test outputting summary with custom types.
  - `test_output_summary_with_empty_summary_types(self, command)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L208) — Test outputting summary with empty summary types (uses defaults).
  - `test_output_summary_with_json_format(self, command)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L134) — Test outputting summary in JSON format.
  - `test_output_summary_with_none_summary_types(self, command)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L230) — Test outputting summary with None summary types.
  - `test_output_summary_with_whitespace_in_types(self, command)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L252) — Test outputting summary with whitespace in types.
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`SummaryCommand`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand)

### `TestOutputTextFormat`
- def: [`tests/unit/cli/test_summary_command_comprehensive.py:323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L323)
- doc: Test _output_text_format method.
- signature: `class TestOutputTextFormat:`
- members:
  - `command(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L327) — Create a SummaryCommand instance.
  - `test_output_text_format_displays_counts(self, command)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L494) — Test that text format displays counts correctly.
  - `test_output_text_format_with_classes(self, command)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L334) — Test text format output with classes.
  - `test_output_text_format_with_empty_elements(self, command)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L456) — Test text format output with empty elements.
  - `test_output_text_format_with_fields(self, command)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L385) — Test text format output with fields.
  - `test_output_text_format_with_imports(self, command)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L407) — Test text format output with imports.
  - `test_output_text_format_with_methods(self, command)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L361) — Test text format output with methods.
  - `test_output_text_format_with_multiple_types(self, command)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L431) — Test text format output with multiple types.
  - `test_output_text_format_with_unknown_type(self, command)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L476) — Test text format output with unknown type.
- uses (calls/refs, reference-scoped): [`SummaryCommand`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand)

### `TestSummaryCommandInitialization`
- def: [`tests/unit/cli/test_summary_command_comprehensive.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L17)
- doc: Test SummaryCommand initialization.
- signature: `class TestSummaryCommandInitialization:`
- members:
  - `test_inherits_from_base_command(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L26) — Test that SummaryCommand inherits from BaseCommand.
  - `test_init_with_args(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_summary_command_comprehensive.py#L20) — Test initialization with args.
- uses (calls/refs, reference-scoped): [`args`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.args), [`BaseCommand`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand), [`SummaryCommand`](../../../tree_sitter_analyzer/cli/commands/summary_command.md#SummaryCommand)

