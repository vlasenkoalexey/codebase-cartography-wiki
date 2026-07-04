---
title: 'Module: tests/unit/core/test_queries_typescript_extended.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_typescript_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_typescript_extended`/TestTypeScript
symbols:
  TestTypeScriptExtendedQueries.test_function_utilities: ExtendedQueries#test_function_utilities().
  TestTypeScriptExtendedQueries.test_new_function_queries: ExtendedQueries#test_new_function_queries().
  TestTypeScriptExtendedQueries.test_new_class_queries: ExtendedQueries#test_new_class_queries().
  TestTypeScriptExtendedQueries.test_new_variable_queries: ExtendedQueries#test_new_variable_queries().
  TestTypeScriptExtendedQueries.test_new_import_queries: ExtendedQueries#test_new_import_queries().
  TestTypeScriptExtendedQueries.test_type_system_queries: ExtendedQueries#test_type_system_queries().
  TestTypeScriptExtendedQueries.test_method_visibility_queries: ExtendedQueries#test_method_visibility_queries().
  TestTypeScriptExtendedQueries.test_property_queries: ExtendedQueries#test_property_queries().
  TestTypeScriptExtendedQueries.test_signature_queries: ExtendedQueries#test_signature_queries().
  TestTypeScriptExtendedQueries.test_jsx_queries: ExtendedQueries#test_jsx_queries().
  TestTypeScriptExtendedQueries.test_expression_queries: ExtendedQueries#test_expression_queries().
  TestTypeScriptExtendedQueries.test_pattern_queries: ExtendedQueries#test_pattern_queries().
  TestTypeScriptExtendedQueries.test_literal_queries: ExtendedQueries#test_literal_queries().
  TestTypeScriptExtendedQueries.test_declaration_queries: ExtendedQueries#test_declaration_queries().
  TestTypeScriptExtendedQueries.test_modifier_queries: ExtendedQueries#test_modifier_queries().
  TestTypeScriptExtendedQueries.test_query_count: ExtendedQueries#test_query_count().
  TestTypeScriptExtendedQueries.test_all_queries_have_valid_structure: ExtendedQueries#test_all_queries_have_valid_structure().
  TestTypeScriptExtendedQueries.test_query_syntax_basic_validation: ExtendedQueries#test_query_syntax_basic_validation().
  TestTypeScriptExtendedQueries.test_capture_groups_present: ExtendedQueries#test_capture_groups_present().
  TestTypeScriptExtendedQueries.test_typescript_coverage_comprehensive: ExtendedQueries#test_typescript_coverage_comprehensive().
  TestTypeScriptExtendedQueries.test_alias_queries: ExtendedQueries#test_alias_queries().
  TestTypeScriptExtendedQueries.test_generic_type_query_specific: ExtendedQueries#test_generic_type_query_specific().
  TestTypeScriptExtendedQueries.test_namespace_query_specific: ExtendedQueries#test_namespace_query_specific().
  TestTypeScriptExtendedQueries.test_query_descriptions_meaningful: ExtendedQueries#test_query_descriptions_meaningful().
  TestTypeScriptExtendedQueries.test_new_queries_integration: ExtendedQueries#test_new_queries_integration().
  TestTypeScriptQueryComparison.test_typescript_vs_javascript_coverage: QueryComparison#test_typescript_vs_javascript_coverage().
  TestTypeScriptQueryComparison.test_comprehensive_language_support: QueryComparison#test_comprehensive_language_support().
  TestTypeScriptExtendedQueries: ExtendedQueries#
  TestTypeScriptQueryComparison: QueryComparison#
---
# Module: [`tests/unit/core/test_queries_typescript_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py)

## Classes
### `TestTypeScriptExtendedQueries`
- def: [`tests/unit/core/test_queries_typescript_extended.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L15)
- doc: Test cases for extended TypeScript query definitions
- signature: `class TestTypeScriptExtendedQueries:`
- members:
  - `test_alias_queries(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L318) — Test that alias queries work correctly
  - `test_all_queries_have_valid_structure(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L232) — Test that all queries have valid structure
  - `test_capture_groups_present(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L272) — Test that queries contain capture groups
  - `test_declaration_queries(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L195) — Test declaration-specific queries
  - `test_expression_queries(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L158) — Test expression-specific queries
  - `test_function_utilities(self)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L375) — Test utility functions work with extended queries
  - `test_generic_type_query_specific(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L326) — Test generic_type query specifically
  - `test_jsx_queries(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L147) — Test that JSX queries are not in TypeScript grammar (TSX-only)
  - `test_literal_queries(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L185) — Test literal-specific queries
  - `test_method_visibility_queries(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L97) — Test method visibility queries
  - `test_modifier_queries(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L210) — Test modifier-specific queries
  - `test_namespace_query_specific(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L336) — Test namespace query specifically
  - `test_new_class_queries(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L36) — Test new class-specific queries
  - `test_new_function_queries(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L18) — Test new function-specific queries
  - `test_new_import_queries(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L56) — Test new import-specific queries
  - `test_new_queries_integration(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L363) — Test that new queries integrate well with existing ones
  - `test_new_variable_queries(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L46) — Test new variable-specific queries
  - `test_pattern_queries(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L175) — Test pattern-specific queries
  - `test_property_queries(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L116) — Test property-specific queries
  - `test_query_count(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L227) — Test that we have the expected number of queries
  - `test_query_descriptions_meaningful(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L345) — Test that query descriptions are meaningful and specific
  - `test_query_syntax_basic_validation(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L254) — Test basic syntax validation for queries
  - `test_signature_queries(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L131) — Test signature-specific queries
  - `test_type_system_queries(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L71) — Test TypeScript type system queries
  - `test_typescript_coverage_comprehensive(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L280) — Test comprehensive TypeScript feature coverage
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/typescript.md#ALL_QUERIES), [`list_queries`](../../../tree_sitter_analyzer/queries/typescript.md#list_queries), [`get_query`](../../../tree_sitter_analyzer/queries/typescript.md#get_query), [`get_all_queries`](../../../tree_sitter_analyzer/queries/typescript.md#get_all_queries)

### `TestTypeScriptQueryComparison`
- def: [`tests/unit/core/test_queries_typescript_extended.py:396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L396)
- doc: Test TypeScript queries compared to other languages
- signature: `class TestTypeScriptQueryComparison:`
- members:
  - `test_comprehensive_language_support(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L426) — Test that TypeScript queries provide comprehensive language support
  - `test_typescript_vs_javascript_coverage(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript_extended.py#L399) — Test that TypeScript has more queries than JavaScript
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/typescript.md#ALL_QUERIES)

