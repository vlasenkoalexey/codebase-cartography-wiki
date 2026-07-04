---
title: 'Module: tests/integration/cli/test_cli_query_exec_coverage.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_query_exec_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_query_exec_coverage`/
symbols:
  TestCLIQueryExecution.test_query_execution_no_results: TestCLIQueryExecution#test_query_execution_no_results().
  TestCLIQueryExecution.test_query_execution_parse_failure: TestCLIQueryExecution#test_query_execution_parse_failure().
  TestCLIQueryExecution.test_no_query_or_advanced_error: TestCLIQueryExecution#test_no_query_or_advanced_error().
  TestCLIQueryExecution.test_query_not_found_error: TestCLIQueryExecution#test_query_not_found_error().
  TestCLIQueryExecution.test_query_exception_error: TestCLIQueryExecution#test_query_exception_error().
  TestCLILoggingConfiguration.test_table_option_logging_suppression: TestCLILoggingConfiguration#test_table_option_logging_suppression().
  TestCLIAdditionalCoverage.test_list_queries_with_file: TestCLIAdditionalCoverage#test_list_queries_with_file().
  TestCLIAdditionalCoverage.test_list_queries_all_languages: TestCLIAdditionalCoverage#test_list_queries_all_languages().
  TestCLIAdditionalCoverage.test_describe_query_with_file: TestCLIAdditionalCoverage#test_describe_query_with_file().
  TestCLIAdditionalCoverage.test_describe_query_missing_language_and_file: TestCLIAdditionalCoverage#test_describe_query_missing_language_and_file().
  TestCLIAdditionalCoverage.test_missing_file_path_error: TestCLIAdditionalCoverage#test_missing_file_path_error().
  TestCLIAdditionalCoverage.test_nonexistent_file_error: TestCLIAdditionalCoverage#test_nonexistent_file_error().
  TestCLIAdditionalCoverage.test_unknown_language_detection: TestCLIAdditionalCoverage#test_unknown_language_detection().
  TestCLIAdditionalCoverage.test_unsupported_language_fallback: TestCLIAdditionalCoverage#test_unsupported_language_fallback().
  TestCLIAdditionalCoverage.test_query_string_option: TestCLIAdditionalCoverage#test_query_string_option().
  TestCLIQueryExecution.mock_execute_query: TestCLIQueryExecution#mock_execute_query().
  TestCLIQueryExecution.mock_get_available_queries: TestCLIQueryExecution#mock_get_available_queries().
  TestCLIQueryExecution: TestCLIQueryExecution#
  TestCLILoggingConfiguration: TestCLILoggingConfiguration#
  TestCLIAdditionalCoverage: TestCLIAdditionalCoverage#
  pytestmark: pytestmark.
---
# Module: [`tests/integration/cli/test_cli_query_exec_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py)

## Classes
### `TestCLIAdditionalCoverage`
- def: [`tests/integration/cli/test_cli_query_exec_coverage.py:198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L198)
- doc: Additional test cases to improve CLI coverage
- signature: `class TestCLIAdditionalCoverage:`
- members:
  - `test_describe_query_missing_language_and_file(self, monkeypatch, capsys)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L246)
  - `test_describe_query_with_file(self, monkeypatch, sample_java_file)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L223)
  - `test_list_queries_all_languages(self, monkeypatch)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L212)
  - `test_list_queries_with_file(self, monkeypatch, sample_java_file)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L201)
  - `test_missing_file_path_error(self, monkeypatch)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L264)
  - `test_nonexistent_file_error(self, monkeypatch)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L275)
  - `test_query_string_option(self, monkeypatch, sample_java_file)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L368)
  - `test_unknown_language_detection(self, monkeypatch, capsys)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L297)
  - `test_unsupported_language_fallback(self, monkeypatch, capsys, sample_java_file)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L335)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLILoggingConfiguration`
- def: [`tests/integration/cli/test_cli_query_exec_coverage.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L173)
- doc: Test cases for logging configuration
- signature: `class TestCLILoggingConfiguration:`
- members:
  - `test_table_option_logging_suppression(self, monkeypatch, sample_java_file)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L176)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIQueryExecution`
- def: [`tests/integration/cli/test_cli_query_exec_coverage.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L17)
- doc: Test cases for query execution
- signature: `class TestCLIQueryExecution:`
- members:
  - `mock_execute_query(*args, **kwargs)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L41)
  - `mock_get_available_queries(language)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L44)
  - `test_no_query_or_advanced_error(self, monkeypatch, sample_java_file)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L102)
  - `test_query_exception_error(self, monkeypatch, sample_java_file)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L143)
  - `test_query_execution_no_results(self, monkeypatch, sample_java_file)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L20)
  - `test_query_execution_parse_failure(self, monkeypatch, sample_java_file)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L66)
  - `test_query_not_found_error(self, monkeypatch, sample_java_file)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L117)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

## Module values
- `pytestmark` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_exec_coverage.py#L195)

