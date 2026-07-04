---
title: 'Module: tests/unit/core/test_query_executor.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_executor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_executor`/TestQueryExecutor
symbols:
  TestQueryExecutorInit.test_init: Init#test_init().
  TestQueryExecutorExecuteQuery.test_execute_query_success: ExecuteQuery#test_execute_query_success().
  TestQueryExecutorExecuteQuery.test_execute_query_updates_stats: ExecuteQuery#test_execute_query_updates_stats().
  TestQueryExecutorExecuteQueryString.test_execute_query_string_updates_stats: ExecuteQueryString#test_execute_query_string_updates_stats().
  TestQueryExecutorExecuteMultipleQueries.test_execute_multiple_queries: ExecuteMultipleQueries#test_execute_multiple_queries().
  TestQueryExecutorGetQueryStatistics.test_get_query_statistics_after_execution: GetQueryStatistics#test_get_query_statistics_after_execution().
  TestQueryExecutorResetStatistics.test_reset_statistics: ResetStatistics#test_reset_statistics().
  TestQueryExecutorExecuteQuery.test_execute_query_with_none_tree: ExecuteQuery#test_execute_query_with_none_tree().
  TestQueryExecutorExecuteQuery.test_execute_query_with_none_language: ExecuteQuery#test_execute_query_with_none_language().
  TestQueryExecutorExecuteQuery.test_execute_query_query_not_found: ExecuteQuery#test_execute_query_query_not_found().
  TestQueryExecutorExecuteQueryWithLanguageName.test_execute_query_with_language_name_none_tree: ExecuteQueryWithLanguageName#test_execute_query_with_language_name_none_tree().
  TestQueryExecutorExecuteQueryWithLanguageName.test_execute_query_with_language_name_none_language: ExecuteQueryWithLanguageName#test_execute_query_with_language_name_none_language().
  TestQueryExecutorExecuteQueryWithLanguageName.test_execute_query_with_language_name_success: ExecuteQueryWithLanguageName#test_execute_query_with_language_name_success().
  TestQueryExecutorExecuteQueryString.test_execute_query_string_none_tree: ExecuteQueryString#test_execute_query_string_none_tree().
  TestQueryExecutorExecuteQueryString.test_execute_query_string_none_language: ExecuteQueryString#test_execute_query_string_none_language().
  TestQueryExecutorExecuteQueryString.test_execute_query_string_success: ExecuteQueryString#test_execute_query_string_success().
  TestQueryExecutorExecuteMultipleQueries.test_execute_multiple_queries_empty_list: ExecuteMultipleQueries#test_execute_multiple_queries_empty_list().
  TestQueryExecutorProcessCaptures.test_process_captures_tuple_format: ProcessCaptures#test_process_captures_tuple_format().
  TestQueryExecutorProcessCaptures.test_process_captures_dict_format: ProcessCaptures#test_process_captures_dict_format().
  TestQueryExecutorProcessCaptures.test_process_captures_none_node: ProcessCaptures#test_process_captures_none_node().
  TestQueryExecutorProcessCaptures.test_process_captures_multiple: ProcessCaptures#test_process_captures_multiple().
  TestQueryExecutorCreateResultDict.test_create_result_dict: CreateResultDict#test_create_result_dict().
  TestQueryExecutorCreateResultDict.test_create_result_dict_error: CreateResultDict#test_create_result_dict_error().
  TestQueryExecutorCreateErrorResult.test_create_error_result_basic: CreateErrorResult#test_create_error_result_basic().
  TestQueryExecutorCreateErrorResult.test_create_error_result_with_query_name: CreateErrorResult#test_create_error_result_with_query_name().
  TestQueryExecutorCreateErrorResult.test_create_error_result_with_extra_fields: CreateErrorResult#test_create_error_result_with_extra_fields().
  TestQueryExecutorGetAvailableQueries.test_get_available_queries: GetAvailableQueries#test_get_available_queries().
  TestQueryExecutorGetAvailableQueries.test_get_available_queries_empty_language: GetAvailableQueries#test_get_available_queries_empty_language().
  TestQueryExecutorGetQueryDescription.test_get_query_description: GetQueryDescription#test_get_query_description().
  TestQueryExecutorGetQueryDescription.test_get_query_description_nonexistent: GetQueryDescription#test_get_query_description_nonexistent().
  TestQueryExecutorValidateQuery.test_validate_query_success: ValidateQuery#test_validate_query_success().
  TestQueryExecutorValidateQuery.test_validate_query_invalid: ValidateQuery#test_validate_query_invalid().
  TestQueryExecutorGetQueryStatistics.test_get_query_statistics_initial: GetQueryStatistics#test_get_query_statistics_initial().
  TestQueryExecutorInit.test_init_creates_query_loader: Init#test_init_creates_query_loader().
  TestQueryExecutorInit: Init#
  TestQueryExecutorExecuteQuery: ExecuteQuery#
  TestQueryExecutorExecuteQueryWithLanguageName: ExecuteQueryWithLanguageName#
  TestQueryExecutorExecuteQueryString: ExecuteQueryString#
  TestQueryExecutorExecuteMultipleQueries: ExecuteMultipleQueries#
  TestQueryExecutorProcessCaptures: ProcessCaptures#
  TestQueryExecutorCreateResultDict: CreateResultDict#
  TestQueryExecutorCreateErrorResult: CreateErrorResult#
  TestQueryExecutorGetAvailableQueries: GetAvailableQueries#
  TestQueryExecutorGetQueryDescription: GetQueryDescription#
  TestQueryExecutorValidateQuery: ValidateQuery#
  TestQueryExecutorGetQueryStatistics: GetQueryStatistics#
  TestQueryExecutorResetStatistics: ResetStatistics#
