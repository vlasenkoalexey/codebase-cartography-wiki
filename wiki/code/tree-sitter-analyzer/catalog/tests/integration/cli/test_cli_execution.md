---
title: 'Module: tests/integration/cli/test_cli_execution.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_execution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_execution`/
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
  pytestmark: pytestmark.
  TestCLIAdditionalCoverage: TestCLIAdditionalCoverage#
---
# Module: [`tests/integration/cli/test_cli_execution.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py)

## Classes
### `TestCLIAdditionalCoverage`
- def: [`tests/integration/cli/test_cli_execution.py:209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L209)
- doc: Additional test cases to improve CLI coverage
- signature: `class TestCLIAdditionalCoverage:`
- members:
  - `test_describe_query_missing_language_and_file(self, monkeypatch, capsys)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L260) — Test --describe-query without language or file
  - `test_describe_query_with_file(self, monkeypatch, sample_java_file)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L236) — Test --describe-query with file path
  - `test_list_queries_all_languages(self, monkeypatch)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L224) — Test --list-queries without language specification
  - `test_list_queries_with_file(self, monkeypatch, sample_java_file)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L212) — Test --list-queries with file path
  - `test_missing_file_path_error(self, monkeypatch)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L278) — Test error when file path is missing
  - `test_nonexistent_file_error(self, monkeypatch)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L290) — Test error when file does not exist
  - `test_query_string_option(self, monkeypatch, sample_java_file)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L389) — Test --query-string option
  - `test_unknown_language_detection(self, monkeypatch, capsys)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L313) — Test unknown language detection
  - `test_unsupported_language_fallback(self, monkeypatch, sample_java_file)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L356) — Test unsupported language with fallback to Java
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLILoggingConfiguration`
- def: [`tests/integration/cli/test_cli_execution.py:180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L180)
- doc: Test cases for logging configuration
- signature: `class TestCLILoggingConfiguration:`
- members:
  - `test_table_option_logging_suppression(self, monkeypatch, sample_java_file)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L183) — Test that --table option suppresses logging
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

### `TestCLIQueryExecution`
- def: [`tests/integration/cli/test_cli_execution.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L16)
- doc: Test cases for query execution
- signature: `class TestCLIQueryExecution:`
- members:
  - `mock_execute_query(*args, **kwargs)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L42)
  - `mock_get_available_queries(language)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L45)
  - `test_no_query_or_advanced_error(self, monkeypatch, sample_java_file)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L106) — Test error when neither query nor --advanced is specified
  - `test_query_exception_error(self, monkeypatch, sample_java_file)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L149) — Test error when query loading raises exception
  - `test_query_execution_no_results(self, monkeypatch, sample_java_file)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L19) — Test query execution with no results
  - `test_query_execution_parse_failure(self, monkeypatch, sample_java_file)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L68) — Test query execution when parsing fails
  - `test_query_not_found_error(self, monkeypatch, sample_java_file)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L122) — Test error when query is not found
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/cli_main.md#main)

## Module values
- `pytestmark` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_execution.py#L206)

