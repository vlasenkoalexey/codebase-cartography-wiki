---
title: 'Module: tests/unit/languages/test_go_queries.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_queries.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_queries`/Test
symbols:
  TestGoQueryDescriptions.test_all_queries_have_descriptions: GoQueryDescriptions#test_all_queries_have_descriptions().
  TestGetGoQuery.test_get_all_queries: GetGoQuery#test_get_all_queries().
  TestGetGoQueryDescription.test_get_all_descriptions: GetGoQueryDescription#test_get_all_descriptions().
  TestAllQueries.test_contains_all_go_queries: AllQueries#test_contains_all_go_queries().
  TestGetAllQueries.test_returns_all_queries: GetAllQueries#test_returns_all_queries().
  TestListQueries.test_contains_all_query_names: ListQueries#test_contains_all_query_names().
  TestGetAvailableGoQueries.test_contains_all_query_names: GetAvailableGoQueries#test_contains_all_query_names().
  TestGoQueriesDict.test_go_queries_is_dict: GoQueriesDict#test_go_queries_is_dict().
  TestGoQueriesDict.test_go_queries_not_empty: GoQueriesDict#test_go_queries_not_empty().
  TestGoQueriesDict.test_all_queries_are_strings: GoQueriesDict#test_all_queries_are_strings().
  TestGoQueriesDict.test_all_queries_not_empty: GoQueriesDict#test_all_queries_not_empty().
  TestGoQueriesContent.test_package_query_exists: GoQueriesContent#test_package_query_exists().
  TestGoQueriesContent.test_import_query_exists: GoQueriesContent#test_import_query_exists().
  TestGoQueriesContent.test_function_query_exists: GoQueriesContent#test_function_query_exists().
  TestGoQueriesContent.test_method_query_exists: GoQueriesContent#test_method_query_exists().
  TestGoQueriesContent.test_struct_query_exists: GoQueriesContent#test_struct_query_exists().
  TestGoQueriesContent.test_interface_query_exists: GoQueriesContent#test_interface_query_exists().
  TestGoQueriesContent.test_const_query_exists: GoQueriesContent#test_const_query_exists().
  TestGoQueriesContent.test_var_query_exists: GoQueriesContent#test_var_query_exists().
  TestGoQueriesContent.test_goroutine_query_exists: GoQueriesContent#test_goroutine_query_exists().
  TestGoQueriesContent.test_defer_query_exists: GoQueriesContent#test_defer_query_exists().
  TestGoQueriesContent.test_select_query_exists: GoQueriesContent#test_select_query_exists().
  TestGoQueriesContent.test_comment_query_exists: GoQueriesContent#test_comment_query_exists().
  TestGoQueryDescriptions.test_descriptions_is_dict: GoQueryDescriptions#test_descriptions_is_dict().
  TestGoQueryDescriptions.test_descriptions_not_empty: GoQueryDescriptions#test_descriptions_not_empty().
  TestGoQueryDescriptions.test_all_descriptions_are_strings: GoQueryDescriptions#test_all_descriptions_are_strings().
  TestGetGoQuery.test_get_valid_query: GetGoQuery#test_get_valid_query().
  TestGetGoQuery.test_invalid_query_raises_error: GetGoQuery#test_invalid_query_raises_error().
  TestGetGoQueryDescription.test_get_valid_description: GetGoQueryDescription#test_get_valid_description().
  TestGetGoQueryDescription.test_invalid_query_returns_default: GetGoQueryDescription#test_invalid_query_returns_default().
  TestAllQueries.test_all_queries_is_dict: AllQueries#test_all_queries_is_dict().
  TestAllQueries.test_all_queries_not_empty: AllQueries#test_all_queries_not_empty().
  TestAllQueries.test_all_queries_structure: AllQueries#test_all_queries_structure().
  TestAllQueries.test_contains_aliases: AllQueries#test_contains_aliases().
  TestGetQuery.test_get_valid_query: GetQuery#test_get_valid_query().
  TestGetQuery.test_get_alias_query: GetQuery#test_get_alias_query().
  TestGetQuery.test_invalid_query_raises_error: GetQuery#test_invalid_query_raises_error().
  TestGetAllQueries.test_returns_dict: GetAllQueries#test_returns_dict().
  TestListQueries.test_returns_list: ListQueries#test_returns_list().
  TestListQueries.test_not_empty: ListQueries#test_not_empty().
  TestGetAvailableGoQueries.test_returns_list: GetAvailableGoQueries#test_returns_list().
  TestGetAvailableGoQueries.test_not_empty: GetAvailableGoQueries#test_not_empty().
  TestGetAvailableGoQueries.test_no_duplicates: GetAvailableGoQueries#test_no_duplicates().
  TestGoQueriesDict: GoQueriesDict#
  TestGoQueriesContent: GoQueriesContent#
  TestGoQueryDescriptions: GoQueryDescriptions#
  TestGetGoQuery: GetGoQuery#
  TestGetGoQueryDescription: GetGoQueryDescription#
  TestAllQueries: AllQueries#
  TestGetQuery: GetQuery#
  TestGetAllQueries: GetAllQueries#
  TestListQueries: ListQueries#
  TestGetAvailableGoQueries: GetAvailableGoQueries#
