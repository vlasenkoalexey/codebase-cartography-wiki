---
title: 'Module: tests/unit/core/test_queries_javascript_enhanced.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_javascript_enhanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_javascript_enhanced`/TestEnhancedJavaScriptQueries#
symbols:
  TestEnhancedJavaScriptQueries.test_get_all_queries_structure: test_get_all_queries_structure().
  TestEnhancedJavaScriptQueries.test_javascript_query_descriptions: test_javascript_query_descriptions().
  TestEnhancedJavaScriptQueries.test_query_consistency_with_descriptions: test_query_consistency_with_descriptions().
  TestEnhancedJavaScriptQueries.test_get_query_function_compatibility: test_get_query_function_compatibility().
  TestEnhancedJavaScriptQueries.test_list_queries_includes_all: test_list_queries_includes_all().
  TestEnhancedJavaScriptQueries.test_javascript_queries_structure: test_javascript_queries_structure().
  TestEnhancedJavaScriptQueries.test_get_javascript_query_valid: test_get_javascript_query_valid().
  TestEnhancedJavaScriptQueries.test_get_javascript_query_invalid: test_get_javascript_query_invalid().
  TestEnhancedJavaScriptQueries.test_get_javascript_query_description_valid: test_get_javascript_query_description_valid().
  TestEnhancedJavaScriptQueries.test_get_javascript_query_description_invalid: test_get_javascript_query_description_invalid().
  TestEnhancedJavaScriptQueries.test_get_available_javascript_queries: test_get_available_javascript_queries().
  TestEnhancedJavaScriptQueries.test_all_queries_integration: test_all_queries_integration().
  TestEnhancedJavaScriptQueries.test_legacy_queries_compatibility: test_legacy_queries_compatibility().
  TestEnhancedJavaScriptQueries.test_function_queries_comprehensive: test_function_queries_comprehensive().
  TestEnhancedJavaScriptQueries.test_class_queries_comprehensive: test_class_queries_comprehensive().
  TestEnhancedJavaScriptQueries.test_variable_queries_comprehensive: test_variable_queries_comprehensive().
  TestEnhancedJavaScriptQueries.test_import_export_queries_comprehensive: test_import_export_queries_comprehensive().
  TestEnhancedJavaScriptQueries.test_modern_javascript_queries: test_modern_javascript_queries().
  TestEnhancedJavaScriptQueries.test_jsx_queries: test_jsx_queries().
  TestEnhancedJavaScriptQueries.test_framework_queries: test_framework_queries().
  TestEnhancedJavaScriptQueries.test_control_flow_queries: test_control_flow_queries().
  TestEnhancedJavaScriptQueries.test_error_handling_queries: test_error_handling_queries().
  TestEnhancedJavaScriptQueries.test_comment_queries: test_comment_queries().
  TestEnhancedJavaScriptQueries.test_advanced_pattern_queries: test_advanced_pattern_queries().
  TestEnhancedJavaScriptQueries.test_name_extraction_queries: test_name_extraction_queries().
  TestEnhancedJavaScriptQueries.test_all_queries_have_capture_groups: test_all_queries_have_capture_groups().
  TestEnhancedJavaScriptQueries.test_query_syntax_validity: test_query_syntax_validity().
  TestEnhancedJavaScriptQueries: ''
---
# Module: [`tests/unit/core/test_queries_javascript_enhanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py)

## Classes
### `TestEnhancedJavaScriptQueries`
- def: [`tests/unit/core/test_queries_javascript_enhanced.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L24)
- doc: Test enhanced JavaScript queries functionality
- signature: `class TestEnhancedJavaScriptQueries:`
- members:
  - `test_advanced_pattern_queries(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L378) — Test advanced pattern queries
  - `test_all_queries_have_capture_groups(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L427) — Test that all queries have proper capture groups
  - `test_all_queries_integration(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L137) — Test ALL_QUERIES integration with enhanced queries
  - `test_class_queries_comprehensive(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L190) — Test comprehensive class query coverage
  - `test_comment_queries(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L361) — Test comment-related queries
  - `test_control_flow_queries(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L312) — Test control flow queries
  - `test_error_handling_queries(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L338) — Test error handling queries
  - `test_framework_queries(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L298) — Test framework-specific queries
  - `test_function_queries_comprehensive(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L167) — Test comprehensive function query coverage
  - `test_get_all_queries_structure(self)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L477) — Test get_all_queries returns proper structure
  - `test_get_available_javascript_queries(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L120) — Test getting list of available JavaScript queries
  - `test_get_javascript_query_description_invalid(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L115) — Test getting description for invalid query
  - `test_get_javascript_query_description_valid(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L106) — Test getting valid query descriptions
  - `test_get_javascript_query_invalid(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L96) — Test getting invalid JavaScript query raises ValueError
  - `test_get_javascript_query_valid(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L80) — Test getting valid JavaScript queries
  - `test_get_query_function_compatibility(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L447) — Test compatibility with get_query function
  - `test_import_export_queries_comprehensive(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L239) — Test comprehensive import/export query coverage
  - `test_javascript_queries_structure(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L27) — Test JAVASCRIPT_QUERIES dictionary structure
  - `test_javascript_query_descriptions(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L64) — Test JAVASCRIPT_QUERY_DESCRIPTIONS dictionary
  - `test_jsx_queries(self)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L284) — Test JSX-related queries
  - `test_legacy_queries_compatibility(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L154) — Test backward compatibility with legacy queries
  - `test_list_queries_includes_all(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L459) — Test that list_queries includes all available queries
  - `test_modern_javascript_queries(self)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L268) — Test modern JavaScript feature queries
  - `test_name_extraction_queries(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L394) — Test name-only extraction queries
  - `test_query_consistency_with_descriptions(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L404) — Test consistency between queries and descriptions
  - `test_query_syntax_validity(self)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L433) — Test basic query syntax validity
  - `test_variable_queries_comprehensive(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_enhanced.py#L216) — Test comprehensive variable query coverage
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/javascript.md#ALL_QUERIES), [`JAVASCRIPT_QUERIES`](../../../tree_sitter_analyzer/queries/javascript.md#JAVASCRIPT_QUERIES.JAVASCRIPT_QUERIES), [`JAVASCRIPT_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/javascript.md#JAVASCRIPT_QUERY_DESCRIPTIONS.JAVASCRIPT_QUERY_DESCRIPTIONS), [`get_javascript_query`](../../../tree_sitter_analyzer/queries/javascript.md#get_javascript_query), [`list_queries`](../../../tree_sitter_analyzer/queries/javascript.md#list_queries), [`get_javascript_query_description`](../../../tree_sitter_analyzer/queries/javascript.md#get_javascript_query_description), [`get_available_javascript_queries`](../../../tree_sitter_analyzer/queries/javascript.md#get_available_javascript_queries), [`get_query`](../../../tree_sitter_analyzer/queries/javascript.md#get_query), [`get_all_queries`](../../../tree_sitter_analyzer/queries/javascript.md#get_all_queries)

