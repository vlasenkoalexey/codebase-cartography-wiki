---
title: 'Module: tests/unit/languages/test_kotlin_queries.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_queries.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_queries`/Test
symbols:
  TestKotlinQueries.test_query_descriptions_exist: KotlinQueries#test_query_descriptions_exist().
  TestGetAllQueries.test_returns_all_queries: GetAllQueries#test_returns_all_queries().
  TestGetAvailableKotlinQueries.test_returns_kotlin_query_keys: GetAvailableKotlinQueries#test_returns_kotlin_query_keys().
  TestKotlinQueries.test_kotlin_queries_not_empty: KotlinQueries#test_kotlin_queries_not_empty().
  TestKotlinQueries.test_all_queries_not_empty: KotlinQueries#test_all_queries_not_empty().
  TestKotlinQueries.test_kotlin_query_keys: KotlinQueries#test_kotlin_query_keys().
  TestKotlinQueries.test_all_queries_has_common_aliases: KotlinQueries#test_all_queries_has_common_aliases().
  TestGetKotlinQuery.test_get_existing_query: GetKotlinQuery#test_get_existing_query().
  TestGetKotlinQuery.test_get_function_query: GetKotlinQuery#test_get_function_query().
  TestGetKotlinQuery.test_get_property_query: GetKotlinQuery#test_get_property_query().
  TestGetKotlinQuery.test_get_nonexistent_query_raises: GetKotlinQuery#test_get_nonexistent_query_raises().
  TestGetKotlinQuery.test_get_data_class_query: GetKotlinQuery#test_get_data_class_query().
  TestGetKotlinQuery.test_get_suspend_function_query: GetKotlinQuery#test_get_suspend_function_query().
  TestGetKotlinQueryDescription.test_get_existing_description: GetKotlinQueryDescription#test_get_existing_description().
  TestGetKotlinQueryDescription.test_get_function_description: GetKotlinQueryDescription#test_get_function_description().
  TestGetKotlinQueryDescription.test_get_nonexistent_description_returns_default: GetKotlinQueryDescription#test_get_nonexistent_description_returns_default().
  TestGetQuery.test_get_query_from_all_queries: GetQuery#test_get_query_from_all_queries().
  TestGetQuery.test_get_alias_query: GetQuery#test_get_alias_query().
  TestGetQuery.test_get_classes_alias: GetQuery#test_get_classes_alias().
  TestGetQuery.test_get_nonexistent_raises: GetQuery#test_get_nonexistent_raises().
  TestGetAllQueries.test_returns_dict: GetAllQueries#test_returns_dict().
  TestGetAllQueries.test_queries_have_correct_structure: GetAllQueries#test_queries_have_correct_structure().
  TestListQueries.test_returns_list: ListQueries#test_returns_list().
  TestListQueries.test_contains_expected_queries: ListQueries#test_contains_expected_queries().
  TestListQueries.test_contains_aliases: ListQueries#test_contains_aliases().
  TestGetAvailableKotlinQueries.test_returns_list: GetAvailableKotlinQueries#test_returns_list().
  TestGetAvailableKotlinQueries.test_does_not_include_aliases: GetAvailableKotlinQueries#test_does_not_include_aliases().
  TestQueryContent.test_class_query_syntax: QueryContent#test_class_query_syntax().
  TestQueryContent.test_function_query_syntax: QueryContent#test_function_query_syntax().
  TestQueryContent.test_package_query_syntax: QueryContent#test_package_query_syntax().
  TestQueryContent.test_annotation_query_syntax: QueryContent#test_annotation_query_syntax().
  TestKotlinQueries: KotlinQueries#
  TestGetKotlinQuery: GetKotlinQuery#
  TestGetKotlinQueryDescription: GetKotlinQueryDescription#
  TestGetQuery: GetQuery#
  TestGetAllQueries: GetAllQueries#
  TestListQueries: ListQueries#
  TestGetAvailableKotlinQueries: GetAvailableKotlinQueries#
  TestQueryContent: QueryContent#
---
# Module: [`tests/unit/languages/test_kotlin_queries.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py)

