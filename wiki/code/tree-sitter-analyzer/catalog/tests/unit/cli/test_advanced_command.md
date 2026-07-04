---
title: 'Module: tests/unit/cli/test_advanced_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_advanced_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_advanced_command`/
symbols:
  TestBuildElementsPayloadClassType._make_class: TestBuildElementsPayloadClassType#_make_class().
  TestBuildElementsPayloadClassType.test_function_unaffected: TestBuildElementsPayloadClassType#test_function_unaffected().
  TestBuildElementsPayloadClassType._build: TestBuildElementsPayloadClassType#_build().
  TestBuildElementsPayloadClassType.test_interface_type_preserved: TestBuildElementsPayloadClassType#test_interface_type_preserved().
  TestBuildElementsPayloadClassType.test_enum_type_preserved: TestBuildElementsPayloadClassType#test_enum_type_preserved().
  TestBuildElementsPayloadClassType.test_type_alias_preserved: TestBuildElementsPayloadClassType#test_type_alias_preserved().
  TestBuildElementsPayloadClassType.test_namespace_type_preserved: TestBuildElementsPayloadClassType#test_namespace_type_preserved().
  TestBuildElementsPayloadClassType.test_actual_class_still_class: TestBuildElementsPayloadClassType#test_actual_class_still_class().
  command: command().
  mock_analysis_result: mock_analysis_result().
  mock_args: mock_args().
  TestAdvancedCommandInit: TestAdvancedCommandInit#
  TestAdvancedCommandInit.test_init: TestAdvancedCommandInit#test_init().
  TestAdvancedCommandInit.test_init_with_args: TestAdvancedCommandInit#test_init_with_args().
  TestAdvancedCommandExecuteAsync: TestAdvancedCommandExecuteAsync#
  TestAdvancedCommandExecuteAsync.test_execute_async_success: TestAdvancedCommandExecuteAsync#test_execute_async_success().
  TestAdvancedCommandExecuteAsync.test_execute_async_with_statistics: TestAdvancedCommandExecuteAsync#test_execute_async_with_statistics().
  TestAdvancedCommandExecuteAsync.test_execute_async_no_analysis_result: TestAdvancedCommandExecuteAsync#test_execute_async_no_analysis_result().
  TestAdvancedCommandCalculateFileMetrics: TestAdvancedCommandCalculateFileMetrics#
  TestAdvancedCommandCalculateFileMetrics.test_calculate_file_metrics_python: TestAdvancedCommandCalculateFileMetrics#test_calculate_file_metrics_python().
  TestAdvancedCommandCalculateFileMetrics.test_calculate_file_metrics_java: TestAdvancedCommandCalculateFileMetrics#test_calculate_file_metrics_java().
  TestAdvancedCommandCalculateFileMetrics.test_calculate_file_metrics_sql: TestAdvancedCommandCalculateFileMetrics#test_calculate_file_metrics_sql().
  TestAdvancedCommandCalculateFileMetrics.test_calculate_file_metrics_html: TestAdvancedCommandCalculateFileMetrics#test_calculate_file_metrics_html().
  TestAdvancedCommandCalculateFileMetrics.test_calculate_file_metrics_empty_file: TestAdvancedCommandCalculateFileMetrics#test_calculate_file_metrics_empty_file().
  TestAdvancedCommandCalculateFileMetrics.test_calculate_file_metrics_file_read_error: TestAdvancedCommandCalculateFileMetrics#test_calculate_file_metrics_file_read_error().
  TestAdvancedCommandOutputStatistics: TestAdvancedCommandOutputStatistics#
  TestAdvancedCommandOutputStatistics.test_output_statistics_text: TestAdvancedCommandOutputStatistics#test_output_statistics_text().
  TestAdvancedCommandOutputStatistics.test_output_statistics_json: TestAdvancedCommandOutputStatistics#test_output_statistics_json().
  TestAdvancedCommandOutputStatistics.test_output_statistics_toon: TestAdvancedCommandOutputStatistics#test_output_statistics_toon().
  TestAdvancedCommandOutputFullAnalysis: TestAdvancedCommandOutputFullAnalysis#
  TestAdvancedCommandOutputFullAnalysis.test_output_full_analysis_text: TestAdvancedCommandOutputFullAnalysis#test_output_full_analysis_text().
  TestAdvancedCommandOutputFullAnalysis.test_output_full_analysis_json: TestAdvancedCommandOutputFullAnalysis#test_output_full_analysis_json().
  TestAdvancedCommandOutputFullAnalysis.test_output_full_analysis_toon: TestAdvancedCommandOutputFullAnalysis#test_output_full_analysis_toon().
  TestAdvancedCommandOutputTextAnalysis: TestAdvancedCommandOutputTextAnalysis#
  TestAdvancedCommandOutputTextAnalysis.test_output_text_analysis_basic: TestAdvancedCommandOutputTextAnalysis#test_output_text_analysis_basic().
  TestAdvancedCommandOutputTextAnalysis.test_output_text_analysis_no_methods: TestAdvancedCommandOutputTextAnalysis#test_output_text_analysis_no_methods().
  TestR37yCanonicalEnvelope: TestR37yCanonicalEnvelope#
  TestR37yCanonicalEnvelope.test_full_analysis_emits_canonical_envelope: TestR37yCanonicalEnvelope#test_full_analysis_emits_canonical_envelope().
  TestR37yCanonicalEnvelope.test_statistics_emits_canonical_envelope: TestR37yCanonicalEnvelope#test_statistics_emits_canonical_envelope().
  TestR37yCanonicalEnvelope.test_full_mode_label_differs_from_stats: TestR37yCanonicalEnvelope#test_full_mode_label_differs_from_stats().
  TestBuildElementsPayloadClassType: TestBuildElementsPayloadClassType#
