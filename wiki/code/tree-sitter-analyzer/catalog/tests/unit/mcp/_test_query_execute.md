---
title: 'Module: tests/unit/mcp/_test_query_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/_test_query_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp._test_query_execute`/TestExecute
symbols:
  TestExecuteTestMixin: TestMixin#
  TestExecuteAdditionalCoverageTestMixin: AdditionalCoverageTestMixin#
  TestExecuteCoverageBoostTestMixin: CoverageBoostTestMixin#
  TestExecuteInvalidQueryKeyTestMixin: InvalidQueryKeyTestMixin#
  TestExecuteAdditionalCoverageTestMixin.test_execute_analysis_error_reraise: AdditionalCoverageTestMixin#test_execute_analysis_error_reraise().
  TestExecuteInvalidQueryKeyTestMixin.test_execute_no_results_with_productive_queries: InvalidQueryKeyTestMixin#test_execute_no_results_with_productive_queries().
  TestExecuteInvalidQueryKeyTestMixin.test_execute_no_results_productive_queries_exception: InvalidQueryKeyTestMixin#test_execute_no_results_productive_queries_exception().
  TestExecuteInvalidQueryKeyTestMixin.mock_execute_query: InvalidQueryKeyTestMixin#mock_execute_query().
  TestExecuteTestMixin.test_execute_empty_arguments: TestMixin#test_execute_empty_arguments().
  TestExecuteTestMixin.test_execute_missing_file_path: TestMixin#test_execute_missing_file_path().
  TestExecuteTestMixin.test_execute_missing_both_query_params: TestMixin#test_execute_missing_both_query_params().
  TestExecuteTestMixin.test_execute_both_query_params_provided: TestMixin#test_execute_both_query_params_provided().
  TestExecuteTestMixin.test_execute_language_detection_fails: TestMixin#test_execute_language_detection_fails().
  TestExecuteTestMixin.test_execute_success_with_query_key: TestMixin#test_execute_success_with_query_key().
  TestExecuteTestMixin.test_execute_success_with_query_string: TestMixin#test_execute_success_with_query_string().
  TestExecuteTestMixin.test_execute_no_results: TestMixin#test_execute_no_results().
  TestExecuteTestMixin.test_execute_with_summary_format: TestMixin#test_execute_with_summary_format().
  TestExecuteTestMixin.test_execute_with_file_output: TestMixin#test_execute_with_file_output().
  TestExecuteTestMixin.test_execute_with_suppress_output: TestMixin#test_execute_with_suppress_output().
  TestExecuteTestMixin.test_execute_with_toon_format: TestMixin#test_execute_with_toon_format().
  TestExecuteTestMixin.test_execute_exception_handling: TestMixin#test_execute_exception_handling().
  TestExecuteTestMixin.test_execute_file_save_error: TestMixin#test_execute_file_save_error().
  TestExecuteTestMixin.test_execute_auto_language_detection: TestMixin#test_execute_auto_language_detection().
  TestExecuteTestMixin.test_execute_suppress_output_with_file_save_error: TestMixin#test_execute_suppress_output_with_file_save_error().
  TestExecuteTestMixin.test_execute_with_empty_output_file_string: TestMixin#test_execute_with_empty_output_file_string().
  TestExecuteTestMixin.test_execute_with_query_string_and_file_output: TestMixin#test_execute_with_query_string_and_file_output().
  TestExecuteAdditionalCoverageTestMixin.test_execute_none_arguments: AdditionalCoverageTestMixin#test_execute_none_arguments().
  TestExecuteAdditionalCoverageTestMixin.test_execute_summary_format_with_file_output: AdditionalCoverageTestMixin#test_execute_summary_format_with_file_output().
  TestExecuteAdditionalCoverageTestMixin.test_execute_summary_format_file_save_error: AdditionalCoverageTestMixin#test_execute_summary_format_file_save_error().
  TestExecuteAdditionalCoverageTestMixin.test_execute_suppress_output_with_file_save_info: AdditionalCoverageTestMixin#test_execute_suppress_output_with_file_save_info().
  TestExecuteAdditionalCoverageTestMixin.test_execute_suppress_output_with_save_error_info: AdditionalCoverageTestMixin#test_execute_suppress_output_with_save_error_info().
  TestExecuteAdditionalCoverageTestMixin.test_execute_with_output_format_json: AdditionalCoverageTestMixin#test_execute_with_output_format_json().
  TestExecuteAdditionalCoverageTestMixin.test_execute_no_language_provided_auto_detect: AdditionalCoverageTestMixin#test_execute_no_language_provided_auto_detect().
  TestExecuteCoverageBoostTestMixin.test_execute_generic_exception_returns_error: CoverageBoostTestMixin#test_execute_generic_exception_returns_error().
  TestExecuteCoverageBoostTestMixin.test_execute_suppress_output_without_file_save: CoverageBoostTestMixin#test_execute_suppress_output_without_file_save().
  TestExecuteCoverageBoostTestMixin.test_execute_file_output_with_toon_format: CoverageBoostTestMixin#test_execute_file_output_with_toon_format().
  TestExecuteCoverageBoostTestMixin.test_execute_empty_arguments_dict_triggers_error: CoverageBoostTestMixin#test_execute_empty_arguments_dict_triggers_error().
  TestExecuteCoverageBoostTestMixin.test_execute_none_file_path_triggers_error: CoverageBoostTestMixin#test_execute_none_file_path_triggers_error().
  TestExecuteInvalidQueryKeyTestMixin.test_execute_invalid_query_key_returns_suggestions: InvalidQueryKeyTestMixin#test_execute_invalid_query_key_returns_suggestions().
  TestExecuteInvalidQueryKeyTestMixin.test_execute_no_results_with_query_string: InvalidQueryKeyTestMixin#test_execute_no_results_with_query_string().
  TestExecuteInvalidQueryKeyTestMixin.test_execute_suppress_output_without_output_file: InvalidQueryKeyTestMixin#test_execute_suppress_output_without_output_file().
