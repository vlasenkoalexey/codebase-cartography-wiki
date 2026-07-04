---
title: 'Module: tests/integration/cli/test_cli_core.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_core`/TestCLI
symbols:
  TestCLIAdvancedOptions.test_advanced_option_analysis_failure: AdvancedOptions#test_advanced_option_analysis_failure().
  TestCLISummaryOption.test_summary_option_analysis_failure: SummaryOption#test_summary_option_analysis_failure().
  TestCLIStructureOption.test_structure_option_analysis_failure: StructureOption#test_structure_option_analysis_failure().
  TestCLIAdvancedOptions.test_advanced_option_json_output: AdvancedOptions#test_advanced_option_json_output().
  TestCLIAdvancedOptions.test_advanced_option_text_output: AdvancedOptions#test_advanced_option_text_output().
  TestCLIAdvancedOptions.test_advanced_option_text_output_strict: AdvancedOptions#test_advanced_option_text_output_strict().
  TestCLIAdvancedOptions.test_statistics_option: AdvancedOptions#test_statistics_option().
  TestCLIAdvancedOptions.test_statistics_option_json: AdvancedOptions#test_statistics_option_json().
  TestCLISummaryOption.test_summary_option_default: SummaryOption#test_summary_option_default().
  TestCLISummaryOption.test_summary_option_specific_types: SummaryOption#test_summary_option_specific_types().
  TestCLISummaryOption.test_summary_option_json: SummaryOption#test_summary_option_json().
  TestCLIStructureOption.test_structure_option_json: StructureOption#test_structure_option_json().
  TestCLIStructureOption.test_structure_option_text: StructureOption#test_structure_option_text().
  TestCLIAdvancedOptions: AdvancedOptions#
  TestCLISummaryOption: SummaryOption#
  TestCLIStructureOption: StructureOption#
---
# Module: [`tests/integration/cli/test_cli_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py)

## Classes
### `TestCLIAdvancedOptions`
- def: [`tests/integration/cli/test_cli_core.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L14)
- doc: Test cases for advanced CLI options
- signature: `class TestCLIAdvancedOptions:`
- members:
  - `test_advanced_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L139) — Test --advanced option when analysis fails
  - `test_advanced_option_json_output(self, monkeypatch, sample_java_file)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L17) — Test --advanced option with JSON output
  - `test_advanced_option_text_output(self, monkeypatch, sample_java_file)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L52) — Test --advanced option with text output
  - `test_advanced_option_text_output_strict(self, monkeypatch, sample_java_file)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L86) — Test --advanced option with strict content validation
  - `test_statistics_option(self, monkeypatch, sample_java_file)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L178) — Test --statistics option
  - `test_statistics_option_json(self, monkeypatch, sample_java_file)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L211) — Test --statistics option with JSON output
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

### `TestCLIStructureOption`
- def: [`tests/integration/cli/test_cli_core.py:387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L387)
- doc: Test cases for --structure option
- signature: `class TestCLIStructureOption:`
- members:
  - `test_structure_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L456) — Test --structure option when analysis fails
  - `test_structure_option_json(self, monkeypatch, sample_java_file)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L390) — Test --structure option with JSON output
  - `test_structure_option_text(self, monkeypatch, sample_java_file)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L424) — Test --structure option with text output
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

### `TestCLISummaryOption`
- def: [`tests/integration/cli/test_cli_core.py:246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L246)
- doc: Test cases for --summary option
- signature: `class TestCLISummaryOption:`
- members:
  - `test_summary_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L347) — Test --summary option when analysis fails
  - `test_summary_option_default(self, monkeypatch, sample_java_file)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L249) — Test --summary option with default types
  - `test_summary_option_json(self, monkeypatch, sample_java_file)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L312) — Test --summary option with JSON output
  - `test_summary_option_specific_types(self, monkeypatch, sample_java_file)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_core.py#L277) — Test --summary option with specific types
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

