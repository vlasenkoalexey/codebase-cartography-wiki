---
title: 'Module: tests/unit/queries/test_markdown_query_registry.py'
type: catalog
provenance: extracted
module: tests/unit/queries/test_markdown_query_registry.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.queries.test_markdown_query_registry`/Test
symbols:
  TestGetAllQueries.test_contains_all_base_queries: GetAllQueries#test_contains_all_base_queries().
  TestGetAllQueries.test_contains_aliases: GetAllQueries#test_contains_aliases().
  TestListQueries.test_includes_base_query_names: ListQueries#test_includes_base_query_names().
  TestListQueries.test_includes_alias_names: ListQueries#test_includes_alias_names().
  TestAllQueriesModuleDict.test_alias_points_to_same_query_as_target: AllQueriesModuleDict#test_alias_points_to_same_query_as_target().
  TestGetAllQueries.test_returns_dict: GetAllQueries#test_returns_dict().
  TestGetAllQueries.test_each_entry_has_query_and_description: GetAllQueries#test_each_entry_has_query_and_description().
  TestListQueries.test_returns_list: ListQueries#test_returns_list().
  TestAllQueriesModuleDict.test_alias_entry_has_description: AllQueriesModuleDict#test_alias_entry_has_description().
  TestGetAllQueries: GetAllQueries#
  TestListQueries: ListQueries#
  TestAllQueriesModuleDict: AllQueriesModuleDict#
---
# Module: [`tests/unit/queries/test_markdown_query_registry.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py)

## Classes
### `TestAllQueriesModuleDict`
- def: [`tests/unit/queries/test_markdown_query_registry.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L48)
- signature: `class TestAllQueriesModuleDict:`
- members:
  - `test_alias_entry_has_description(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L53)
  - `test_alias_points_to_same_query_as_target(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L49)
- uses (calls/refs, reference-scoped): [`MARKDOWN_QUERIES`](../../../tree_sitter_analyzer/queries/markdown.md#MARKDOWN_QUERIES.MARKDOWN_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/markdown.md#ALL_QUERIES.ALL_QUERIES)

### `TestGetAllQueries`
- def: [`tests/unit/queries/test_markdown_query_registry.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L10)
- signature: `class TestGetAllQueries:`
- members:
  - `test_contains_aliases(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L20)
  - `test_contains_all_base_queries(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L15)
  - `test_each_entry_has_query_and_description(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L25)
  - `test_returns_dict(self)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L11)
- uses (calls/refs, reference-scoped): [`MARKDOWN_QUERIES`](../../../tree_sitter_analyzer/queries/markdown.md#MARKDOWN_QUERIES.MARKDOWN_QUERIES), [`QUERY_ALIASES`](../../../tree_sitter_analyzer/queries/markdown.md#QUERY_ALIASES.QUERY_ALIASES), [`get_all_queries`](../../../tree_sitter_analyzer/queries/markdown.md#get_all_queries)

### `TestListQueries`
- def: [`tests/unit/queries/test_markdown_query_registry.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L32)
- signature: `class TestListQueries:`
- members:
  - `test_includes_alias_names(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L42)
  - `test_includes_base_query_names(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L37)
  - `test_returns_list(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/queries/test_markdown_query_registry.py#L33)
- uses (calls/refs, reference-scoped): [`MARKDOWN_QUERIES`](../../../tree_sitter_analyzer/queries/markdown.md#MARKDOWN_QUERIES.MARKDOWN_QUERIES), [`QUERY_ALIASES`](../../../tree_sitter_analyzer/queries/markdown.md#QUERY_ALIASES.QUERY_ALIASES), [`list_queries`](../../../tree_sitter_analyzer/queries/markdown.md#list_queries)

