---
title: 'Module: tests/regression/test_api_regression.py'
type: catalog
provenance: extracted
module: tests/regression/test_api_regression.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.regression.test_api_regression`/TestAPI
symbols:
  TestAPIMigration.test_old_api_still_works: Migration#test_old_api_still_works().
  TestAPIBackwardCompatibility.test_analysis_request_from_mcp_arguments_compatibility: BackwardCompatibility#test_analysis_request_from_mcp_arguments_compatibility().
  TestAPIParameterCompatibility.test_analysis_request_boolean_parameters: ParameterCompatibility#test_analysis_request_boolean_parameters().
  TestAPIBackwardCompatibility.test_analysis_request_backward_compatibility: BackwardCompatibility#test_analysis_request_backward_compatibility().
  TestAPIBackwardCompatibility.test_analysis_request_new_parameters_compatibility: BackwardCompatibility#test_analysis_request_new_parameters_compatibility().
  TestAPIParameterCompatibility.test_analysis_request_parameter_types: ParameterCompatibility#test_analysis_request_parameter_types().
  TestAPIStatistics.test_query_executor_reset_statistics: Statistics#test_query_executor_reset_statistics().
  TestAPIMigration.test_new_api_features: Migration#test_new_api_features().
  TestAPIParameterCompatibility.test_analysis_request_format_type_variations: ParameterCompatibility#test_analysis_request_format_type_variations().
  TestAPIParameterCompatibility.test_query_executor_parameter_types: ParameterCompatibility#test_query_executor_parameter_types().
  TestAPIParameterCompatibility.test_query_executor_query_name_parameter: ParameterCompatibility#test_query_executor_query_name_parameter().
  TestAPIParameterCompatibility.test_query_executor_source_code_parameter: ParameterCompatibility#test_query_executor_source_code_parameter().
  TestAPIStatistics.test_query_executor_statistics_structure: Statistics#test_query_executor_statistics_structure().
  TestAPIStatistics.test_query_executor_statistics_initial_values: Statistics#test_query_executor_statistics_initial_values().
  TestAPIBackwardCompatibility.test_query_executor_backward_compatibility: BackwardCompatibility#test_query_executor_backward_compatibility().
  TestAPIBackwardCompatibility: BackwardCompatibility#
  TestAPIParameterCompatibility: ParameterCompatibility#
  TestAPIResponseFormat: ResponseFormat#
  TestAPIResponseFormat.test_analysis_response_structure: ResponseFormat#test_analysis_response_structure().
  TestAPIResponseFormat.test_query_response_structure: ResponseFormat#test_query_response_structure().
  TestAPIResponseFormat.test_error_response_structure: ResponseFormat#test_error_response_structure().
  TestAPIStatistics: Statistics#
  TestAPIMigration: Migration#
---
# Module: [`tests/regression/test_api_regression.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py)

## Classes
### `TestAPIBackwardCompatibility`
- def: [`tests/regression/test_api_regression.py:14`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L14)
- doc: API向后兼容性测试
- signature: `class TestAPIBackwardCompatibility:`
- members:
  - `test_analysis_request_backward_compatibility(self)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L18) — 测试AnalysisRequest向后兼容性
  - `test_analysis_request_from_mcp_arguments_compatibility(self)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L35) — 测试from_mcp_arguments方法兼容性
  - `test_analysis_request_new_parameters_compatibility(self)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L56) — 测试新增参数的兼容性
  - `test_query_executor_backward_compatibility(self)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L74) — 测试QueryExecutor向后兼容性
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`language`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`format_type`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`include_queries`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`include_elements`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements), [`from_mcp_arguments`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.from_mcp_arguments)

### `TestAPIMigration`
- def: [`tests/regression/test_api_regression.py:327`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L327)
- doc: API迁移测试
- signature: `class TestAPIMigration:`
- members:
  - `test_new_api_features(self)` — [`L354`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L354) — 测试新API特性
  - `test_old_api_still_works(self)` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L331) — 测试旧API仍然工作
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`format_type`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`include_queries`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`include_elements`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements), [`from_mcp_arguments`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.from_mcp_arguments)

### `TestAPIParameterCompatibility`
- def: [`tests/regression/test_api_regression.py:89`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L89)
- doc: API参数兼容性测试
- signature: `class TestAPIParameterCompatibility:`
- members:
  - `test_analysis_request_boolean_parameters(self)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L112) — 测试布尔参数兼容性
  - `test_analysis_request_format_type_variations(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L137) — 测试format_type参数变化
  - `test_analysis_request_parameter_types(self)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L93) — 测试AnalysisRequest参数类型兼容性
  - `test_query_executor_parameter_types(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L146) — 测试QueryExecutor参数类型兼容性
  - `test_query_executor_query_name_parameter(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L167) — 测试query_name参数兼容性
  - `test_query_executor_source_code_parameter(self)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L190) — 测试source_code参数兼容性
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`language`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`execute_query`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`format_type`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`include_queries`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`queries`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.queries), [`include_elements`](../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements)

### `TestAPIResponseFormat`
- def: [`tests/regression/test_api_regression.py:215`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L215)
- doc: API响应格式测试
- signature: `class TestAPIResponseFormat:`
- members:
  - `test_analysis_response_structure(self)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L219) — 测试分析响应结构
  - `test_error_response_structure(self)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L258) — 测试错误响应结构
  - `test_query_response_structure(self)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L241) — 测试查询响应结构

### `TestAPIStatistics`
- def: [`tests/regression/test_api_regression.py:272`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L272)
- doc: API统计功能测试
- signature: `class TestAPIStatistics:`
- members:
  - `test_query_executor_reset_statistics(self)` — [`L306`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L306) — 测试重置统计功能
  - `test_query_executor_statistics_initial_values(self)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L291) — 测试统计初始值
  - `test_query_executor_statistics_structure(self)` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_api_regression.py#L276) — 测试查询执行统计结构
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_execution_stats`](../../tree_sitter_analyzer/core/query.md#QueryExecutor._execution_stats), [`get_query_statistics`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_query_statistics), [`reset_statistics`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.reset_statistics)

