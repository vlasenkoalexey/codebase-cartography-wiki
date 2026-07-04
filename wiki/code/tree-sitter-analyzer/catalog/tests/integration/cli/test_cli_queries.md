---
title: 'Module: tests/integration/cli/test_cli_queries.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_queries.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_queries`/
symbols:
  TestCLITableOption.test_table_option_analysis_failure: TestCLITableOption#test_table_option_analysis_failure().
  TestCLITableOption.test_table_option_full: TestCLITableOption#test_table_option_full().
  TestCLITableOption.test_table_option_full_strict: TestCLITableOption#test_table_option_full_strict().
  TestCLITableOption.test_table_option_compact: TestCLITableOption#test_table_option_compact().
  TestCLITableOption.test_table_option_csv: TestCLITableOption#test_table_option_csv().
  TestCLIPartialReadOption.test_partial_read_basic: TestCLIPartialReadOption#test_partial_read_basic().
  TestCLIPartialReadOption.test_partial_read_missing_start_line: TestCLIPartialReadOption#test_partial_read_missing_start_line().
  TestCLIPartialReadOption.test_partial_read_invalid_start_line: TestCLIPartialReadOption#test_partial_read_invalid_start_line().
  TestCLIPartialReadOption.test_partial_read_invalid_end_line: TestCLIPartialReadOption#test_partial_read_invalid_end_line().
  TestCLIPartialReadOption.test_partial_read_invalid_start_column: TestCLIPartialReadOption#test_partial_read_invalid_start_column().
  TestCLIPartialReadOption.test_partial_read_invalid_end_column: TestCLIPartialReadOption#test_partial_read_invalid_end_column().
  TestCLIPartialReadOption.test_partial_read_failure: TestCLIPartialReadOption#test_partial_read_failure().
  TestCLIQueryHandling.test_describe_query_not_found: TestCLIQueryHandling#test_describe_query_not_found().
  TestCLIQueryHandling.test_describe_query_exception: TestCLIQueryHandling#test_describe_query_exception().
  TestCLILanguageHandling.test_unsupported_language_fallback: TestCLILanguageHandling#test_unsupported_language_fallback().
  sample_java_file: sample_java_file().
  TestCLITableOption: TestCLITableOption#
  TestCLIPartialReadOption: TestCLIPartialReadOption#
  TestCLIQueryHandling: TestCLIQueryHandling#
  TestCLILanguageHandling: TestCLILanguageHandling#
---
# Module: [`tests/integration/cli/test_cli_queries.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py)

## Classes
### `TestCLILanguageHandling`
- def: [`tests/integration/cli/test_cli_queries.py:425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L425)
- doc: Test cases for language handling
- signature: `class TestCLILanguageHandling:`
- members:
  - `test_unsupported_language_fallback(self, monkeypatch, sample_java_file)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L428) — Test unsupported language handling.
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIPartialReadOption`
- def: [`tests/integration/cli/test_cli_queries.py:215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L215)
- doc: Test cases for --partial-read option
- signature: `class TestCLIPartialReadOption:`
- members:
  - `test_partial_read_basic(self, monkeypatch, sample_java_file)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L218) — Test --partial-read option with basic parameters
  - `test_partial_read_failure(self, monkeypatch, sample_java_file)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L356) — Test --partial-read option when reading fails
  - `test_partial_read_invalid_end_column(self, monkeypatch, sample_java_file)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L332) — Test --partial-read option with invalid end column
  - `test_partial_read_invalid_end_line(self, monkeypatch, sample_java_file)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L282) — Test --partial-read option with invalid end line
  - `test_partial_read_invalid_start_column(self, monkeypatch, sample_java_file)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L308) — Test --partial-read option with invalid start column
  - `test_partial_read_invalid_start_line(self, monkeypatch, sample_java_file)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L266) — Test --partial-read option with invalid start line
  - `test_partial_read_missing_start_line(self, monkeypatch, sample_java_file)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L248) — Test --partial-read option without required --start-line
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIQueryHandling`
- def: [`tests/integration/cli/test_cli_queries.py:378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L378)
- doc: Test cases for query handling
- signature: `class TestCLIQueryHandling:`
- members:
  - `test_describe_query_exception(self, monkeypatch, sample_java_file)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L401) — Test --describe-query with exception
  - `test_describe_query_not_found(self, monkeypatch, sample_java_file)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L381) — Test --describe-query with non-existent query
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLITableOption`
- def: [`tests/integration/cli/test_cli_queries.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L58)
- doc: Test cases for --table option
- signature: `class TestCLITableOption:`
- members:
  - `test_table_option_analysis_failure(self, monkeypatch, sample_java_file)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L175) — Test --table option when analysis fails
  - `test_table_option_compact(self, monkeypatch, sample_java_file)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L130) — Test --table option with compact format
  - `test_table_option_csv(self, monkeypatch, sample_java_file)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L156) — Test --table option with CSV format
  - `test_table_option_full(self, monkeypatch, sample_java_file)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L61) — Test --table option with full format
  - `test_table_option_full_strict(self, monkeypatch, sample_java_file)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L81) — Test --table option with strict content validation
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`main`](../../../tree_sitter_analyzer/cli_main.md#main), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results)

## Functions
- `sample_java_file()` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_queries.py#L17) — Fixture providing a temporary Java file for testing

