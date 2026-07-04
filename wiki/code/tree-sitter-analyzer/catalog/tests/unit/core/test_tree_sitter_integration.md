---
title: 'Module: tests/unit/core/test_tree_sitter_integration.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_tree_sitter_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_tree_sitter_integration`/TestTreeSitterIntegration#
symbols:
  TestTreeSitterIntegration.test_files: test_files.
  TestTreeSitterIntegration.query_service: query_service.
  TestTreeSitterIntegration.test_mcp_tool_integration: test_mcp_tool_integration().
  TestTreeSitterIntegration.test_large_file_performance: test_large_file_performance().
  TestTreeSitterIntegration.temp_dir: temp_dir.
  TestTreeSitterIntegration.test_parser_integration_all_languages: test_parser_integration_all_languages().
  TestTreeSitterIntegration.test_predefined_queries_all_languages: test_predefined_queries_all_languages().
  TestTreeSitterIntegration.test_custom_queries_integration: test_custom_queries_integration().
  TestTreeSitterIntegration.test_query_result_structure: test_query_result_structure().
  TestTreeSitterIntegration.test_filter_integration: test_filter_integration().
  TestTreeSitterIntegration.test_error_handling_integration: test_error_handling_integration().
  TestTreeSitterIntegration.test_encoding_handling: test_encoding_handling().
  TestTreeSitterIntegration.test_concurrent_queries: test_concurrent_queries().
  TestTreeSitterIntegration.test_query_service_initialization: test_query_service_initialization().
  TestTreeSitterIntegration.test_fallback_mechanisms: test_fallback_mechanisms().
  TestTreeSitterIntegration.test_memory_efficiency: test_memory_efficiency().
  TestTreeSitterIntegration.query_tool: query_tool.
  TestTreeSitterIntegration.test_language_detection_integration: test_language_detection_integration().
  TestTreeSitterIntegration.test_available_queries_integration: test_available_queries_integration().
  TestTreeSitterIntegration.teardown_method: teardown_method().
  TestTreeSitterIntegration.TEST_SAMPLES: TEST_SAMPLES.
  TestTreeSitterIntegration: ''
  TestTreeSitterIntegration.setup_method: setup_method().
---
# Module: [`tests/unit/core/test_tree_sitter_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py)

## Classes
### `TestTreeSitterIntegration`
- def: [`tests/unit/core/test_tree_sitter_integration.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L20)
- doc: Comprehensive tree-sitter integration tests
- signature: `class TestTreeSitterIntegration:`
- members:
  - `setup_method(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L203) — Set up test fixtures
  - `teardown_method(self)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L225) — Clean up test fixtures
  - `test_available_queries_integration(self)` — [`L581`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L581) — Test available queries functionality
  - `test_concurrent_queries(self)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L502) — Test concurrent query execution
  - `test_custom_queries_integration(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L319) — Test custom tree-sitter queries work correctly
  - `test_encoding_handling(self)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L470) — Test handling of different file encodings
  - `test_error_handling_integration(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L427) — Test error handling in tree-sitter integration
  - `test_fallback_mechanisms(self)` — [`L540`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L540) — Test fallback mechanisms in query execution
  - `test_filter_integration(self)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L392) — Test query filtering functionality
  - `test_language_detection_integration(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L232) — Test language detection for all supported file types
  - `test_large_file_performance(self)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L443) — Test performance with larger files
  - `test_mcp_tool_integration(self)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L407) — Test MCP tool integration with tree-sitter
  - `test_memory_efficiency(self)` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L556) — Test memory efficiency of query operations
  - `test_parser_integration_all_languages(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L249) — Test that parser can successfully parse all supported languages
  - `test_predefined_queries_all_languages(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L274) — Test predefined queries work for all languages
  - `test_query_result_structure(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L362) — Test that query results have correct structure
  - `test_query_service_initialization(self)` — [`L529`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L529) — Test QueryService initialization and configuration
  - `TEST_SAMPLES` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L24)
  - `query_service` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L206)
  - `query_tool` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L207)
  - `temp_dir` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L205)
  - `test_files` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_integration.py#L208)
- uses (calls/refs, reference-scoped): [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`detect_language_from_file`](../../../tree_sitter_analyzer/language_detector.md#detect_language_from_file), [`QueryService`](../../../tree_sitter_analyzer/core/query_service.md#QueryService), [`execute_query`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.execute_query), [`execute`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.execute), [`get_available_queries`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.get_available_queries), [`project_root`](../../../tree_sitter_analyzer/core/query_service.md#QueryService.project_root)

