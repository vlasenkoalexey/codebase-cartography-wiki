---
title: 'Module: tests/unit/core/test_tree_sitter_compat.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_tree_sitter_compat.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_tree_sitter_compat`/Test
symbols:
  TestTreeSitterQueryCompatExecuteQuery.test_execute_query_with_real_tree_sitter: TreeSitterQueryCompatExecuteQuery#test_execute_query_with_real_tree_sitter().
  TestTreeSitterQueryCompatExecuteQuery.test_execute_query_error_handling: TreeSitterQueryCompatExecuteQuery#test_execute_query_error_handling().
  TestTreeSitterQueryCompatExecuteQuery.test_execute_query_with_mocked_import_error: TreeSitterQueryCompatExecuteQuery#test_execute_query_with_mocked_import_error().
  TestTreeSitterQueryCompatSafeExecuteQuery.test_safe_execute_query_success: TreeSitterQueryCompatSafeExecuteQuery#test_safe_execute_query_success().
  TestTreeSitterQueryCompatSafeExecuteQuery.test_safe_execute_query_with_fallback: TreeSitterQueryCompatSafeExecuteQuery#test_safe_execute_query_with_fallback().
  TestTreeSitterQueryCompatSafeExecuteQuery.test_safe_execute_query_default_fallback: TreeSitterQueryCompatSafeExecuteQuery#test_safe_execute_query_default_fallback().
  TestTreeSitterQueryCompatInternalMethods.test_execute_newest_api_with_mocks: TreeSitterQueryCompatInternalMethods#test_execute_newest_api_with_mocks().
  TestTreeSitterQueryCompatInternalMethods.test_execute_modern_api_with_mocks: TreeSitterQueryCompatInternalMethods#test_execute_modern_api_with_mocks().
  TestTreeSitterQueryCompatInternalMethods.test_execute_legacy_api_with_mocks: TreeSitterQueryCompatInternalMethods#test_execute_legacy_api_with_mocks().
  TestTreeSitterQueryCompatInternalMethods.test_execute_old_api_callable: TreeSitterQueryCompatInternalMethods#test_execute_old_api_callable().
  TestTreeSitterQueryCompatInternalMethods.test_execute_old_api_non_callable: TreeSitterQueryCompatInternalMethods#test_execute_old_api_non_callable().
  TestCompatibilityScenarios.test_module_has_execute_query: CompatibilityScenarios#test_module_has_execute_query().
  TestCompatibilityScenarios.test_module_has_safe_execute_query: CompatibilityScenarios#test_module_has_safe_execute_query().
  TestCompatibilityScenarios.test_all_api_methods_are_static: CompatibilityScenarios#test_all_api_methods_are_static().
  TestGetNodeTextSafe.test_byte_based_extraction: GetNodeTextSafe#test_byte_based_extraction().
  TestGetNodeTextSafe.test_byte_based_extraction_middle: GetNodeTextSafe#test_byte_based_extraction_middle().
  TestGetNodeTextSafe.test_byte_based_extraction_unicode: GetNodeTextSafe#test_byte_based_extraction_unicode().
  TestGetNodeTextSafe.test_byte_based_extraction_empty: GetNodeTextSafe#test_byte_based_extraction_empty().
  TestGetNodeTextSafe.test_node_text_attribute_bytes: GetNodeTextSafe#test_node_text_attribute_bytes().
  TestGetNodeTextSafe.test_node_text_attribute_string: GetNodeTextSafe#test_node_text_attribute_string().
  TestGetNodeTextSafe.test_point_based_extraction_single_line: GetNodeTextSafe#test_point_based_extraction_single_line().
  TestGetNodeTextSafe.test_point_based_extraction_multi_line: GetNodeTextSafe#test_point_based_extraction_multi_line().
  TestGetNodeTextSafe.test_point_based_extraction_partial_lines: GetNodeTextSafe#test_point_based_extraction_partial_lines().
  TestGetNodeTextSafe.test_invalid_byte_range: GetNodeTextSafe#test_invalid_byte_range().
  TestGetNodeTextSafe.test_negative_byte_range: GetNodeTextSafe#test_negative_byte_range().
  TestGetNodeTextSafe.test_no_attributes: GetNodeTextSafe#test_no_attributes().
  TestGetNodeTextSafe.test_exception_handling: GetNodeTextSafe#test_exception_handling().
  TestGetNodeTextSafe.test_different_encoding: GetNodeTextSafe#test_different_encoding().
  TestGetNodeTextSafe.test_decoding_error_handling: GetNodeTextSafe#test_decoding_error_handling().
  TestCreateQuerySafely.test_successful_query_creation: CreateQuerySafely#test_successful_query_creation().
  TestCreateQuerySafely.test_query_creation_failure: CreateQuerySafely#test_query_creation_failure().
  TestCreateQuerySafely.test_query_creation_invalid_query: CreateQuerySafely#test_query_creation_invalid_query().
  TestLogApiInfo.test_log_api_info_with_tree_sitter: LogApiInfo#test_log_api_info_with_tree_sitter().
  TestLogApiInfo.test_log_api_info_callable: LogApiInfo#test_log_api_info_callable().
  TestLogApiInfo.test_log_api_info_logs_debug_info: LogApiInfo#test_log_api_info_logs_debug_info().
  TestTreeSitterQueryCompatInternalMethods.test_all_internal_methods_exist: TreeSitterQueryCompatInternalMethods#test_all_internal_methods_exist().
  TestEdgeCases.test_empty_source_code: EdgeCases#test_empty_source_code().
  TestEdgeCases.test_very_large_source_code: EdgeCases#test_very_large_source_code().
  TestEdgeCases.test_multi_byte_characters: EdgeCases#test_multi_byte_characters().
  TestEdgeCases.test_point_extraction_out_of_bounds: EdgeCases#test_point_extraction_out_of_bounds().
  TestCompatibilityScenarios.test_query_compat_is_class: CompatibilityScenarios#test_query_compat_is_class().
  TestGetNodeTextSafe: GetNodeTextSafe#
  TestCreateQuerySafely: CreateQuerySafely#
  TestLogApiInfo: LogApiInfo#
  TestTreeSitterQueryCompatExecuteQuery: TreeSitterQueryCompatExecuteQuery#
  TestTreeSitterQueryCompatSafeExecuteQuery: TreeSitterQueryCompatSafeExecuteQuery#
  TestTreeSitterQueryCompatInternalMethods: TreeSitterQueryCompatInternalMethods#
  TestEdgeCases: EdgeCases#
  TestCompatibilityScenarios: CompatibilityScenarios#
