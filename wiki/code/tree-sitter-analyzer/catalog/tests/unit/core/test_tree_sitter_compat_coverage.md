---
title: 'Module: tests/unit/core/test_tree_sitter_compat_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_tree_sitter_compat_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_tree_sitter_compat_coverage`/TestTreeSitterCompatCoverage#
symbols:
  TestTreeSitterCompatCoverage.test_execute_query_old_api_callable: test_execute_query_old_api_callable().
  TestTreeSitterCompatCoverage.test_execute_query_old_api_callable_named_tuple: test_execute_query_old_api_callable_named_tuple().
  TestTreeSitterCompatCoverage.test_execute_old_api_exception_handling: test_execute_old_api_exception_handling().
  TestTreeSitterCompatCoverage.test_execute_old_api_with_invalid_result_items: test_execute_old_api_with_invalid_result_items().
  TestTreeSitterCompatCoverage.test_execute_old_api_non_callable_warning: test_execute_old_api_non_callable_warning().
  TestTreeSitterCompatCoverage.test_execute_query_newest_api: test_execute_query_newest_api().
  TestTreeSitterCompatCoverage.test_execute_query_modern_api: test_execute_query_modern_api().
  TestTreeSitterCompatCoverage.test_execute_query_legacy_api: test_execute_query_legacy_api().
  TestTreeSitterCompatCoverage.test_execute_query_no_compatible_api: test_execute_query_no_compatible_api().
  TestTreeSitterCompatCoverage.test_execute_query_exception: test_execute_query_exception().
  TestTreeSitterCompatCoverage.test_safe_execute_query: test_safe_execute_query().
  TestTreeSitterCompatCoverage.test_log_api_info_import_error: test_log_api_info_import_error().
  TestTreeSitterCompatCoverage.test_log_api_info_api_detection_exception_via_dir: test_log_api_info_api_detection_exception_via_dir().
  TestTreeSitterCompatCoverage.test_execute_modern_api_exception_raises: test_execute_modern_api_exception_raises().
  TestTreeSitterCompatCoverage.test_execute_legacy_api_exception_raises: test_execute_legacy_api_exception_raises().
  TestTreeSitterCompatCoverage.test_create_query_safely: test_create_query_safely().
  TestTreeSitterCompatCoverage.test_get_node_text_safe_byte_range: test_get_node_text_safe_byte_range().
  TestTreeSitterCompatCoverage.test_get_node_text_safe_text_attr_bytes: test_get_node_text_safe_text_attr_bytes().
  TestTreeSitterCompatCoverage.test_get_node_text_safe_text_attr_str: test_get_node_text_safe_text_attr_str().
  TestTreeSitterCompatCoverage.test_get_node_text_safe_points_single_line: test_get_node_text_safe_points_single_line().
  TestTreeSitterCompatCoverage.test_get_node_text_safe_points_multi_line: test_get_node_text_safe_points_multi_line().
  TestTreeSitterCompatCoverage.test_get_node_text_safe_fallback_empty: test_get_node_text_safe_fallback_empty().
  TestTreeSitterCompatCoverage.test_log_api_info: test_log_api_info().
  TestTreeSitterCompatCoverage.test_log_api_info_api_detection_exception: test_log_api_info_api_detection_exception().
  TestTreeSitterCompatCoverage.test_execute_query_old_api_callable.MockQuery: test_execute_query_old_api_callable().MockQuery#
  TestTreeSitterCompatCoverage.test_execute_query_old_api_callable_named_tuple.MockQuery: test_execute_query_old_api_callable_named_tuple().MockQuery#
  TestTreeSitterCompatCoverage.mock_import: mock_import().
  TestTreeSitterCompatCoverage.test_log_api_info_api_detection_exception_via_dir.QueryThatFailsOnDir: test_log_api_info_api_detection_exception_via_dir().QueryThatFailsOnDir#
  TestTreeSitterCompatCoverage.test_execute_old_api_exception_handling.MockQueryWithException: test_execute_old_api_exception_handling().MockQueryWithException#
  TestTreeSitterCompatCoverage.test_execute_old_api_with_invalid_result_items.MockQueryWithInvalidItems: test_execute_old_api_with_invalid_result_items().MockQueryWithInvalidItems#
  TestTreeSitterCompatCoverage.test_execute_old_api_non_callable_warning.NonCallableQuery: test_execute_old_api_non_callable_warning().NonCallableQuery#
  TestTreeSitterCompatCoverage: ''
  TestTreeSitterCompatCoverage.test_execute_query_old_api_callable.MockQuery.__call__: test_execute_query_old_api_callable().MockQuery#__call__().
  TestTreeSitterCompatCoverage.test_execute_query_old_api_callable_named_tuple.MockQuery.__call__: test_execute_query_old_api_callable_named_tuple().MockQuery#__call__().
  TestTreeSitterCompatCoverage.test_log_api_info_api_detection_exception_via_dir.QueryThatFailsOnDir.__dir__: test_log_api_info_api_detection_exception_via_dir().QueryThatFailsOnDir#__dir__().
  TestTreeSitterCompatCoverage.test_execute_old_api_exception_handling.MockQueryWithException.__call__: test_execute_old_api_exception_handling().MockQueryWithException#__call__().
  TestTreeSitterCompatCoverage.test_execute_old_api_with_invalid_result_items.MockQueryWithInvalidItems.__call__: test_execute_old_api_with_invalid_result_items().MockQueryWithInvalidItems#__call__().
