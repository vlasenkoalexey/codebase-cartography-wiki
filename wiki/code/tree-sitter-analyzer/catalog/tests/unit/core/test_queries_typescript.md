---
title: 'Module: tests/unit/core/test_queries_typescript.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_typescript.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_typescript`/TestTypeScriptQueries#
symbols:
  TestTypeScriptQueries.test_get_query_function: test_get_query_function().
  TestTypeScriptQueries.test_get_all_queries_function: test_get_all_queries_function().
  TestTypeScriptQueries.test_list_queries_function: test_list_queries_function().
  TestTypeScriptQueries.test_functions_query_exists: test_functions_query_exists().
  TestTypeScriptQueries.test_classes_query_exists: test_classes_query_exists().
  TestTypeScriptQueries.test_interfaces_query_exists: test_interfaces_query_exists().
  TestTypeScriptQueries.test_type_aliases_query_exists: test_type_aliases_query_exists().
  TestTypeScriptQueries.test_enums_query_exists: test_enums_query_exists().
  TestTypeScriptQueries.test_variables_query_exists: test_variables_query_exists().
  TestTypeScriptQueries.test_imports_query_exists: test_imports_query_exists().
  TestTypeScriptQueries.test_exports_query_exists: test_exports_query_exists().
  TestTypeScriptQueries.test_decorators_query_exists: test_decorators_query_exists().
  TestTypeScriptQueries.test_generics_query_exists: test_generics_query_exists().
  TestTypeScriptQueries.test_signatures_query_exists: test_signatures_query_exists().
  TestTypeScriptQueries.test_comments_query_exists: test_comments_query_exists().
  TestTypeScriptQueries.test_all_queries_dict_exists: test_all_queries_dict_exists().
  TestTypeScriptQueries.test_all_queries_structure: test_all_queries_structure().
  TestTypeScriptQueries.test_expected_queries_present: test_expected_queries_present().
  TestTypeScriptQueries.test_functions_query_patterns: test_functions_query_patterns().
  TestTypeScriptQueries.test_classes_query_patterns: test_classes_query_patterns().
  TestTypeScriptQueries.test_interfaces_query_patterns: test_interfaces_query_patterns().
  TestTypeScriptQueries.test_type_aliases_query_patterns: test_type_aliases_query_patterns().
  TestTypeScriptQueries.test_enums_query_patterns: test_enums_query_patterns().
  TestTypeScriptQueries.test_variables_query_patterns: test_variables_query_patterns().
  TestTypeScriptQueries.test_imports_query_patterns: test_imports_query_patterns().
  TestTypeScriptQueries.test_exports_query_patterns: test_exports_query_patterns().
  TestTypeScriptQueries.test_decorators_query_patterns: test_decorators_query_patterns().
  TestTypeScriptQueries.test_generics_query_patterns: test_generics_query_patterns().
  TestTypeScriptQueries.test_signatures_query_patterns: test_signatures_query_patterns().
  TestTypeScriptQueries.test_query_syntax_validity: test_query_syntax_validity().
  TestTypeScriptQueries.test_typescript_specific_features: test_typescript_specific_features().
  TestTypeScriptQueries.test_query_descriptions_quality: test_query_descriptions_quality().
  TestTypeScriptQueries.test_capture_group_consistency: test_capture_group_consistency().
  TestTypeScriptQueries: ''
---
# Module: [`tests/unit/core/test_queries_typescript.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py)