---
# Module: [`tests/unit/mcp/_test_query_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py)

## Classes
### `TestExecuteAdditionalCoverageTestMixin`
- def: [`tests/unit/mcp/_test_query_execute.py:362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L362)
- doc: Additional tests targeting uncovered branches in execute.
- signature: `class TestExecuteAdditionalCoverageTestMixin:`
- members:
  - `test_execute_analysis_error_reraise(self, tool, sample_python_file)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L477)
  - `test_execute_no_language_provided_auto_detect(self, tool, sample_python_file, mock_query_results)` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L515)
  - `test_execute_none_arguments(self, tool)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L366)
  - `test_execute_summary_format_file_save_error(self, tool, sample_python_file, mock_query_results)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L397)
  - `test_execute_summary_format_with_file_output(self, tool, sample_python_file, mock_query_results)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L371)
  - `test_execute_suppress_output_with_file_save_info(self, tool, sample_python_file, mock_query_results)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L423)
  - `test_execute_suppress_output_with_save_error_info(self, tool, sample_python_file, mock_query_results)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L450)
  - `test_execute_with_output_format_json(self, tool, sample_python_file, mock_query_results)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L493)
- uses (calls/refs, reference-scoped): [`AnalysisError`](../../../tree_sitter_analyzer/mcp/utils/error_handler.md#AnalysisError)  (1 test-only)
- used by: (1 test-only callers)

### `TestExecuteCoverageBoostTestMixin`
- def: [`tests/unit/mcp/_test_query_execute.py:539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L539)
- doc: Tests targeting specific uncovered lines in execute().
- signature: `class TestExecuteCoverageBoostTestMixin:`
- members:
  - `test_execute_empty_arguments_dict_triggers_error(self, tool)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L616)
  - `test_execute_file_output_with_toon_format(self, tool, sample_python_file, mock_query_results)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L590)
  - `test_execute_generic_exception_returns_error(self, tool, sample_python_file)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L543)
  - `test_execute_none_file_path_triggers_error(self, tool)` — [`L621`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L621)
  - `test_execute_suppress_output_without_file_save(self, tool, sample_python_file, mock_query_results)` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L563)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExecuteInvalidQueryKeyTestMixin`
- def: [`tests/unit/mcp/_test_query_execute.py:626`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L626)
- doc: Tests for execute with invalid query_key.
- signature: `class TestExecuteInvalidQueryKeyTestMixin:`
- members:
  - `mock_execute_query(*args, **kwargs)` — [`L656`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L656)
  - `test_execute_invalid_query_key_returns_suggestions(self, tool, sample_python_file)` — [`L630`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L630)
  - `test_execute_no_results_productive_queries_exception(self, tool, sample_python_file)` — [`L689`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L689)
  - `test_execute_no_results_with_productive_queries(self, tool, sample_python_file)` — [`L651`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L651)
  - `test_execute_no_results_with_query_string(self, tool, sample_python_file)` — [`L717`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L717)
  - `test_execute_suppress_output_without_output_file(self, tool, sample_python_file, mock_query_results)` — [`L739`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L739)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExecuteTestMixin`
- def: [`tests/unit/mcp/_test_query_execute.py:8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L8)
- doc: Tests for execute method.
- signature: `class TestExecuteTestMixin:`
- members:
  - `test_execute_auto_language_detection(self, tool, sample_python_file, mock_query_results)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L264)
  - `test_execute_both_query_params_provided(self, tool, sample_python_file)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L31)
  - `test_execute_empty_arguments(self, tool)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L12)
  - `test_execute_exception_handling(self, tool, sample_python_file)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L221)
  - `test_execute_file_save_error(self, tool, sample_python_file, mock_query_results)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L239)
  - `test_execute_language_detection_fails(self, tool, sample_python_file)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L42)
  - `test_execute_missing_both_query_params(self, tool)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L23)
  - `test_execute_missing_file_path(self, tool)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L17)
  - `test_execute_no_results(self, tool, sample_python_file)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L100)
  - `test_execute_success_with_query_key(self, tool, sample_python_file, mock_query_results)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L56)
  - `test_execute_success_with_query_string(self, tool, sample_python_file, mock_query_results)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L80)
  - `test_execute_suppress_output_with_file_save_error(self, tool, sample_python_file, mock_query_results)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L287)
  - `test_execute_with_empty_output_file_string(self, tool, sample_python_file, mock_query_results)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L313)
  - `test_execute_with_file_output(self, tool, sample_python_file, mock_query_results)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L143)
  - `test_execute_with_query_string_and_file_output(self, tool, sample_python_file, mock_query_results)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L338)
  - `test_execute_with_summary_format(self, tool, sample_python_file, mock_query_results)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L119)
  - `test_execute_with_suppress_output(self, tool, sample_python_file, mock_query_results)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L169)
  - `test_execute_with_toon_format(self, tool, sample_python_file, mock_query_results)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_execute.py#L195)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