---
# Module: [`tests/unit/core/test_query_executor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py)

## Classes
### `TestQueryExecutorCreateErrorResult`
- def: [`tests/unit/core/test_query_executor.py:413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L413)
- doc: _create_error_result方法测试
- signature: `class TestQueryExecutorCreateErrorResult:`
- members:
  - `test_create_error_result_basic(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L416) — 测试创建基本错误结果
  - `test_create_error_result_with_extra_fields(self)` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L434) — 测试创建带额外字段的错误结果
  - `test_create_error_result_with_query_name(self)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L425) — 测试创建带查询名的错误结果
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_create_error_result`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._create_error_result)

### `TestQueryExecutorCreateResultDict`
- def: [`tests/unit/core/test_query_executor.py:370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L370)
- doc: _create_result_dict方法测试
- signature: `class TestQueryExecutorCreateResultDict:`
- members:
  - `test_create_result_dict(self, mock_get_text)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L374) — 测试创建结果字典
  - `test_create_result_dict_error(self, mock_get_text)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L399) — 测试创建结果字典时出错
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_create_result_dict`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._create_result_dict)

### `TestQueryExecutorExecuteMultipleQueries`
- def: [`tests/unit/core/test_query_executor.py:254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L254)
- doc: execute_multiple_queries方法测试
- signature: `class TestQueryExecutorExecuteMultipleQueries:`
- members:
  - `test_execute_multiple_queries(self, mock_compat)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L258) — 测试执行多个查询
  - `test_execute_multiple_queries_empty_list(self, mock_compat)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L280) — 测试执行空查询列表
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_execution_stats`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._execution_stats), [`execute_multiple_queries`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_multiple_queries)

### `TestQueryExecutorExecuteQuery`
- def: [`tests/unit/core/test_query_executor.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L33)
- doc: execute_query方法测试
- signature: `class TestQueryExecutorExecuteQuery:`
- members:
  - `test_execute_query_query_not_found(self, mock_compat)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L88) — 测试查询未找到
  - `test_execute_query_success(self, mock_compat)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L63) — 测试成功执行查询
  - `test_execute_query_updates_stats(self, mock_compat)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L108) — 测试执行查询更新统计信息
  - `test_execute_query_with_none_language(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L49) — 测试language为None时返回错误
  - `test_execute_query_with_none_tree(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L36) — 测试tree为None时返回错误
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`_execution_stats`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._execution_stats)

### `TestQueryExecutorExecuteQueryString`
- def: [`tests/unit/core/test_query_executor.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L185)
- doc: execute_query_string方法测试
- signature: `class TestQueryExecutorExecuteQueryString:`
- members:
  - `test_execute_query_string_none_language(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L200) — 测试language为None时返回错误
  - `test_execute_query_string_none_tree(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L188) — 测试tree为None时返回错误
  - `test_execute_query_string_success(self, mock_compat)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L213) — 测试成功执行查询字符串
  - `test_execute_query_string_updates_stats(self, mock_compat)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L234) — 测试执行查询字符串更新统计信息
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_execution_stats`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._execution_stats), [`execute_query_string`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query_string)

