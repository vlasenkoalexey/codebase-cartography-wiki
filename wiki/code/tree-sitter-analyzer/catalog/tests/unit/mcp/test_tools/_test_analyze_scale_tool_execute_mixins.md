---
title: 'Module: tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools._test_analyze_scale_tool_execute_mixins`/AnalyzeScaleTool
symbols:
  AnalyzeScaleToolExecuteMixin: ExecuteMixin#
  AnalyzeScaleToolExecuteMetricsBatchMixin: ExecuteMetricsBatchMixin#
  AnalyzeScaleToolCreateJsonFileAnalysisMixin: CreateJsonFileAnalysisMixin#
  AnalyzeScaleToolExecuteJavaMixin: ExecuteJavaMixin#
  AnalyzeScaleToolExecuteBatchAdvancedMixin: ExecuteBatchAdvancedMixin#
  AnalyzeScaleToolExecuteMixin.test_execute_missing_file_path: ExecuteMixin#test_execute_missing_file_path().
  AnalyzeScaleToolExecuteMixin.test_execute_file_not_found: ExecuteMixin#test_execute_file_not_found().
  AnalyzeScaleToolExecuteMixin.test_execute_unsupported_language: ExecuteMixin#test_execute_unsupported_language().
  AnalyzeScaleToolExecuteMixin.test_execute_json_file: ExecuteMixin#test_execute_json_file().
  AnalyzeScaleToolExecuteMixin.test_execute_success_python: ExecuteMixin#test_execute_success_python().
  AnalyzeScaleToolExecuteMixin.test_execute_with_include_details: ExecuteMixin#test_execute_with_include_details().
  AnalyzeScaleToolExecuteMixin.test_execute_without_include_guidance: ExecuteMixin#test_execute_without_include_guidance().
  AnalyzeScaleToolExecuteMixin.test_execute_with_json_output_format: ExecuteMixin#test_execute_with_json_output_format().
  AnalyzeScaleToolExecuteMixin.test_execute_analysis_failure: ExecuteMixin#test_execute_analysis_failure().
  AnalyzeScaleToolExecuteMetricsBatchMixin.test_execute_batch_missing_metrics_only: ExecuteMetricsBatchMixin#test_execute_batch_missing_metrics_only().
  AnalyzeScaleToolExecuteMetricsBatchMixin.test_execute_batch_empty_file_paths: ExecuteMetricsBatchMixin#test_execute_batch_empty_file_paths().
  AnalyzeScaleToolExecuteMetricsBatchMixin.test_execute_batch_invalid_file_paths_type: ExecuteMetricsBatchMixin#test_execute_batch_invalid_file_paths_type().
  AnalyzeScaleToolExecuteMetricsBatchMixin.test_execute_batch_too_many_files: ExecuteMetricsBatchMixin#test_execute_batch_too_many_files().
  AnalyzeScaleToolExecuteMetricsBatchMixin.test_execute_batch_success: ExecuteMetricsBatchMixin#test_execute_batch_success().
  AnalyzeScaleToolExecuteMetricsBatchMixin.test_execute_batch_with_errors: ExecuteMetricsBatchMixin#test_execute_batch_with_errors().
  AnalyzeScaleToolExecuteMetricsBatchMixin.test_execute_batch_file_not_found: ExecuteMetricsBatchMixin#test_execute_batch_file_not_found().
  AnalyzeScaleToolCreateJsonFileAnalysisMixin.test_create_json_file_analysis_small: CreateJsonFileAnalysisMixin#test_create_json_file_analysis_small().
  AnalyzeScaleToolCreateJsonFileAnalysisMixin.test_create_json_file_analysis_medium: CreateJsonFileAnalysisMixin#test_create_json_file_analysis_medium().
  AnalyzeScaleToolCreateJsonFileAnalysisMixin.test_create_json_file_analysis_large: CreateJsonFileAnalysisMixin#test_create_json_file_analysis_large().
  AnalyzeScaleToolCreateJsonFileAnalysisMixin.test_create_json_file_analysis_without_guidance: CreateJsonFileAnalysisMixin#test_create_json_file_analysis_without_guidance().
  AnalyzeScaleToolCreateJsonFileAnalysisMixin.test_create_json_file_analysis_json_format: CreateJsonFileAnalysisMixin#test_create_json_file_analysis_json_format().
  AnalyzeScaleToolExecuteJavaMixin.test_execute_java_success: ExecuteJavaMixin#test_execute_java_success().
  AnalyzeScaleToolExecuteJavaMixin.test_execute_java_analysis_none: ExecuteJavaMixin#test_execute_java_analysis_none().
  AnalyzeScaleToolExecuteJavaMixin.test_execute_non_java_universal_failure: ExecuteJavaMixin#test_execute_non_java_universal_failure().
  AnalyzeScaleToolExecuteBatchAdvancedMixin.test_execute_batch_with_invalid_path_entries: ExecuteBatchAdvancedMixin#test_execute_batch_with_invalid_path_entries().
  AnalyzeScaleToolExecuteBatchAdvancedMixin.test_execute_batch_with_resolve_error: ExecuteBatchAdvancedMixin#test_execute_batch_with_resolve_error().
  AnalyzeScaleToolExecuteBatchAdvancedMixin.test_execute_batch_unknown_language: ExecuteBatchAdvancedMixin#test_execute_batch_unknown_language().
  AnalyzeScaleToolExecuteBatchAdvancedMixin.test_execute_batch_all_errors: ExecuteBatchAdvancedMixin#test_execute_batch_all_errors().