---
# Module: [`tests/unit/cli/test_advanced_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py)

## Classes
### `TestAdvancedCommandCalculateFileMetrics`
- def: [`tests/unit/cli/test_advanced_command.py:125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L125)
- doc: Tests for _calculate_file_metrics method.
- signature: `class TestAdvancedCommandCalculateFileMetrics:`
- members:
  - `test_calculate_file_metrics_empty_file(self, command, tmp_path)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L191) — Test calculating metrics for empty file.
  - `test_calculate_file_metrics_file_read_error(self, command)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L203) — Test calculating metrics when file read fails.
  - `test_calculate_file_metrics_html(self, command, tmp_path)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L179) — Test calculating metrics for HTML file.
  - `test_calculate_file_metrics_java(self, command, tmp_path)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L146) — Test calculating metrics for Java file.
  - `test_calculate_file_metrics_python(self, command, tmp_path)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L128) — Test calculating metrics for Python file.
  - `test_calculate_file_metrics_sql(self, command, tmp_path)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L165) — Test calculating metrics for SQL file.

### `TestAdvancedCommandExecuteAsync`
- def: [`tests/unit/cli/test_advanced_command.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L68)
- doc: Tests for execute_async method.
- signature: `class TestAdvancedCommandExecuteAsync:`
- members:
  - `test_execute_async_no_analysis_result(self, command)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L112) — Test execution when analysis returns None.
  - `test_execute_async_success(self, command, mock_analysis_result)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L72) — Test successful execution.
  - `test_execute_async_with_statistics(self, command, mock_analysis_result)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L92) — Test execution with statistics flag.

### `TestAdvancedCommandInit`
- def: [`tests/unit/cli/test_advanced_command.py:50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L50)
- doc: Tests for AdvancedCommand initialization.
- signature: `class TestAdvancedCommandInit:`
- members:
  - `test_init(self, command)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L53) — Test initialization.
  - `test_init_with_args(self, command)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L59) — Test initialization with arguments.

### `TestAdvancedCommandOutputFullAnalysis`
- def: [`tests/unit/cli/test_advanced_command.py:279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L279)
- doc: Tests for _output_full_analysis method.
- signature: `class TestAdvancedCommandOutputFullAnalysis:`
- members:
  - `test_output_full_analysis_json(self, command, mock_analysis_result)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L299) — Test output full analysis in JSON format.
  - `test_output_full_analysis_text(self, command, mock_analysis_result)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L282) — Test output full analysis in text format.
  - `test_output_full_analysis_toon(self, command, mock_analysis_result)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L320) — Test output full analysis in toon format.

### `TestAdvancedCommandOutputStatistics`
- def: [`tests/unit/cli/test_advanced_command.py:214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L214)
- doc: Tests for _output_statistics method.
- signature: `class TestAdvancedCommandOutputStatistics:`
- members:
  - `test_output_statistics_json(self, command, mock_analysis_result)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L237) — Test output statistics in JSON format.
  - `test_output_statistics_text(self, command, mock_analysis_result)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L217) — Test output statistics in text format.
  - `test_output_statistics_toon(self, command, mock_analysis_result)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L257) — Test output statistics in toon format.

### `TestAdvancedCommandOutputTextAnalysis`
- def: [`tests/unit/cli/test_advanced_command.py:342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L342)
- doc: Tests for _output_text_analysis method.
- signature: `class TestAdvancedCommandOutputTextAnalysis:`
- members:
  - `test_output_text_analysis_basic(self, command, mock_analysis_result)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L345) — Test basic text analysis output.
  - `test_output_text_analysis_no_methods(self, command, mock_analysis_result)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L367) — Test text analysis when no methods present.

### `TestBuildElementsPayloadClassType`
- def: [`tests/unit/cli/test_advanced_command.py:476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L476)
- doc: #795: enum/interface/type-alias mislabeled as type='class' in --advanced.
- signature: `class TestBuildElementsPayloadClassType:`
- members:
  - `test_actual_class_still_class(self)` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L520)
  - `test_enum_type_preserved(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L508)
  - `test_function_unaffected(self)` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L524)
  - `test_interface_type_preserved(self)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L504)
  - `test_namespace_type_preserved(self)` — [`L516`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L516)
  - `test_type_alias_preserved(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L512)
- protocol/private: `_build`[`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L497), `_make_class`[`L485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L485)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`_build_elements_payload`](../../../tree_sitter_analyzer/cli/commands/advanced_command.md#_build_elements_payload)

### `TestR37yCanonicalEnvelope`
- def: [`tests/unit/cli/test_advanced_command.py:395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L395)
- doc: r37y (dogfood): CLI `--advanced` JSON output was missing
- signature: `class TestR37yCanonicalEnvelope:`
- members:
  - `test_full_analysis_emits_canonical_envelope(self, command, mock_analysis_result)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L401) — ``--advanced --format json`` must include summary_line + verdict + agent_summary.
  - `test_full_mode_label_differs_from_stats(self, command, mock_analysis_result)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L446) — summary_line carries mode= label to distinguish dispatch paths.
  - `test_statistics_emits_canonical_envelope(self, command, mock_analysis_result)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L426) — ``--advanced --statistics --format json`` also exposes envelope.

## Functions
- `command(mock_args)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L31) — Create an AdvancedCommand instance for testing.
- `mock_analysis_result()` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L37) — Create a mock analysis result.
- `mock_args()` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_advanced_command.py#L18) — Create mock arguments for testing.

