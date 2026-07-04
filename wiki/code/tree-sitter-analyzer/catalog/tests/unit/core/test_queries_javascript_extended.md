---
title: 'Module: tests/unit/core/test_queries_javascript_extended.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_javascript_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_javascript_extended`/TestJavaScript
symbols:
  TestJavaScriptExtendedQueries.test_consistency_with_constants: ExtendedQueries#test_consistency_with_constants().
  TestJavaScriptExtendedQueries.test_utility_functions: ExtendedQueries#test_utility_functions().
  TestJavaScriptExtendedQueries.test_query_count_comprehensive: ExtendedQueries#test_query_count_comprehensive().
  TestJavaScriptExtendedQueries.test_function_queries_comprehensive: ExtendedQueries#test_function_queries_comprehensive().
  TestJavaScriptExtendedQueries.test_class_queries_comprehensive: ExtendedQueries#test_class_queries_comprehensive().
  TestJavaScriptExtendedQueries.test_variable_queries_comprehensive: ExtendedQueries#test_variable_queries_comprehensive().
  TestJavaScriptExtendedQueries.test_import_export_queries: ExtendedQueries#test_import_export_queries().
  TestJavaScriptExtendedQueries.test_modern_javascript_features: ExtendedQueries#test_modern_javascript_features().
  TestJavaScriptExtendedQueries.test_jsx_queries: ExtendedQueries#test_jsx_queries().
  TestJavaScriptExtendedQueries.test_object_queries: ExtendedQueries#test_object_queries().
  TestJavaScriptExtendedQueries.test_control_flow_queries: ExtendedQueries#test_control_flow_queries().
  TestJavaScriptExtendedQueries.test_expression_queries: ExtendedQueries#test_expression_queries().
  TestJavaScriptExtendedQueries.test_comment_queries: ExtendedQueries#test_comment_queries().
  TestJavaScriptExtendedQueries.test_all_queries_structure: ExtendedQueries#test_all_queries_structure().
  TestJavaScriptExtendedQueries.test_query_syntax_validation: ExtendedQueries#test_query_syntax_validation().
  TestJavaScriptExtendedQueries.test_capture_groups_present: ExtendedQueries#test_capture_groups_present().
  TestJavaScriptExtendedQueries.test_javascript_specific_features: ExtendedQueries#test_javascript_specific_features().
  TestJavaScriptExtendedQueries.test_query_descriptions_quality: ExtendedQueries#test_query_descriptions_quality().
  TestJavaScriptExtendedQueries.test_framework_specific_queries: ExtendedQueries#test_framework_specific_queries().
  TestJavaScriptExtendedQueries.test_advanced_patterns: ExtendedQueries#test_advanced_patterns().
  TestJavaScriptExtendedQueries.test_es6_plus_features: ExtendedQueries#test_es6_plus_features().
  TestJavaScriptQueryComparison.test_javascript_comprehensive_coverage: QueryComparison#test_javascript_comprehensive_coverage().
  TestJavaScriptQueryComparison.test_javascript_vs_typescript_features: QueryComparison#test_javascript_vs_typescript_features().
  TestJavaScriptQueryComparison.test_javascript_specific_vs_typescript: QueryComparison#test_javascript_specific_vs_typescript().
  TestJavaScriptExtendedQueries: ExtendedQueries#
  TestJavaScriptQueryComparison: QueryComparison#
---
# Module: [`tests/unit/core/test_queries_javascript_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py)

## Classes
### `TestJavaScriptExtendedQueries`
- def: [`tests/unit/core/test_queries_javascript_extended.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L15)
- doc: Test cases for extended JavaScript query definitions
- signature: `class TestJavaScriptExtendedQueries:`
- members:
  - `test_advanced_patterns(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L321) — Test advanced JavaScript patterns
  - `test_all_queries_structure(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L192) — Test that all queries have valid structure
  - `test_capture_groups_present(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L230) — Test that queries contain capture groups
  - `test_class_queries_comprehensive(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L43) — Test comprehensive class query coverage
  - `test_comment_queries(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L182) — Test comment queries
  - `test_consistency_with_constants(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L294) — Test consistency between constants and ALL_QUERIES
  - `test_control_flow_queries(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L147) — Test control flow queries
  - `test_es6_plus_features(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L338) — Test ES6+ feature queries
  - `test_expression_queries(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L165) — Test expression queries
  - `test_framework_specific_queries(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L306) — Test framework-specific queries
  - `test_function_queries_comprehensive(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L23) — Test comprehensive function query coverage
  - `test_import_export_queries(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L77) — Test import/export query coverage
  - `test_javascript_specific_features(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L238) — Test JavaScript-specific features in queries
  - `test_jsx_queries(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L115) — Test JSX query coverage
  - `test_modern_javascript_features(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L96) — Test modern JavaScript feature queries
  - `test_object_queries(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L131) — Test object-related queries
  - `test_query_count_comprehensive(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L18) — Test that JavaScript has comprehensive query coverage
  - `test_query_descriptions_quality(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L261) — Test that query descriptions are meaningful
  - `test_query_syntax_validation(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L214) — Test basic syntax validation for queries
  - `test_utility_functions(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L274) — Test utility functions
  - `test_variable_queries_comprehensive(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L62) — Test comprehensive variable query coverage
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/javascript.md#ALL_QUERIES), [`VARIABLES`](../../../tree_sitter_analyzer/queries/javascript.md#VARIABLES), [`list_queries`](../../../tree_sitter_analyzer/queries/javascript.md#list_queries), [`FUNCTIONS`](../../../tree_sitter_analyzer/queries/javascript.md#FUNCTIONS), [`get_query`](../../../tree_sitter_analyzer/queries/javascript.md#get_query), [`CLASSES`](../../../tree_sitter_analyzer/queries/javascript.md#CLASSES), [`get_all_queries`](../../../tree_sitter_analyzer/queries/javascript.md#get_all_queries)

### `TestJavaScriptQueryComparison`
- def: [`tests/unit/core/test_queries_javascript_extended.py:358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L358)
- doc: Test JavaScript queries in comparison to other languages
- signature: `class TestJavaScriptQueryComparison:`
- members:
  - `test_javascript_comprehensive_coverage(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L361) — Test that JavaScript has comprehensive coverage
  - `test_javascript_specific_vs_typescript(self)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L379) — Test JavaScript-specific features vs TypeScript
  - `test_javascript_vs_typescript_features(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript_extended.py#L369) — Test JavaScript vs TypeScript feature overlap
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/javascript.md#ALL_QUERIES)

