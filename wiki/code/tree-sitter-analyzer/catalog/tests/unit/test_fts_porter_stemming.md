---
title: 'Module: tests/unit/test_fts_porter_stemming.py'
type: catalog
provenance: extracted
module: tests/unit/test_fts_porter_stemming.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_fts_porter_stemming`/
symbols:
  TestV12MigrationRebuild.test_existing_cache_rebuilt_with_stemming: TestV12MigrationRebuild#test_existing_cache_rebuilt_with_stemming().
  TestV12MigrationRebuild.test_migration_idempotent_on_second_open: TestV12MigrationRebuild#test_migration_idempotent_on_second_open().
  TestV12MigrationRebuild._build_legacy_db: TestV12MigrationRebuild#_build_legacy_db().
  TestExactTokenQueriesUnchanged.test_exact_identifier_query_identical_old_vs_new: TestExactTokenQueriesUnchanged#test_exact_identifier_query_identical_old_vs_new().
  TestV12MigrationRebuild.test_fresh_cache_end_to_end: TestV12MigrationRebuild#test_fresh_cache_end_to_end().
  TestPorterStemmingRecall.test_dispatching_matches_dispatch_family: TestPorterStemmingRecall#test_dispatching_matches_dispatch_family().
  TestPorterStemmingRecall.test_stemming_does_not_leak_unrelated_symbols: TestPorterStemmingRecall#test_stemming_does_not_leak_unrelated_symbols().
  _make_conn: _make_conn().
  TestPorterStemmingRecall.test_old_tokenizer_misses_dispatching: TestPorterStemmingRecall#test_old_tokenizer_misses_dispatching().
  TestBm25RankingStillApplies.test_relevance_scores_normalized_and_descending: TestBm25RankingStillApplies#test_relevance_scores_normalized_and_descending().
  _c: _c.
  _names: _names().
  TestV12MigrationRebuild.test_migration_degrades_silently_without_fts5: TestV12MigrationRebuild#test_migration_degrades_silently_without_fts5().
  _OLD_FTS_DDL: _OLD_FTS_DDL.
  pytestmark: pytestmark.
  _FTS5_AVAILABLE: _FTS5_AVAILABLE.
  _SYMBOLS: _SYMBOLS.
  TestV12MigrationRebuild.test_migration_degrades_silently_without_fts5._NoFts5Conn: TestV12MigrationRebuild#test_migration_degrades_silently_without_fts5()._NoFts5Conn#
  TestPorterStemmingRecall: TestPorterStemmingRecall#
  TestExactTokenQueriesUnchanged: TestExactTokenQueriesUnchanged#
  TestBm25RankingStillApplies: TestBm25RankingStillApplies#
  TestV12MigrationRebuild: TestV12MigrationRebuild#
  TestV12MigrationRebuild.test_migration_degrades_silently_without_fts5._NoFts5Conn.execute: TestV12MigrationRebuild#test_migration_degrades_silently_without_fts5()._NoFts5Conn#execute().
  TestV12MigrationRebuild.test_migration_degrades_silently_without_fts5._NoFts5Conn.executescript: TestV12MigrationRebuild#test_migration_degrades_silently_without_fts5()._NoFts5Conn#executescript().
---
# Module: [`tests/unit/test_fts_porter_stemming.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py)

## Classes
### `TestBm25RankingStillApplies`
- def: [`tests/unit/test_fts_porter_stemming.py:152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L152)
- signature: `class TestBm25RankingStillApplies:`
- members:
  - `test_relevance_scores_normalized_and_descending(self)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L153)
- uses (calls/refs, reference-scoped): [`fts_search_ranked`](../../tree_sitter_analyzer/_ast_cache_query.md#fts_search_ranked), [`SCHEMA_V2_FTS`](../../tree_sitter_analyzer/_ast_cache_schema.md#SCHEMA_V2_FTS)  (1 test-only)

### `TestExactTokenQueriesUnchanged`
- def: [`tests/unit/test_fts_porter_stemming.py:130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L130)
- signature: `class TestExactTokenQueriesUnchanged:`
- members:
  - `test_exact_identifier_query_identical_old_vs_new(self, query, expected_names)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L138)
- uses (calls/refs, reference-scoped): [`fts_search_ranked`](../../tree_sitter_analyzer/_ast_cache_query.md#fts_search_ranked), [`SCHEMA_V2_FTS`](../../tree_sitter_analyzer/_ast_cache_schema.md#SCHEMA_V2_FTS)  (3 test-only)

### `TestPorterStemmingRecall`
- def: [`tests/unit/test_fts_porter_stemming.py:106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L106)
- signature: `class TestPorterStemmingRecall:`
- members:
  - `test_dispatching_matches_dispatch_family(self)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L112) — Porter stems query + index: exactly the 3 dispatch symbols match.
  - `test_old_tokenizer_misses_dispatching(self)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L107) — Executable record of the pre-#604 gap: default tokenizer → 0 hits.
  - `test_stemming_does_not_leak_unrelated_symbols(self)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L118) — handle_call_tool shares no stem with "dispatching" — excluded.
- uses (calls/refs, reference-scoped): [`fts_search_ranked`](../../tree_sitter_analyzer/_ast_cache_query.md#fts_search_ranked), [`SCHEMA_V2_FTS`](../../tree_sitter_analyzer/_ast_cache_schema.md#SCHEMA_V2_FTS)  (3 test-only)

### `TestV12MigrationRebuild`
- def: [`tests/unit/test_fts_porter_stemming.py:167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L167)
- signature: `class TestV12MigrationRebuild:`
- members:
  - `_build_legacy_db(self, tmp_path)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L168) — Hand-build a cache DB exactly as pre-#604 code would have left it.
  - `test_existing_cache_rebuilt_with_stemming(self, tmp_path)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L195)
  - `test_fresh_cache_end_to_end(self, tmp_path)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L248) — Index a real file through ASTCache — stemmed recall on a fresh DB.
  - `test_migration_degrades_silently_without_fts5(self)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L231) — FTS5-less builds: OperationalError is swallowed, version NOT stamped.
  - `test_migration_idempotent_on_second_open(self, tmp_path)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L214)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`fts_search_ranked`](../../tree_sitter_analyzer/_ast_cache_query.md#fts_search_ranked), [`fts_search_ranked`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.fts_search_ranked), [`apply_migration_v12`](../../tree_sitter_analyzer/_ast_cache_schema.md#apply_migration_v12), [`SCHEMA_V1`](../../tree_sitter_analyzer/_ast_cache_schema.md#SCHEMA_V1), [`SCHEMA_VERSIONS_DDL`](../../tree_sitter_analyzer/_ast_cache_schema.md#SCHEMA_VERSIONS_DDL)  (4 test-only)

### `_NoFts5Conn`
- def: [`tests/unit/test_fts_porter_stemming.py:235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L235)
- signature: `class _NoFts5Conn:`
- members:
  - `execute(self, *args, **kwargs)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L236)
  - `executescript(self, *args, **kwargs)` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L239)
- used by: (1 test-only callers)

## Functions
- `_make_conn(ddl: str)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L78)
- `_names(rows: list[dict])` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L97)

## Module values
- `_FTS5_AVAILABLE` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L33)
- `_OLD_FTS_DDL` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L48)
- `_SYMBOLS` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L70)
- `_c` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L35)
- `pytestmark` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_fts_porter_stemming.py#L41)

