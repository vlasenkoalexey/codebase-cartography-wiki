---
title: 'Module: tests/unit/languages/test_rust_queries.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_rust_queries.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_rust_queries`/Test
symbols:
  TestRustQueryDescriptions.test_all_queries_have_descriptions: RustQueryDescriptions#test_all_queries_have_descriptions().
  TestGetRustQuery.test_get_all_queries: GetRustQuery#test_get_all_queries().
  TestGetRustQueryDescription.test_get_all_descriptions: GetRustQueryDescription#test_get_all_descriptions().
  TestAllQueries.test_contains_all_rust_queries: AllQueries#test_contains_all_rust_queries().
  TestGetAllQueries.test_returns_all_queries: GetAllQueries#test_returns_all_queries().
  TestListQueries.test_contains_all_query_names: ListQueries#test_contains_all_query_names().
  TestGetAvailableRustQueries.test_contains_all_query_names: GetAvailableRustQueries#test_contains_all_query_names().
  TestRustQueriesDict.test_rust_queries_is_dict: RustQueriesDict#test_rust_queries_is_dict().
  TestRustQueriesDict.test_rust_queries_not_empty: RustQueriesDict#test_rust_queries_not_empty().
  TestRustQueriesDict.test_all_queries_are_strings: RustQueriesDict#test_all_queries_are_strings().
  TestRustQueriesDict.test_all_queries_not_empty: RustQueriesDict#test_all_queries_not_empty().
  TestRustQueriesContent.test_mod_query_exists: RustQueriesContent#test_mod_query_exists().
  TestRustQueriesContent.test_struct_query_exists: RustQueriesContent#test_struct_query_exists().
  TestRustQueriesContent.test_enum_query_exists: RustQueriesContent#test_enum_query_exists().
  TestRustQueriesContent.test_trait_query_exists: RustQueriesContent#test_trait_query_exists().
  TestRustQueriesContent.test_impl_query_exists: RustQueriesContent#test_impl_query_exists().
  TestRustQueriesContent.test_fn_query_exists: RustQueriesContent#test_fn_query_exists().
  TestRustQueriesContent.test_const_query_exists: RustQueriesContent#test_const_query_exists().
  TestRustQueriesContent.test_static_query_exists: RustQueriesContent#test_static_query_exists().
  TestRustQueriesContent.test_macro_query_exists: RustQueriesContent#test_macro_query_exists().
  TestRustQueriesContent.test_attribute_query_exists: RustQueriesContent#test_attribute_query_exists().
  TestRustQueriesContent.test_field_query_exists: RustQueriesContent#test_field_query_exists().
  TestRustQueriesContent.test_enum_variant_query_exists: RustQueriesContent#test_enum_variant_query_exists().
  TestRustQueryDescriptions.test_descriptions_is_dict: RustQueryDescriptions#test_descriptions_is_dict().
  TestRustQueryDescriptions.test_descriptions_not_empty: RustQueryDescriptions#test_descriptions_not_empty().
  TestRustQueryDescriptions.test_all_descriptions_are_strings: RustQueryDescriptions#test_all_descriptions_are_strings().
  TestGetRustQuery.test_get_valid_query: GetRustQuery#test_get_valid_query().
  TestGetRustQuery.test_invalid_query_raises_error: GetRustQuery#test_invalid_query_raises_error().
  TestGetRustQueryDescription.test_get_valid_description: GetRustQueryDescription#test_get_valid_description().
  TestGetRustQueryDescription.test_invalid_query_returns_default: GetRustQueryDescription#test_invalid_query_returns_default().
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
  TestGetAvailableRustQueries.test_returns_list: GetAvailableRustQueries#test_returns_list().
  TestGetAvailableRustQueries.test_not_empty: GetAvailableRustQueries#test_not_empty().
  TestGetAvailableRustQueries.test_no_duplicates: GetAvailableRustQueries#test_no_duplicates().
  TestRustQueriesDict: RustQueriesDict#
  TestRustQueriesContent: RustQueriesContent#
  TestRustQueryDescriptions: RustQueryDescriptions#
  TestGetRustQuery: GetRustQuery#
  TestGetRustQueryDescription: GetRustQueryDescription#
  TestAllQueries: AllQueries#
  TestGetQuery: GetQuery#
  TestGetAllQueries: GetAllQueries#
  TestListQueries: ListQueries#
  TestGetAvailableRustQueries: GetAvailableRustQueries#
