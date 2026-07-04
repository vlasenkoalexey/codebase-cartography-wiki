---
title: 'Module: tests/integration/cli/test_cli_table_partial_query.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_table_partial_query.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_table_partial_query`/TestCLI
symbols:
  TestCLITableOption.test_table_option_analysis_failure: TableOption#test_table_option_analysis_failure().
  TestCLITableOption.test_table_option_full: TableOption#test_table_option_full().
  TestCLITableOption.test_table_option_full_strict: TableOption#test_table_option_full_strict().
  TestCLITableOption.test_table_option_compact: TableOption#test_table_option_compact().
  TestCLITableOption.test_table_option_csv: TableOption#test_table_option_csv().
  TestCLIPartialReadOption.test_partial_read_basic: PartialReadOption#test_partial_read_basic().
  TestCLIPartialReadOption.test_partial_read_missing_start_line: PartialReadOption#test_partial_read_missing_start_line().
  TestCLIPartialReadOption.test_partial_read_invalid_start_line: PartialReadOption#test_partial_read_invalid_start_line().
  TestCLIPartialReadOption.test_partial_read_invalid_end_line: PartialReadOption#test_partial_read_invalid_end_line().
  TestCLIPartialReadOption.test_partial_read_invalid_start_column: PartialReadOption#test_partial_read_invalid_start_column().
  TestCLIPartialReadOption.test_partial_read_invalid_end_column: PartialReadOption#test_partial_read_invalid_end_column().
  TestCLIPartialReadOption.test_partial_read_failure: PartialReadOption#test_partial_read_failure().
  TestCLIQueryHandling.test_describe_query_not_found: QueryHandling#test_describe_query_not_found().
  TestCLIQueryHandling.test_describe_query_exception: QueryHandling#test_describe_query_exception().
  TestCLILanguageHandling.test_unsupported_language_fallback: LanguageHandling#test_unsupported_language_fallback().
  TestCLITableOption: TableOption#
  TestCLIPartialReadOption: PartialReadOption#
  TestCLIQueryHandling: QueryHandling#
  TestCLILanguageHandling: LanguageHandling#
---
# Module: [`tests/integration/cli/test_cli_table_partial_query.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py)

## Classes
### `TestCLILanguageHandling`
- def: [`tests/integration/cli/test_cli_table_partial_query.py:351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L351)
- doc: Test cases for language handling
- signature: `class TestCLILanguageHandling:`
- members:
  - `test_unsupported_language_fallback(self, monkeypatch, capsys, sample_java_file)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L354)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIPartialReadOption`
- def: [`tests/integration/cli/test_cli_table_partial_query.py:160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L160)
- doc: Test cases for --partial-read option
- signature: `class TestCLIPartialReadOption:`
- members:
  - `test_partial_read_basic(self, monkeypatch, sample_java_file)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L163)
  - `test_partial_read_failure(self, monkeypatch, sample_java_file)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L295)
  - `test_partial_read_invalid_end_column(self, monkeypatch, sample_java_file)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L272)
  - `test_partial_read_invalid_end_line(self, monkeypatch, sample_java_file)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L224)
  - `test_partial_read_invalid_start_column(self, monkeypatch, sample_java_file)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L249)
  - `test_partial_read_invalid_start_line(self, monkeypatch, sample_java_file)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L209)
  - `test_partial_read_missing_start_line(self, monkeypatch, sample_java_file)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L192)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIQueryHandling`
- def: [`tests/integration/cli/test_cli_table_partial_query.py:316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L316)
- doc: Test cases for query handling
- signature: `class TestCLIQueryHandling:`
- members:
  - `test_describe_query_exception(self, monkeypatch, capsys, sample_java_file)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L334)
  - `test_describe_query_not_found(self, monkeypatch, capsys, sample_java_file)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L319)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLITableOption`
- def: [`tests/integration/cli/test_cli_table_partial_query.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L13)
- doc: Test cases for --table option
- signature: `class TestCLITableOption:`
- members:
  - `test_table_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L123)
  - `test_table_option_compact(self, monkeypatch, sample_java_file)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L79)
  - `test_table_option_csv(self, monkeypatch, sample_java_file)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L105)
  - `test_table_option_full(self, monkeypatch, sample_java_file)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L16)
  - `test_table_option_full_strict(self, monkeypatch, sample_java_file)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_table_partial_query.py#L35)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