## Classes
### `TestTypeScriptQueries`
- def: [`tests/unit/core/test_queries_typescript.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L14)
- doc: Test cases for TypeScript query definitions
- signature: `class TestTypeScriptQueries:`
- members:
  - `test_all_queries_dict_exists(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L89) — Test that ALL_QUERIES dictionary is defined
  - `test_all_queries_structure(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L95) — Test the structure of ALL_QUERIES dictionary
  - `test_capture_group_consistency(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L362) — Test that capture groups follow consistent naming patterns
  - `test_classes_query_exists(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L23) — Test that CLASSES query is defined
  - `test_classes_query_patterns(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L150) — Test that CLASSES query contains expected patterns
  - `test_comments_query_exists(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L83) — Test that COMMENTS query is defined
  - `test_decorators_query_exists(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L65) — Test that DECORATORS query is defined
  - `test_decorators_query_patterns(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L228) — Test that DECORATORS query contains expected patterns
  - `test_enums_query_exists(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L41) — Test that ENUMS query is defined
  - `test_enums_query_patterns(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L184) — Test that ENUMS query contains expected patterns
  - `test_expected_queries_present(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L112) — Test that expected TypeScript queries are present
  - `test_exports_query_exists(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L59) — Test that EXPORTS query is defined
  - `test_exports_query_patterns(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L218) — Test that EXPORTS query contains expected patterns
  - `test_functions_query_exists(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L17) — Test that FUNCTIONS query is defined
  - `test_functions_query_patterns(self)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L135) — Test that FUNCTIONS query contains expected patterns
  - `test_generics_query_exists(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L71) — Test that GENERICS query is defined
  - `test_generics_query_patterns(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L238) — Test that GENERICS query contains expected patterns
  - `test_get_all_queries_function(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L275) — Test the get_all_queries function
  - `test_get_query_function(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L261) — Test the get_query function
  - `test_imports_query_exists(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L53) — Test that IMPORTS query is defined
  - `test_imports_query_patterns(self)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L207) — Test that IMPORTS query contains expected patterns
  - `test_interfaces_query_exists(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L29) — Test that INTERFACES query is defined
  - `test_interfaces_query_patterns(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L162) — Test that INTERFACES query contains expected patterns
  - `test_list_queries_function(self)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L284) — Test the list_queries function
  - `test_query_descriptions_quality(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L342) — Test that query descriptions are meaningful
  - `test_query_syntax_validity(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L297) — Test that queries have valid Tree-sitter syntax
  - `test_signatures_query_exists(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L77) — Test that SIGNATURES query is defined
  - `test_signatures_query_patterns(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L249) — Test that SIGNATURES query contains expected patterns
  - `test_type_aliases_query_exists(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L35) — Test that TYPE_ALIASES query is defined
  - `test_type_aliases_query_patterns(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L173) — Test that TYPE_ALIASES query contains expected patterns
  - `test_typescript_specific_features(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L318) — Test that TypeScript-specific features are covered in queries
  - `test_variables_query_exists(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L47) — Test that VARIABLES query is defined
  - `test_variables_query_patterns(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_typescript.py#L195) — Test that VARIABLES query contains expected patterns
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/typescript.md#ALL_QUERIES), [`FUNCTIONS`](../../../tree_sitter_analyzer/queries/typescript.md#FUNCTIONS), [`list_queries`](../../../tree_sitter_analyzer/queries/typescript.md#list_queries), [`SIGNATURES`](../../../tree_sitter_analyzer/queries/typescript.md#SIGNATURES), [`TYPE_ALIASES`](../../../tree_sitter_analyzer/queries/typescript.md#TYPE_ALIASES), [`CLASSES`](../../../tree_sitter_analyzer/queries/typescript.md#CLASSES), [`INTERFACES`](../../../tree_sitter_analyzer/queries/typescript.md#INTERFACES), [`DECORATORS`](../../../tree_sitter_analyzer/queries/typescript.md#DECORATORS), [`ENUMS`](../../../tree_sitter_analyzer/queries/typescript.md#ENUMS), [`EXPORTS`](../../../tree_sitter_analyzer/queries/typescript.md#EXPORTS), [`GENERICS`](../../../tree_sitter_analyzer/queries/typescript.md#GENERICS), [`IMPORTS`](../../../tree_sitter_analyzer/queries/typescript.md#IMPORTS), [`VARIABLES`](../../../tree_sitter_analyzer/queries/typescript.md#VARIABLES), [`get_query`](../../../tree_sitter_analyzer/queries/typescript.md#get_query), [`COMMENTS`](../../../tree_sitter_analyzer/queries/typescript.md#COMMENTS), [`get_all_queries`](../../../tree_sitter_analyzer/queries/typescript.md#get_all_queries)