---
# Module: [`tests/unit/languages/test_rust_queries.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py)

## Classes
### `TestAllQueries`
- def: [`tests/unit/languages/test_rust_queries.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L173)
- doc: Tests for ALL_QUERIES dictionary.
- signature: `class TestAllQueries:`
- members:
  - `test_all_queries_is_dict(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L176) — ALL_QUERIES should be a dictionary.
  - `test_all_queries_not_empty(self)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L180) — ALL_QUERIES should not be empty.
  - `test_all_queries_structure(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L184) — ALL_QUERIES should have correct structure.
  - `test_contains_aliases(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L196) — ALL_QUERIES should contain common aliases.
  - `test_contains_all_rust_queries(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L191) — ALL_QUERIES should contain all RUST_QUERIES.
- uses (calls/refs, reference-scoped): [`RUST_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERIES.RUST_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#ALL_QUERIES)

### `TestGetAllQueries`
- def: [`tests/unit/languages/test_rust_queries.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L225)
- doc: Tests for get_all_queries function.
- signature: `class TestGetAllQueries:`
- members:
  - `test_returns_all_queries(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L233) — get_all_queries should return ALL_QUERIES.
  - `test_returns_dict(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L228) — get_all_queries should return a dictionary.
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#ALL_QUERIES), [`get_all_queries`](../../../tree_sitter_analyzer/queries/rust.md#get_all_queries)

### `TestGetAvailableRustQueries`
- def: [`tests/unit/languages/test_rust_queries.py:259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L259)
- doc: Tests for get_available_rust_queries function.
- signature: `class TestGetAvailableRustQueries:`
- members:
  - `test_contains_all_query_names(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L272) — get_available_rust_queries should contain all RUST_QUERIES names.
  - `test_no_duplicates(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L278) — get_available_rust_queries should have no duplicates.
  - `test_not_empty(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L267) — get_available_rust_queries should not be empty.
  - `test_returns_list(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L262) — get_available_rust_queries should return a list.
- uses (calls/refs, reference-scoped): [`RUST_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERIES.RUST_QUERIES), [`get_available_rust_queries`](../../../tree_sitter_analyzer/queries/rust.md#get_available_rust_queries)

### `TestGetQuery`
- def: [`tests/unit/languages/test_rust_queries.py:203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L203)
- doc: Tests for get_query function.
- signature: `class TestGetQuery:`
- members:
  - `test_get_alias_query(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L212) — get_query should work for aliases.
  - `test_get_valid_query(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L206) — get_query should return query for valid name.
  - `test_invalid_query_raises_error(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L218) — get_query should raise ValueError for invalid name.
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/rust.md#get_query)

### `TestGetRustQuery`
- def: [`tests/unit/languages/test_rust_queries.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L128)
- doc: Tests for get_rust_query function.
- signature: `class TestGetRustQuery:`
- members:
  - `test_get_all_queries(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L137) — get_rust_query should work for all defined queries.
  - `test_get_valid_query(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L131) — get_rust_query should return query for valid name.
  - `test_invalid_query_raises_error(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L144) — get_rust_query should raise ValueError for invalid name.
- uses (calls/refs, reference-scoped): [`RUST_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERIES.RUST_QUERIES), [`get_rust_query`](../../../tree_sitter_analyzer/queries/rust.md#get_rust_query)

### `TestGetRustQueryDescription`
- def: [`tests/unit/languages/test_rust_queries.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L152)
- doc: Tests for get_rust_query_description function.
- signature: `class TestGetRustQueryDescription:`
- members:
  - `test_get_all_descriptions(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L161) — get_rust_query_description should work for all defined queries.
  - `test_get_valid_description(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L155) — get_rust_query_description should return description for valid name.
  - `test_invalid_query_returns_default(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L167) — get_rust_query_description should return default for invalid name.
- uses (calls/refs, reference-scoped): [`RUST_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERIES.RUST_QUERIES), [`get_rust_query_description`](../../../tree_sitter_analyzer/queries/rust.md#get_rust_query_description)

### `TestListQueries`
- def: [`tests/unit/languages/test_rust_queries.py:239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L239)
- doc: Tests for list_queries function.
- signature: `class TestListQueries:`
- members:
  - `test_contains_all_query_names(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L252) — list_queries should contain all query names.
  - `test_not_empty(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L247) — list_queries should not be empty.
  - `test_returns_list(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L242) — list_queries should return a list.
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#ALL_QUERIES), [`list_queries`](../../../tree_sitter_analyzer/queries/rust.md#list_queries)

### `TestRustQueriesContent`
- def: [`tests/unit/languages/test_rust_queries.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L40)
- doc: Tests for Rust query content.
- signature: `class TestRustQueriesContent:`
- members:
  - `test_attribute_query_exists(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L88) — Attribute query should exist.
  - `test_const_query_exists(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L73) — Const query should exist.
  - `test_enum_query_exists(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L53) — Enum query should exist.
  - `test_enum_variant_query_exists(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L98) — Enum variant query should exist.
  - `test_field_query_exists(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L93) — Field query should exist.
  - `test_fn_query_exists(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L68) — Function query should exist.
  - `test_impl_query_exists(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L63) — Impl query should exist.
  - `test_macro_query_exists(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L83) — Macro query should exist.
  - `test_mod_query_exists(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L43) — Module query should exist.
  - `test_static_query_exists(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L78) — Static query should exist.
  - `test_struct_query_exists(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L48) — Struct query should exist.
  - `test_trait_query_exists(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L58) — Trait query should exist.
- uses (calls/refs, reference-scoped): [`RUST_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERIES.RUST_QUERIES)

### `TestRustQueriesDict`
- def: [`tests/unit/languages/test_rust_queries.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L18)
- doc: Tests for RUST_QUERIES dictionary.
- signature: `class TestRustQueriesDict:`
- members:
  - `test_all_queries_are_strings(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L29) — All query values should be strings.
  - `test_all_queries_not_empty(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L34) — All query values should not be empty.
  - `test_rust_queries_is_dict(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L21) — RUST_QUERIES should be a dictionary.
  - `test_rust_queries_not_empty(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L25) — RUST_QUERIES should not be empty.
- uses (calls/refs, reference-scoped): [`RUST_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERIES.RUST_QUERIES)

### `TestRustQueryDescriptions`
- def: [`tests/unit/languages/test_rust_queries.py:104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L104)
- doc: Tests for RUST_QUERY_DESCRIPTIONS dictionary.
- signature: `class TestRustQueryDescriptions:`
- members:
  - `test_all_descriptions_are_strings(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L115) — All description values should be strings.
  - `test_all_queries_have_descriptions(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L120) — All queries should have descriptions.
  - `test_descriptions_is_dict(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L107) — RUST_QUERY_DESCRIPTIONS should be a dictionary.
  - `test_descriptions_not_empty(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_queries.py#L111) — RUST_QUERY_DESCRIPTIONS should not be empty.
- uses (calls/refs, reference-scoped): [`RUST_QUERIES`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERIES.RUST_QUERIES), [`RUST_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/rust.md#RUST_QUERY_DESCRIPTIONS.RUST_QUERY_DESCRIPTIONS)

