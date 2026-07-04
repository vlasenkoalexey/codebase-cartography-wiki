---
title: 'Module: tests/unit/core/test_database_kuzu_compat.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_database_kuzu_compat.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.core.test_database_kuzu_compat`/
symbols:
  _FakeConn.queries: _FakeConn#queries.
  _FakeConn: _FakeConn#
  _FakeConn.execute: _FakeConn#execute().
  test_rewrites_module_deps_query_for_kuzu_scope_and_ordering: test_rewrites_module_deps_query_for_kuzu_scope_and_ordering().
  test_rewrites_coimports_order_by_alias: test_rewrites_coimports_order_by_alias().
  test_fail_fast_disables_query_type_after_first_known_compat_error: test_fail_fast_disables_query_type_after_first_known_compat_error().
  test_fulltext_index_procedure_becomes_noop: test_fulltext_index_procedure_becomes_noop().
  test_fulltext_query_rewrites_to_substring_search: test_fulltext_query_rewrites_to_substring_search().
  test_import_batch_rewrite_sets_missing_full_import_name: test_import_batch_rewrite_sets_missing_full_import_name().
  test_unwind_uid_injection_uses_fallback_for_missing_pk_fields: test_unwind_uid_injection_uses_fallback_for_missing_pk_fields().
  _make_importers_query: _make_importers_query().
  test_inheritance_queries_bypass_fail_fast_guard: test_inheritance_queries_bypass_fail_fast_guard().
  _FakeConn.fail_with: _FakeConn#fail_with.
  _FakeRawResult: _FakeRawResult#
  _make_coimports_query: _make_coimports_query().
  _FakeRawResult.get_column_names: _FakeRawResult#get_column_names().
  _FakeRawResult.has_next: _FakeRawResult#has_next().
  _FakeRawResult.get_next: _FakeRawResult#get_next().
  _FakeConn.__init__: _FakeConn#__init__().
  test_sanitize_value_normalizes_list_of_dict_keys_for_unwind_batches: test_sanitize_value_normalizes_list_of_dict_keys_for_unwind_batches().
  test_sanitize_value_deduplicates_identical_batch_rows: test_sanitize_value_deduplicates_identical_batch_rows().
---
# Module: [`tests/unit/core/test_database_kuzu_compat.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py)

## Classes
### `_FakeConn`
- def: [`tests/unit/core/test_database_kuzu_compat.py:13`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L13)
- signature: `class _FakeConn:`
- members:
  - `execute(self, query, params)` — [`L18`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L18)
  - `fail_with` — [`L16`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L16)
  - `queries` — [`L15`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L15)
- protocol/private: `__init__`[`L14`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L14)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (8 test-only callers)

### `_FakeRawResult`
- def: [`tests/unit/core/test_database_kuzu_compat.py:3`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L3)
- signature: `class _FakeRawResult:`
- members:
  - `get_column_names(self)` — [`L4`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L4)
  - `get_next(self)` — [`L10`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L10)
  - `has_next(self)` — [`L7`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L7)
- used by: (1 test-only callers)

## Functions
- `_make_coimports_query()` — [`L40`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L40)
- `_make_importers_query()` — [`L25`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L25)
- `test_fail_fast_disables_query_type_after_first_known_compat_error()` — [`L113`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L113)
- `test_fulltext_index_procedure_becomes_noop()` — [`L76`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L76)
- `test_fulltext_query_rewrites_to_substring_search()` — [`L86`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L86)
- `test_import_batch_rewrite_sets_missing_full_import_name()` — [`L153`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L153)
- `test_inheritance_queries_bypass_fail_fast_guard()` — [`L202`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L202)
- `test_rewrites_coimports_order_by_alias()` — [`L66`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L66)
- `test_rewrites_module_deps_query_for_kuzu_scope_and_ordering()` — [`L53`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L53)
- `test_sanitize_value_deduplicates_identical_batch_rows()` — [`L142`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L142)
- `test_sanitize_value_normalizes_list_of_dict_keys_for_unwind_batches()` — [`L126`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L126)
- `test_unwind_uid_injection_uses_fallback_for_missing_pk_fields()` — [`L178`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_database_kuzu_compat.py#L178)