---
# Module: [`tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py)

## Classes
### `AnalyzeScaleToolCreateJsonFileAnalysisMixin`
- def: [`tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py:427`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L427)
- doc: Tests for _create_json_file_analysis method.
- signature: `class AnalyzeScaleToolCreateJsonFileAnalysisMixin:`
- members:
  - `test_create_json_file_analysis_json_format(self, tool)` — [`L506`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L506) — Test JSON file analysis with JSON output format.
  - `test_create_json_file_analysis_large(self, tool)` — [`L468`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L468) — Test JSON file analysis for large file.
  - `test_create_json_file_analysis_medium(self, tool)` — [`L449`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L449) — Test JSON file analysis for medium file.
  - `test_create_json_file_analysis_small(self, tool)` — [`L430`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L430) — Test JSON file analysis for small file.
  - `test_create_json_file_analysis_without_guidance(self, tool)` — [`L487`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L487) — Test JSON file analysis without guidance.
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `AnalyzeScaleToolExecuteBatchAdvancedMixin`
- def: [`tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py:695`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L695)
- doc: Advanced tests for _execute_metrics_batch method.
- signature: `class AnalyzeScaleToolExecuteBatchAdvancedMixin:`
- members:
  - `test_execute_batch_all_errors(self, tool)` — [`L784`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L784) — Test batch mode where all files fail.
  - `test_execute_batch_unknown_language(self, tool)` — [`L751`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L751) — Test batch mode handles unknown language detection.
  - `test_execute_batch_with_invalid_path_entries(self, tool)` — [`L699`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L699) — Test batch mode with invalid file path strings.
  - `test_execute_batch_with_resolve_error(self, tool)` — [`L732`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L732) — Test batch mode handles resolve error.
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `AnalyzeScaleToolExecuteJavaMixin`
- def: [`tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py:526`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L526)
- doc: Tests for execute method with Java language path.
- signature: `class AnalyzeScaleToolExecuteJavaMixin:`
- members:
  - `test_execute_java_analysis_none(self, tool)` — [`L630`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L630) — Test execute handles None result from Java analysis.
  - `test_execute_java_success(self, tool)` — [`L530`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L530) — Test execute succeeds for Java file.
  - `test_execute_non_java_universal_failure(self, tool)` — [`L661`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L661) — Test execute handles universal engine failure.
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `AnalyzeScaleToolExecuteMetricsBatchMixin`
- def: [`tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py:309`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L309)
- doc: Tests for _execute_metrics_batch method.
- signature: `class AnalyzeScaleToolExecuteMetricsBatchMixin:`
- members:
  - `test_execute_batch_empty_file_paths(self, tool)` — [`L320`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L320) — Test batch mode fails when file_paths is empty.
  - `test_execute_batch_file_not_found(self, tool)` — [`L410`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L410) — Test batch mode handles file not found.
  - `test_execute_batch_invalid_file_paths_type(self, tool)` — [`L327`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L327) — Test batch mode fails when file_paths is not a list.
  - `test_execute_batch_missing_metrics_only(self, tool)` — [`L313`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L313) — Test batch mode fails when metrics_only is False.
  - `test_execute_batch_success(self, tool)` — [`L344`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L344) — Test batch mode succeeds.
  - `test_execute_batch_too_many_files(self, tool)` — [`L334`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L334) — Test batch mode fails when too many files.
  - `test_execute_batch_with_errors(self, tool)` — [`L377`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L377) — Test batch mode handles errors gracefully.
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `AnalyzeScaleToolExecuteMixin`
- def: [`tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py:12`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L12)
- doc: Tests for execute method (single mode).
- signature: `class AnalyzeScaleToolExecuteMixin:`
- members:
  - `test_execute_analysis_failure(self, tool)` — [`L274`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L274) — Test execute handles analysis engine failure.
  - `test_execute_file_not_found(self, tool)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L23) — Test execute fails when file doesn't exist.
  - `test_execute_json_file(self, tool)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L53) — Test execute handles JSON files specially.
  - `test_execute_missing_file_path(self, tool)` — [`L16`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L16) — Test execute fails when file_path is missing.
  - `test_execute_success_python(self, tool)` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L86) — Test execute succeeds for Python file.
  - `test_execute_unsupported_language(self, tool)` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L36) — Test execute fails when language is not supported.
  - `test_execute_with_include_details(self, tool)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L133) — Test execute with include_details=True.
  - `test_execute_with_json_output_format(self, tool)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L227) — Test execute with output_format='json'.
  - `test_execute_without_include_guidance(self, tool)` — [`L180`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_analyze_scale_tool_execute_mixins.py#L180) — Test execute with include_guidance=False.
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