---
# Module: [`tests/unit/languages/test_go_queries.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py)

## Classes
### `TestAllQueries`
- def: [`tests/unit/languages/test_go_queries.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L173)
- doc: Tests for ALL_QUERIES dictionary.
- signature: `class TestAllQueries:`
- members:
  - `test_all_queries_is_dict(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L176) — ALL_QUERIES should be a dictionary.
  - `test_all_queries_not_empty(self)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L180) — ALL_QUERIES should not be empty.
  - `test_all_queries_structure(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L184) — ALL_QUERIES should have correct structure.
  - `test_contains_aliases(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L196) — ALL_QUERIES should contain common aliases.
  - `test_contains_all_go_queries(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L191) — ALL_QUERIES should contain all GO_QUERIES.
- uses (calls/refs, reference-scoped): [`GO_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERIES.GO_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#ALL_QUERIES)

### `TestGetAllQueries`
- def: [`tests/unit/languages/test_go_queries.py:227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L227)
- doc: Tests for get_all_queries function.
- signature: `class TestGetAllQueries:`
- members:
  - `test_returns_all_queries(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L235) — get_all_queries should return ALL_QUERIES.
  - `test_returns_dict(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L230) — get_all_queries should return a dictionary.
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#ALL_QUERIES), [`get_all_queries`](../../../tree_sitter_analyzer/queries/go.md#get_all_queries)

### `TestGetAvailableGoQueries`
- def: [`tests/unit/languages/test_go_queries.py:261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L261)
- doc: Tests for get_available_go_queries function.
- signature: `class TestGetAvailableGoQueries:`
- members:
  - `test_contains_all_query_names(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L274) — get_available_go_queries should contain all GO_QUERIES names.
  - `test_no_duplicates(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L280) — get_available_go_queries should have no duplicates.
  - `test_not_empty(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L269) — get_available_go_queries should not be empty.
  - `test_returns_list(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L264) — get_available_go_queries should return a list.
- uses (calls/refs, reference-scoped): [`GO_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERIES.GO_QUERIES), [`get_available_go_queries`](../../../tree_sitter_analyzer/queries/go.md#get_available_go_queries)

### `TestGetGoQuery`
- def: [`tests/unit/languages/test_go_queries.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L128)
- doc: Tests for get_go_query function.
- signature: `class TestGetGoQuery:`
- members:
  - `test_get_all_queries(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L137) — get_go_query should work for all defined queries.
  - `test_get_valid_query(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L131) — get_go_query should return query for valid name.
  - `test_invalid_query_raises_error(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L144) — get_go_query should raise ValueError for invalid name.
- uses (calls/refs, reference-scoped): [`GO_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERIES.GO_QUERIES), [`get_go_query`](../../../tree_sitter_analyzer/queries/go.md#get_go_query)

### `TestGetGoQueryDescription`
- def: [`tests/unit/languages/test_go_queries.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L152)
- doc: Tests for get_go_query_description function.
- signature: `class TestGetGoQueryDescription:`
- members:
  - `test_get_all_descriptions(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L161) — get_go_query_description should work for all defined queries.
  - `test_get_valid_description(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L155) — get_go_query_description should return description for valid name.
  - `test_invalid_query_returns_default(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L167) — get_go_query_description should return default for invalid name.
- uses (calls/refs, reference-scoped): [`GO_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERIES.GO_QUERIES), [`get_go_query_description`](../../../tree_sitter_analyzer/queries/go.md#get_go_query_description)

### `TestGetQuery`
- def: [`tests/unit/languages/test_go_queries.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L205)
- doc: Tests for get_query function.
- signature: `class TestGetQuery:`
- members:
  - `test_get_alias_query(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L214) — get_query should work for aliases.
  - `test_get_valid_query(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L208) — get_query should return query for valid name.
  - `test_invalid_query_raises_error(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L220) — get_query should raise ValueError for invalid name.
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/go.md#get_query)

### `TestGoQueriesContent`
- def: [`tests/unit/languages/test_go_queries.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L40)
- doc: Tests for Go query content.
- signature: `class TestGoQueriesContent:`
- members:
  - `test_comment_query_exists(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L98) — Comment query should exist.
  - `test_const_query_exists(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L73) — Const query should exist.
  - `test_defer_query_exists(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L88) — Defer query should exist.
  - `test_function_query_exists(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L53) — Function query should exist.
  - `test_goroutine_query_exists(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L83) — Goroutine query should exist.
  - `test_import_query_exists(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L48) — Import query should exist.
  - `test_interface_query_exists(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L68) — Interface query should exist.
  - `test_method_query_exists(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L58) — Method query should exist.
  - `test_package_query_exists(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L43) — Package query should exist.
  - `test_select_query_exists(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L93) — Select query should exist.
  - `test_struct_query_exists(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L63) — Struct query should exist.
  - `test_var_query_exists(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L78) — Var query should exist.
- uses (calls/refs, reference-scoped): [`GO_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERIES.GO_QUERIES)

### `TestGoQueriesDict`
- def: [`tests/unit/languages/test_go_queries.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L18)
- doc: Tests for GO_QUERIES dictionary.
- signature: `class TestGoQueriesDict:`
- members:
  - `test_all_queries_are_strings(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L29) — All query values should be strings.
  - `test_all_queries_not_empty(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L34) — All query values should not be empty.
  - `test_go_queries_is_dict(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L21) — GO_QUERIES should be a dictionary.
  - `test_go_queries_not_empty(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L25) — GO_QUERIES should not be empty.
- uses (calls/refs, reference-scoped): [`GO_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERIES.GO_QUERIES)

### `TestGoQueryDescriptions`
- def: [`tests/unit/languages/test_go_queries.py:104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L104)
- doc: Tests for GO_QUERY_DESCRIPTIONS dictionary.
- signature: `class TestGoQueryDescriptions:`
- members:
  - `test_all_descriptions_are_strings(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L115) — All description values should be strings.
  - `test_all_queries_have_descriptions(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L120) — All queries should have descriptions.
  - `test_descriptions_is_dict(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L107) — GO_QUERY_DESCRIPTIONS should be a dictionary.
  - `test_descriptions_not_empty(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L111) — GO_QUERY_DESCRIPTIONS should not be empty.
- uses (calls/refs, reference-scoped): [`GO_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERIES.GO_QUERIES), [`GO_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/go.md#GO_QUERY_DESCRIPTIONS.GO_QUERY_DESCRIPTIONS)

### `TestListQueries`
- def: [`tests/unit/languages/test_go_queries.py:241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L241)
- doc: Tests for list_queries function.
- signature: `class TestListQueries:`
- members:
  - `test_contains_all_query_names(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L254) — list_queries should contain all query names.
  - `test_not_empty(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L249) — list_queries should not be empty.
  - `test_returns_list(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_queries.py#L244) — list_queries should return a list.
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/go.md#ALL_QUERIES), [`list_queries`](../../../tree_sitter_analyzer/queries/go.md#list_queries)