## Classes
### `TestGetAllQueries`
- def: [`tests/unit/languages/test_kotlin_queries.py:147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L147)
- doc: Test get_all_queries function.
- signature: `class TestGetAllQueries:`
- members:
  - `test_queries_have_correct_structure(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L160) — Test that each query has correct structure.
  - `test_returns_all_queries(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L155) — Test that all queries are returned.
  - `test_returns_dict(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L150) — Test that get_all_queries returns a dict.
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/kotlin.md#ALL_QUERIES), [`get_all_queries`](../../../tree_sitter_analyzer/queries/kotlin.md#get_all_queries)

### `TestGetAvailableKotlinQueries`
- def: [`tests/unit/languages/test_kotlin_queries.py:191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L191)
- doc: Test get_available_kotlin_queries function.
- signature: `class TestGetAvailableKotlinQueries:`
- members:
  - `test_does_not_include_aliases(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L204) — Test that aliases are not included.
  - `test_returns_kotlin_query_keys(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L199) — Test that function returns KOTLIN_QUERIES keys.
  - `test_returns_list(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L194) — Test that function returns a list.
- uses (calls/refs, reference-scoped): [`KOTLIN_QUERIES`](../../../tree_sitter_analyzer/queries/kotlin.md#KOTLIN_QUERIES.KOTLIN_QUERIES), [`get_available_kotlin_queries`](../../../tree_sitter_analyzer/queries/kotlin.md#get_available_kotlin_queries)

### `TestGetKotlinQuery`
- def: [`tests/unit/languages/test_kotlin_queries.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L58)
- doc: Test get_kotlin_query function.
- signature: `class TestGetKotlinQuery:`
- members:
  - `test_get_data_class_query(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L86) — Test getting data class query.
  - `test_get_existing_query(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L61) — Test getting an existing query.
  - `test_get_function_query(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L68) — Test getting function query.
  - `test_get_nonexistent_query_raises(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L78) — Test that nonexistent query raises ValueError.
  - `test_get_property_query(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L73) — Test getting property query.
  - `test_get_suspend_function_query(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L91) — Test getting suspend function query.
- uses (calls/refs, reference-scoped): [`get_kotlin_query`](../../../tree_sitter_analyzer/queries/kotlin.md#get_kotlin_query)

### `TestGetKotlinQueryDescription`
- def: [`tests/unit/languages/test_kotlin_queries.py:97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L97)
- doc: Test get_kotlin_query_description function.
- signature: `class TestGetKotlinQueryDescription:`
- members:
  - `test_get_existing_description(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L100) — Test getting description for existing query.
  - `test_get_function_description(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L107) — Test getting function query description.
  - `test_get_nonexistent_description_returns_default(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L112) — Test that nonexistent description returns default.
- uses (calls/refs, reference-scoped): [`get_kotlin_query_description`](../../../tree_sitter_analyzer/queries/kotlin.md#get_kotlin_query_description)

### `TestGetQuery`
- def: [`tests/unit/languages/test_kotlin_queries.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L118)
- doc: Test get_query function.
- signature: `class TestGetQuery:`
- members:
  - `test_get_alias_query(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L127) — Test getting aliased query.
  - `test_get_classes_alias(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L133) — Test getting classes alias.
  - `test_get_nonexistent_raises(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L139) — Test that nonexistent query raises ValueError.
  - `test_get_query_from_all_queries(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L121) — Test getting query from ALL_QUERIES.
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/kotlin.md#get_query)

### `TestKotlinQueries`
- def: [`tests/unit/languages/test_kotlin_queries.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L18)
- doc: Test Kotlin query definitions.
- signature: `class TestKotlinQueries:`
- members:
  - `test_all_queries_has_common_aliases(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L51) — Test that common aliases exist in ALL_QUERIES.
  - `test_all_queries_not_empty(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L25) — Test that ALL_QUERIES is not empty.
  - `test_kotlin_queries_not_empty(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L21) — Test that KOTLIN_QUERIES is not empty.
  - `test_kotlin_query_keys(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L29) — Test that essential queries exist.
  - `test_query_descriptions_exist(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L46) — Test that descriptions exist for queries.
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/kotlin.md#ALL_QUERIES), [`KOTLIN_QUERIES`](../../../tree_sitter_analyzer/queries/kotlin.md#KOTLIN_QUERIES.KOTLIN_QUERIES), [`KOTLIN_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/kotlin.md#KOTLIN_QUERY_DESCRIPTIONS.KOTLIN_QUERY_DESCRIPTIONS)

### `TestListQueries`
- def: [`tests/unit/languages/test_kotlin_queries.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L168)
- doc: Test list_queries function.
- signature: `class TestListQueries:`
- members:
  - `test_contains_aliases(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L183) — Test that list contains aliases.
  - `test_contains_expected_queries(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L176) — Test that list contains expected queries.
  - `test_returns_list(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L171) — Test that list_queries returns a list.
- uses (calls/refs, reference-scoped): [`list_queries`](../../../tree_sitter_analyzer/queries/kotlin.md#list_queries)

### `TestQueryContent`
- def: [`tests/unit/languages/test_kotlin_queries.py:213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L213)
- doc: Test actual query content validity.
- signature: `class TestQueryContent:`
- members:
  - `test_annotation_query_syntax(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L237) — Test that annotation query has valid tree-sitter syntax.
  - `test_class_query_syntax(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L216) — Test that class query has valid tree-sitter syntax.
  - `test_function_query_syntax(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L224) — Test that function query has valid tree-sitter syntax.
  - `test_package_query_syntax(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_queries.py#L231) — Test that package query has valid tree-sitter syntax.
- uses (calls/refs, reference-scoped): [`get_kotlin_query`](../../../tree_sitter_analyzer/queries/kotlin.md#get_kotlin_query)