---
# Module: [`tests/unit/core/test_tree_sitter_compat.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py)

## Classes
### `TestCompatibilityScenarios`
- def: [`tests/unit/core/test_tree_sitter_compat.py:462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L462)
- doc: Test various version compatibility scenarios
- signature: `class TestCompatibilityScenarios:`
- members:
  - `test_all_api_methods_are_static(self)` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L479) — Test that API methods are static methods
  - `test_module_has_execute_query(self)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L465) — Test that TreeSitterQueryCompat has execute_query method
  - `test_module_has_safe_execute_query(self)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L470) — Test that TreeSitterQueryCompat has safe_execute_query method
  - `test_query_compat_is_class(self)` — [`L475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L475) — Test that TreeSitterQueryCompat is a proper class
- uses (calls/refs, reference-scoped): [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`safe_execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.safe_execute_query), [`execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.execute_query)

### `TestCreateQuerySafely`
- def: [`tests/unit/core/test_tree_sitter_compat.py:195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L195)
- doc: Test create_query_safely function
- signature: `class TestCreateQuerySafely:`
- members:
  - `test_query_creation_failure(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L211) — Test query creation failure handling
  - `test_query_creation_invalid_query(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L219) — Test query creation with invalid query string
  - `test_successful_query_creation(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L198) — Test successful query creation
- uses (calls/refs, reference-scoped): [`create_query_safely`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#create_query_safely)

### `TestEdgeCases`
- def: [`tests/unit/core/test_tree_sitter_compat.py:416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L416)
- doc: Test edge cases and boundary conditions
- signature: `class TestEdgeCases:`
- members:
  - `test_empty_source_code(self)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L419) — Test with empty source code
  - `test_multi_byte_characters(self)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L438) — Test with multi-byte UTF-8 characters
  - `test_point_extraction_out_of_bounds(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L448) — Test point-based extraction with out of bounds coordinates
  - `test_very_large_source_code(self)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L428) — Test with very large source code
- uses (calls/refs, reference-scoped): [`get_node_text_safe`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#get_node_text_safe)

### `TestGetNodeTextSafe`
- def: [`tests/unit/core/test_tree_sitter_compat.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L22)
- doc: Test get_node_text_safe function with various node types
- signature: `class TestGetNodeTextSafe:`
- members:
  - `test_byte_based_extraction(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L25) — Test text extraction using byte positions
  - `test_byte_based_extraction_empty(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L55) — Test extraction with empty range
  - `test_byte_based_extraction_middle(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L35) — Test extraction from middle of source
  - `test_byte_based_extraction_unicode(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L45) — Test extraction with unicode characters
  - `test_decoding_error_handling(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L182) — Test handling of decoding errors
  - `test_different_encoding(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L172) — Test with different encoding
  - `test_exception_handling(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L163) — Test that exceptions are handled gracefully
  - `test_invalid_byte_range(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L129) — Test handling of invalid byte range
  - `test_negative_byte_range(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L140) — Test handling of negative byte positions
  - `test_no_attributes(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L150) — Test node with no extraction attributes
  - `test_node_text_attribute_bytes(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L65) — Test fallback to node.text attribute (bytes)
  - `test_node_text_attribute_string(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L78) — Test fallback to node.text attribute (string)
  - `test_point_based_extraction_multi_line(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L102) — Test extraction using point positions (multiple lines)
  - `test_point_based_extraction_partial_lines(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L116) — Test extraction with partial line ranges
  - `test_point_based_extraction_single_line(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L89) — Test extraction using point positions (single line)
- uses (calls/refs, reference-scoped): [`get_node_text_safe`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#get_node_text_safe)

### `TestLogApiInfo`
- def: [`tests/unit/core/test_tree_sitter_compat.py:229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L229)
- doc: Test log_api_info function
- signature: `class TestLogApiInfo:`
- members:
  - `test_log_api_info_callable(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L242) — Test that log_api_info can be called without errors
  - `test_log_api_info_logs_debug_info(self, caplog)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L247) — Test that log_api_info logs debug information
  - `test_log_api_info_with_tree_sitter(self, caplog)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L232) — Test logging API info when tree-sitter is available
- uses (calls/refs, reference-scoped): [`log_api_info`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#log_api_info)

### `TestTreeSitterQueryCompatExecuteQuery`
- def: [`tests/unit/core/test_tree_sitter_compat.py:258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L258)
- doc: Test TreeSitterQueryCompat.execute_query method
- signature: `class TestTreeSitterQueryCompatExecuteQuery:`
- members:
  - `test_execute_query_error_handling(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L281) — Test error handling in query execution
  - `test_execute_query_with_mocked_import_error(self)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L289) — Test handling when tree-sitter import fails
  - `test_execute_query_with_real_tree_sitter(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L261) — Test query execution with real tree-sitter if available
- uses (calls/refs, reference-scoped): [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.execute_query)

### `TestTreeSitterQueryCompatInternalMethods`
- def: [`tests/unit/core/test_tree_sitter_compat.py:339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L339)
- doc: Test internal API compatibility methods
- signature: `class TestTreeSitterQueryCompatInternalMethods:`
- members:
  - `test_all_internal_methods_exist(self)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L408) — Test that all internal methods exist
  - `test_execute_legacy_api_with_mocks(self)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L375) — Test _execute_legacy_api method with mocks
  - `test_execute_modern_api_with_mocks(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L354) — Test _execute_modern_api method with mocks
  - `test_execute_newest_api_with_mocks(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L342) — Test _execute_newest_api method with mocks
  - `test_execute_old_api_callable(self)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L387) — Test _execute_old_api with callable query
  - `test_execute_old_api_non_callable(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L399) — Test _execute_old_api with non-callable query
- uses (calls/refs, reference-scoped): [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`_execute_old_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_old_api), [`_execute_legacy_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_legacy_api), [`_execute_modern_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_modern_api), [`_execute_newest_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_newest_api)

### `TestTreeSitterQueryCompatSafeExecuteQuery`
- def: [`tests/unit/core/test_tree_sitter_compat.py:299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L299)
- doc: Test TreeSitterQueryCompat.safe_execute_query method
- signature: `class TestTreeSitterQueryCompatSafeExecuteQuery:`
- members:
  - `test_safe_execute_query_default_fallback(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L327) — Test safe query execution with default fallback
  - `test_safe_execute_query_success(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L302) — Test successful safe query execution
  - `test_safe_execute_query_with_fallback(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat.py#L314) — Test safe query execution with custom fallback
- uses (calls/refs, reference-scoped): [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`safe_execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.safe_execute_query)

