---
title: 'Module: tests/integration/cli/test_cli_advanced_summary_structure.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_advanced_summary_structure.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_advanced_summary_structure`/TestCLI
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
# Module: [`tests/integration/cli/test_cli_advanced_summary_structure.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py)

## Classes
### `TestCLIAdvancedOptions`
- def: [`tests/integration/cli/test_cli_advanced_summary_structure.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L14)
- doc: Test cases for advanced CLI options
- signature: `class TestCLIAdvancedOptions:`
- members:
  - `test_advanced_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L123)
  - `test_advanced_option_json_output(self, monkeypatch, sample_java_file)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L17)
  - `test_advanced_option_text_output(self, monkeypatch, sample_java_file)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L51)
  - `test_advanced_option_text_output_strict(self, monkeypatch, sample_java_file)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L81)
  - `test_statistics_option(self, monkeypatch, sample_java_file)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L159)
  - `test_statistics_option_json(self, monkeypatch, sample_java_file)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L191)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

### `TestCLIStructureOption`
- def: [`tests/integration/cli/test_cli_advanced_summary_structure.py:360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L360)
- doc: Test cases for --structure option
- signature: `class TestCLIStructureOption:`
- members:
  - `test_structure_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L427)
  - `test_structure_option_json(self, monkeypatch, sample_java_file)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L363)
  - `test_structure_option_text(self, monkeypatch, sample_java_file)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L396)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

### `TestCLISummaryOption`
- def: [`tests/integration/cli/test_cli_advanced_summary_structure.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L225)
- doc: Test cases for --summary option
- signature: `class TestCLISummaryOption:`
- members:
  - `test_summary_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L323)
  - `test_summary_option_default(self, monkeypatch, sample_java_file)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L228)
  - `test_summary_option_json(self, monkeypatch, sample_java_file)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L289)
  - `test_summary_option_specific_types(self, monkeypatch, sample_java_file)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_advanced_summary_structure.py#L255)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

