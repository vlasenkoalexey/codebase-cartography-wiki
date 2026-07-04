---
title: 'Module: tests/property/test_query_properties.py'
type: catalog
provenance: extracted
module: tests/property/test_query_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.property.test_query_properties`/
symbols:
  TestQueryProperties.test_statistics_reset: TestQueryProperties#test_statistics_reset().
  TestQueryProperties.test_query_statistics_tracking: TestQueryProperties#test_query_statistics_tracking().
  QueryStatefulMachine.execute_query: QueryStatefulMachine#execute_query().
  QueryStatefulMachine.statistics_consistency: QueryStatefulMachine#statistics_consistency().
  QueryStatefulMachine.query_executor: QueryStatefulMachine#query_executor.
  TestQueryProperties.test_valid_query_names: TestQueryProperties#test_valid_query_names().
  TestQueryProperties.test_query_description_exists: TestQueryProperties#test_query_description_exists().
  TestQueryProperties.test_multiple_queries_execution: TestQueryProperties#test_multiple_queries_execution().
  TestQueryProperties.test_empty_source_code: TestQueryProperties#test_empty_source_code().
  TestQueryProperties.test_query_result_structure: TestQueryProperties#test_query_result_structure().
  TestQueryProperties.test_language_parameter: TestQueryProperties#test_language_parameter().
  TestQueryProperties.test_invalid_query_name: TestQueryProperties#test_invalid_query_name().
  TestQueryProperties.test_query_idempotency: TestQueryProperties#test_query_idempotency().
  TestQueryProperties.test_query_order_independence: TestQueryProperties#test_query_order_independence().
  QueryStatefulMachine.available_queries_unchanged: QueryStatefulMachine#available_queries_unchanged().
  TestQueryEdgeCases.test_very_long_source_code: TestQueryEdgeCases#test_very_long_source_code().
  TestQueryEdgeCases.test_special_characters_in_source: TestQueryEdgeCases#test_special_characters_in_source().
  TestQueryEdgeCases.test_unicode_in_source: TestQueryEdgeCases#test_unicode_in_source().
  TestQueryEdgeCases.test_empty_query_name: TestQueryEdgeCases#test_empty_query_name().
  TestQueryEdgeCases.test_none_query_name: TestQueryEdgeCases#test_none_query_name().
  TestQueryEdgeCases.test_concurrent_queries: TestQueryEdgeCases#test_concurrent_queries().
  TestQueryEdgeCases.execute_concurrent: TestQueryEdgeCases#execute_concurrent().
  QueryStatefulMachine.executed_queries: QueryStatefulMachine#executed_queries.
  QueryStatefulMachine: QueryStatefulMachine#
  TestQueryProperties: TestQueryProperties#
  QueryStatefulMachine.__init__: QueryStatefulMachine#__init__().
  TestQueryEdgeCases: TestQueryEdgeCases#
---
# Module: [`tests/property/test_query_properties.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py)

## Classes
### `QueryStatefulMachine`
- def: [`tests/property/test_query_properties.py:408`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L408)
- doc: 查询状态机测试。
- signature: `class QueryStatefulMachine(RuleBasedStateMachine):`
- members:
  - `available_queries_unchanged(self)` — [`L451`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L451) — 验证可用查询未改变。
  - `execute_query(self, query_name: str)` — [`L417`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L417) — 执行查询。
  - `statistics_consistency(self)` — [`L443`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L443) — 验证统计的一致性。
  - `executed_queries` — [`L414`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L414)
  - `query_executor` — [`L413`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L413)
- protocol/private: `__init__`[`L411`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L411)
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`get_available_queries`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_available_queries), [`get_query_statistics`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_query_statistics)

### `TestQueryEdgeCases`
- def: [`tests/property/test_query_properties.py:461`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L461)
- doc: 查询边界情况测试。
- signature: `class TestQueryEdgeCases:`
- members:
  - `execute_concurrent()` — [`L606`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L606)
  - `test_concurrent_queries(self)` — [`L601`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L601) — 测试并发查询。
  - `test_empty_query_name(self)` — [`L547`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L547) — 测试空查询名称。
  - `test_none_query_name(self)` — [`L573`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L573) — 测试None查询名称。
  - `test_special_characters_in_source(self)` — [`L488`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L488) — 测试源代码中的特殊字符。
  - `test_unicode_in_source(self)` — [`L518`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L518) — 测试源代码中的Unicode字符。
  - `test_very_long_source_code(self)` — [`L464`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L464) — 测试非常长的源代码。
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query)

### `TestQueryProperties`
- def: [`tests/property/test_query_properties.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L15)
- doc: 查询属性测试类。
- signature: `class TestQueryProperties:`
- members:
  - `test_empty_source_code(self, source_code: str)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L98) — 测试空源代码的属性。
  - `test_invalid_query_name(self, query_name: str)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L197) — 测试无效查询名称的属性。
  - `test_language_parameter(self, language: str)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L164) — 测试语言参数的属性。
  - `test_multiple_queries_execution(self, query_names: list[str])` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L58) — 测试多个查询执行的属性。
  - `test_query_description_exists(self, query_name: str)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L36) — 测试查询描述存在的属性。
  - `test_query_idempotency(self, source_code: str)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L233) — 测试查询执行的幂等性。
  - `test_query_order_independence(self, query_names: list[str])` — [`L355`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L355) — 测试查询顺序独立性的属性。
  - `test_query_result_structure(self, query_name: str)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L128) — 测试查询结果结构的属性。
  - `test_query_statistics_tracking(self, query_name: str)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L271) — 测试查询统计跟踪的属性。
  - `test_statistics_reset(self, query_name: str)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L308) — 测试统计重置的属性。
  - `test_valid_query_names(self, query_name: str)` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_properties.py#L20) — 测试有效查询名称的属性。
- uses (calls/refs, reference-scoped): [`QueryExecutor`](../../tree_sitter_analyzer/core/query.md#QueryExecutor), [`execute_query`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_query), [`get_available_queries`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_available_queries), [`get_query_statistics`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_query_statistics), [`get_query_description`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.get_query_description), [`execute_multiple_queries`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.execute_multiple_queries), [`reset_statistics`](../../tree_sitter_analyzer/core/query.md#QueryExecutor.reset_statistics)

