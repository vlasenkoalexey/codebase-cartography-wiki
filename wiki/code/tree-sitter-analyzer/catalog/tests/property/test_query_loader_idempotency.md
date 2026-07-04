---
title: 'Module: tests/property/test_query_loader_idempotency.py'
type: catalog
provenance: extracted
module: tests/property/test_query_loader_idempotency.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.property.test_query_loader_idempotency`/TestQueryIdempotency#
symbols:
  TestQueryIdempotency.test_get_query_deterministic: test_get_query_deterministic().
  TestQueryIdempotency.test_is_language_supported_consistent: test_is_language_supported_consistent().
  TestQueryIdempotency.test_list_queries_non_empty: test_list_queries_non_empty().
  TestQueryIdempotency.test_get_all_queries_has_tuples: test_get_all_queries_has_tuples().
  TestQueryIdempotency: ''
---
# Module: [`tests/property/test_query_loader_idempotency.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_loader_idempotency.py)

## Classes
### `TestQueryIdempotency`
- def: [`tests/property/test_query_loader_idempotency.py:10`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_loader_idempotency.py#L10)
- doc: get_query is deterministic for known key-language pairs.
- signature: `class TestQueryIdempotency:`
- members:
  - `test_get_all_queries_has_tuples(self, language)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_loader_idempotency.py#L38)
  - `test_get_query_deterministic(self, language, query_key)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_loader_idempotency.py#L17)
  - `test_is_language_supported_consistent(self, language)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_loader_idempotency.py#L24)
  - `test_list_queries_non_empty(self, language)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_query_loader_idempotency.py#L31)
- uses (calls/refs, reference-scoped): [`QueryLoader`](../../tree_sitter_analyzer/query_loader.md#QueryLoader), [`get_query`](../../tree_sitter_analyzer/query_loader.md#QueryLoader.get_query), [`is_language_supported`](../../tree_sitter_analyzer/query_loader.md#QueryLoader.is_language_supported), [`list_queries_for_language`](../../tree_sitter_analyzer/query_loader.md#QueryLoader.list_queries_for_language), [`get_all_queries_for_language`](../../tree_sitter_analyzer/query_loader.md#QueryLoader.get_all_queries_for_language)