---
# Module: [`tests/unit/core/test_tree_sitter_compat_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py)

## Classes
### `MockQuery`
- def: [`tests/unit/core/test_tree_sitter_compat_coverage.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L153)
- signature: `class MockQuery:`
- protocol/private: `__call__`[`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L119), `__call__`[`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L154)
- used by: (1 test-only callers)

### `MockQueryWithException`
- def: [`tests/unit/core/test_tree_sitter_compat_coverage.py:409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L409)
- signature: `class MockQueryWithException:`
- protocol/private: `__call__`[`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L410)
- used by: (1 test-only callers)

### `MockQueryWithInvalidItems`
- def: [`tests/unit/core/test_tree_sitter_compat_coverage.py:424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L424)
- signature: `class MockQueryWithInvalidItems:`
- protocol/private: `__call__`[`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L425)
- used by: (1 test-only callers)

### `NonCallableQuery`
- def: [`tests/unit/core/test_tree_sitter_compat_coverage.py:444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L444)
- signature: `class NonCallableQuery:`
- used by: (1 test-only callers)

### `QueryThatFailsOnDir`
- def: [`tests/unit/core/test_tree_sitter_compat_coverage.py:365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L365)
- signature: `class QueryThatFailsOnDir:`
- protocol/private: `__dir__`[`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L367)
- used by: (1 test-only callers)

### `TestTreeSitterCompatCoverage`
- def: [`tests/unit/core/test_tree_sitter_compat_coverage.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L15)
- signature: `class TestTreeSitterCompatCoverage:`
- members:
  - `mock_import(name, *args, **kwargs)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L326)
  - `test_create_query_safely(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L223) — Test create_query_safely
  - `test_execute_legacy_api_exception_raises(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L390) — Test _execute_legacy_api exception handling (covers lines 116-118)
  - `test_execute_modern_api_exception_raises(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L376) — Test _execute_modern_api exception handling (covers lines 102-104)
  - `test_execute_old_api_exception_handling(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L404) — Test _execute_old_api exception handling (covers lines 138-143)
  - `test_execute_old_api_non_callable_warning(self)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L439) — Test _execute_old_api with non-callable query (covers line 138)
  - `test_execute_old_api_with_invalid_result_items(self)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L419) — Test _execute_old_api with invalid result items
  - `test_execute_query_exception(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L189) — Test exception handling during query execution
  - `test_execute_query_legacy_api(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L83) — Test execution with legacy API (captures)
  - `test_execute_query_modern_api(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L50) — Test execution with modern API (matches)
  - `test_execute_query_newest_api(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L16) — Test execution with newest API (QueryCursor)
  - `test_execute_query_no_compatible_api(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L169) — Test execution when no compatible API is found
  - `test_execute_query_old_api_callable(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L109) — Test execution with old API (callable query)
  - `test_execute_query_old_api_callable_named_tuple(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L140) — Test execution with old API (callable returning objects with node/name attrs)
  - `test_get_node_text_safe_byte_range(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L237) — Test get_node_text_safe using byte range
  - `test_get_node_text_safe_fallback_empty(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L291) — Test get_node_text_safe fallback to empty
  - `test_get_node_text_safe_points_multi_line(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L276) — Test get_node_text_safe using points (multi line)
  - `test_get_node_text_safe_points_single_line(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L265) — Test get_node_text_safe using points (single line)
  - `test_get_node_text_safe_text_attr_bytes(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L247) — Test get_node_text_safe using text attribute (bytes)
  - `test_get_node_text_safe_text_attr_str(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L256) — Test get_node_text_safe using text attribute (str)
  - `test_log_api_info(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L301) — Test log_api_info
  - `test_log_api_info_api_detection_exception(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L345) — Test log_api_info when API detection raises an exception (covers lines 285-286)
  - `test_log_api_info_api_detection_exception_via_dir(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L359) — Test log_api_info when dir() on Query raises an exception (covers lines 285-286)
  - `test_log_api_info_import_error(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L320) — Test log_api_info when tree-sitter import fails (covers lines 288-289)
  - `test_safe_execute_query(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_coverage.py#L203) — Test safe_execute_query wrapper
- uses (calls/refs, reference-scoped): [`get_node_text_safe`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#get_node_text_safe), [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`safe_execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.safe_execute_query), [`execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.execute_query), [`log_api_info`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#log_api_info), [`create_query_safely`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#create_query_safely), [`_execute_old_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_old_api), [`_execute_legacy_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_legacy_api), [`_execute_modern_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_modern_api)  (6 test-only)