### `TestQueryExecutorExecuteQueryWithLanguageName`
- def: [`tests/unit/core/test_query_executor.py:133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L133)
- doc: execute_query_with_language_name方法测试
- signature: `class TestQueryExecutorExecuteQueryWithLanguageName:`
- members:
  - `test_execute_query_with_language_name_none_language(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L149) — 测试language为None时返回错误
  - `test_execute_query_with_language_name_none_tree(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L136) — 测试tree为None时返回错误
  - `test_execute_query_with_language_name_success(self, mock_compat)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L163) — 测试成功执行查询（带语言名）
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query_with_language_name`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query_with_language_name)

### `TestQueryExecutorGetAvailableQueries`
- def: [`tests/unit/core/test_query_executor.py:447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L447)
- doc: get_available_queries方法测试
- signature: `class TestQueryExecutorGetAvailableQueries:`
- members:
  - `test_get_available_queries(self)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L450) — 测试获取可用查询
  - `test_get_available_queries_empty_language(self)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L458) — 测试空语言获取查询
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`get_available_queries`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_available_queries)

### `TestQueryExecutorGetQueryDescription`
- def: [`tests/unit/core/test_query_executor.py:467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L467)
- doc: get_query_description方法测试
- signature: `class TestQueryExecutorGetQueryDescription:`
- members:
  - `test_get_query_description(self)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L470) — 测试获取查询描述
  - `test_get_query_description_nonexistent(self)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L477) — 测试获取不存在查询的描述
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`get_query_description`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_query_description)

### `TestQueryExecutorGetQueryStatistics`
- def: [`tests/unit/core/test_query_executor.py:516`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L516)
- doc: get_query_statistics方法测试
- signature: `class TestQueryExecutorGetQueryStatistics:`
- members:
  - `test_get_query_statistics_after_execution(self, mock_compat)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L532) — 测试执行后的查询统计信息
  - `test_get_query_statistics_initial(self)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L519) — 测试初始查询统计信息
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`get_query_statistics`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_query_statistics)

### `TestQueryExecutorInit`
- def: [`tests/unit/core/test_query_executor.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L11)
- doc: QueryExecutor初始化测试
- signature: `class TestQueryExecutorInit:`
- members:
  - `test_init(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L14) — 测试QueryExecutor初始化
  - `test_init_creates_query_loader(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L25) — 测试初始化时创建query_loader
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_execution_stats`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._execution_stats), [`_query_loader`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._query_loader)

### `TestQueryExecutorProcessCaptures`
- def: [`tests/unit/core/test_query_executor.py:296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L296)
- doc: _process_captures方法测试
- signature: `class TestQueryExecutorProcessCaptures:`
- members:
  - `test_process_captures_dict_format(self, mock_get_text)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L321) — 测试处理字典格式的captures
  - `test_process_captures_multiple(self, mock_get_text)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L348) — 测试处理多个captures
  - `test_process_captures_none_node(self, mock_get_text)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L337) — 测试处理None节点
  - `test_process_captures_tuple_format(self, mock_get_text)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L300) — 测试处理元组格式的captures
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_process_captures`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._process_captures)

### `TestQueryExecutorResetStatistics`
- def: [`tests/unit/core/test_query_executor.py:563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L563)
- doc: reset_statistics方法测试
- signature: `class TestQueryExecutorResetStatistics:`
- members:
  - `test_reset_statistics(self)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L566) — 测试重置统计信息
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`_execution_stats`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor._execution_stats), [`reset_statistics`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.reset_statistics)

### `TestQueryExecutorValidateQuery`
- def: [`tests/unit/core/test_query_executor.py:485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L485)
- doc: validate_query方法测试
- signature: `class TestQueryExecutorValidateQuery:`
- members:
  - `test_validate_query_invalid(self, mock_loader)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L504) — 测试验证无效查询
  - `test_validate_query_success(self, mock_loader)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_executor.py#L489) — 测试验证查询成功
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`validate_query`](../../../tree_sitter_analyzer/core/query.md#QueryExecutor.validate_query)

