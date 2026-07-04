---
title: 'Module: tests/unit/core/test_queries_javascript.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_javascript.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_javascript`/TestJavaScriptQuer
symbols:
  TestJavaScriptQueries.test_query_consistency: ies#test_query_consistency().
  TestJavaScriptQueries.test_query_constants: ies#test_query_constants().
  TestJavaScriptQueryFunctions.test_all_queries_built_from_javascript_queries: yFunctions#test_all_queries_built_from_javascript_queries().
  TestJavaScriptQueryFunctions.test_get_javascript_query_all_keys: yFunctions#test_get_javascript_query_all_keys().
  TestJavaScriptQueryFunctions.test_get_javascript_query_description_all_keys: yFunctions#test_get_javascript_query_description_all_keys().
  TestJavaScriptQueryFunctions.test_get_query_through_all_queries: yFunctions#test_get_query_through_all_queries().
  TestJavaScriptQueryFunctions.test_get_all_queries_returns_dict: yFunctions#test_get_all_queries_returns_dict().
  TestJavaScriptQueryFunctions.test_get_available_javascript_queries: yFunctions#test_get_available_javascript_queries().
  TestJavaScriptQueries.test_get_query_valid: ies#test_get_query_valid().
  TestJavaScriptQueries.test_get_query_invalid: ies#test_get_query_invalid().
  TestJavaScriptQueries.test_get_all_queries: ies#test_get_all_queries().
  TestJavaScriptQueries.test_list_queries: ies#test_list_queries().
  TestJavaScriptQueries.test_all_queries_structure: ies#test_all_queries_structure().
  TestJavaScriptQueries.test_functions_query: ies#test_functions_query().
  TestJavaScriptQueries.test_classes_query: ies#test_classes_query().
  TestJavaScriptQueries.test_variables_query: ies#test_variables_query().
  TestJavaScriptQueries.test_imports_query: ies#test_imports_query().
  TestJavaScriptQueries.test_exports_query: ies#test_exports_query().
  TestJavaScriptQueries.test_objects_query: ies#test_objects_query().
  TestJavaScriptQueries.test_comments_query: ies#test_comments_query().
  TestJavaScriptQueries.test_query_descriptions: ies#test_query_descriptions().
  TestJavaScriptQueryFunctions.test_get_javascript_query_returns_string: yFunctions#test_get_javascript_query_returns_string().
  TestJavaScriptQueryFunctions.test_get_javascript_query_invalid_raises: yFunctions#test_get_javascript_query_invalid_raises().
  TestJavaScriptQueryFunctions.test_get_javascript_query_description_known: yFunctions#test_get_javascript_query_description_known().
  TestJavaScriptQueryFunctions.test_get_javascript_query_description_unknown: yFunctions#test_get_javascript_query_description_unknown().
  TestJavaScriptQueryFunctions.test_list_queries_returns_list: yFunctions#test_list_queries_returns_list().
  TestJavaScriptQueries: ies#
  TestJavaScriptQueryFunctions: yFunctions#
---
# Module: [`tests/unit/core/test_queries_javascript.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py)

## Classes
### `TestJavaScriptQueries`
- def: [`tests/unit/core/test_queries_javascript.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L28)
- doc: Test JavaScript queries functionality
- signature: `class TestJavaScriptQueries:`
- members:
  - `test_all_queries_structure(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L63) — Test ALL_QUERIES dictionary structure
  - `test_classes_query(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L91) — Test classes query content
  - `test_comments_query(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L119) — Test comments query content
  - `test_exports_query(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L108) — Test exports query content
  - `test_functions_query(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L84) — Test functions query content
  - `test_get_all_queries(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L46) — Test getting all queries
  - `test_get_query_invalid(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L38) — Test getting an invalid JavaScript query raises ValueError
  - `test_get_query_valid(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L31) — Test getting a valid JavaScript query
  - `test_imports_query(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L102) — Test imports query content
  - `test_list_queries(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L55) — Test listing all query names
  - `test_objects_query(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L114) — Test objects query content
  - `test_query_consistency(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L132) — Test consistency between constants and ALL_QUERIES
  - `test_query_constants(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L77) — Test that query constants are properly defined
  - `test_query_descriptions(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L124) — Test that all queries have meaningful descriptions
  - `test_variables_query(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L96) — Test variables query content
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/javascript.md#ALL_QUERIES), [`VARIABLES`](../../../tree_sitter_analyzer/queries/javascript.md#VARIABLES), [`list_queries`](../../../tree_sitter_analyzer/queries/javascript.md#list_queries), [`FUNCTIONS`](../../../tree_sitter_analyzer/queries/javascript.md#FUNCTIONS), [`get_query`](../../../tree_sitter_analyzer/queries/javascript.md#get_query), [`CLASSES`](../../../tree_sitter_analyzer/queries/javascript.md#CLASSES), [`EXPORTS`](../../../tree_sitter_analyzer/queries/javascript.md#EXPORTS), [`IMPORTS`](../../../tree_sitter_analyzer/queries/javascript.md#IMPORTS), [`COMMENTS`](../../../tree_sitter_analyzer/queries/javascript.md#COMMENTS), [`OBJECTS`](../../../tree_sitter_analyzer/queries/javascript.md#OBJECTS), [`get_all_queries`](../../../tree_sitter_analyzer/queries/javascript.md#get_all_queries)

### `TestJavaScriptQueryFunctions`
- def: [`tests/unit/core/test_queries_javascript.py:144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L144)
- doc: Cover get_javascript_query, get_javascript_query_description, and related functions.
- signature: `class TestJavaScriptQueryFunctions:`
- members:
  - `test_all_queries_built_from_javascript_queries(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L200)
  - `test_get_all_queries_returns_dict(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L183)
  - `test_get_available_javascript_queries(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L193)
  - `test_get_javascript_query_all_keys(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L152)
  - `test_get_javascript_query_description_all_keys(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L172)
  - `test_get_javascript_query_description_known(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L164)
  - `test_get_javascript_query_description_unknown(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L169)
  - `test_get_javascript_query_invalid_raises(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L158)
  - `test_get_javascript_query_returns_string(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L147)
  - `test_get_query_through_all_queries(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L178)
  - `test_list_queries_returns_list(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_javascript.py#L188)
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/javascript.md#ALL_QUERIES), [`JAVASCRIPT_QUERIES`](../../../tree_sitter_analyzer/queries/javascript.md#JAVASCRIPT_QUERIES.JAVASCRIPT_QUERIES), [`JAVASCRIPT_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/javascript.md#JAVASCRIPT_QUERY_DESCRIPTIONS.JAVASCRIPT_QUERY_DESCRIPTIONS), [`get_javascript_query`](../../../tree_sitter_analyzer/queries/javascript.md#get_javascript_query), [`list_queries`](../../../tree_sitter_analyzer/queries/javascript.md#list_queries), [`get_javascript_query_description`](../../../tree_sitter_analyzer/queries/javascript.md#get_javascript_query_description), [`get_available_javascript_queries`](../../../tree_sitter_analyzer/queries/javascript.md#get_available_javascript_queries), [`get_query`](../../../tree_sitter_analyzer/queries/javascript.md#get_query), [`get_all_queries`](../../../tree_sitter_analyzer/queries/javascript.md#get_all_queries)

