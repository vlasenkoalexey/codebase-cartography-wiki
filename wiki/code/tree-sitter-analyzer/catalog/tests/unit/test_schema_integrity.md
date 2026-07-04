---
title: 'Module: tests/unit/test_schema_integrity.py'
type: catalog
provenance: extracted
module: tests/unit/test_schema_integrity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_schema_integrity`/
symbols:
  TestSelfCheckDetection.test_self_check_error_message_lists_all_problems: TestSelfCheckDetection#test_self_check_error_message_lists_all_problems().
  TestLegacyRecovery.test_legacy_db_without_version_table_is_recovered: TestLegacyRecovery#test_legacy_db_without_version_table_is_recovered().
  TestSelfCheckDetection.test_self_check_detects_missing_column: TestSelfCheckDetection#test_self_check_detects_missing_column().
  TestSelfCheckDetection.test_self_check_detects_missing_table: TestSelfCheckDetection#test_self_check_detects_missing_table().
  TestFreshDb.test_fresh_db_applies_all_versions: TestFreshDb#test_fresh_db_applies_all_versions().
  _seed_healthy_db: _seed_healthy_db().
  _open_db: _open_db().
  TestFreshDb.test_fresh_db_self_check_passes: TestFreshDb#test_fresh_db_self_check_passes().
  _drop_column_raw: _drop_column_raw().
  _make_proj: _make_proj().
  _seed_legacy_db_without_version_table: _seed_legacy_db_without_version_table().
  _drop_table_raw: _drop_table_raw().
  _column_names: _column_names().
  TestFreshDb: TestFreshDb#
  TestSelfCheckDetection: TestSelfCheckDetection#
  TestLegacyRecovery: TestLegacyRecovery#
---
# Module: [`tests/unit/test_schema_integrity.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py)

## Classes
### `TestFreshDb`
- def: [`tests/unit/test_schema_integrity.py:115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L115)
- signature: `class TestFreshDb:`
- members:
  - `test_fresh_db_applies_all_versions(self, tmp_path: Path)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L116) — A brand-new ASTCache stamps every expected version row.
  - `test_fresh_db_self_check_passes(self, tmp_path: Path)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L135) — Constructing ASTCache on a fresh dir must not raise.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`EXPECTED_SCHEMA_VERSIONS`](../../tree_sitter_analyzer/_ast_cache_schema.md#EXPECTED_SCHEMA_VERSIONS.EXPECTED_SCHEMA_VERSIONS)  (1 test-only)

### `TestLegacyRecovery`
- def: [`tests/unit/test_schema_integrity.py:228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L228)
- signature: `class TestLegacyRecovery:`
- members:
  - `test_legacy_db_without_version_table_is_recovered(self, tmp_path: Path)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L229) — All tables present + empty ast_schema_version → backfilled on
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`EXPECTED_SCHEMA_VERSIONS`](../../tree_sitter_analyzer/_ast_cache_schema.md#EXPECTED_SCHEMA_VERSIONS.EXPECTED_SCHEMA_VERSIONS)  (3 test-only)

### `TestSelfCheckDetection`
- def: [`tests/unit/test_schema_integrity.py:154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L154)
- signature: `class TestSelfCheckDetection:`
- members:
  - `test_self_check_detects_missing_column(self, tmp_path: Path)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L159) — Drop callee_resolution from the unified ``edges`` table → error.
  - `test_self_check_detects_missing_table(self, tmp_path: Path)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L182) — Drop ast_imports → SchemaIntegrityError.
  - `test_self_check_error_message_lists_all_problems(self, tmp_path: Path)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L195) — Multiple missing things → error lists ALL of them in one raise.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`SchemaIntegrityError`](../../tree_sitter_analyzer/ast_cache.md#SchemaIntegrityError)  (4 test-only)

## Functions
- `_column_names(conn: sqlite3.Connection, table: str)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L36)
- `_drop_column_raw(db_path: str, table: str, column_to_drop: str)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L62) — Drop a column via raw connection (CREATE-AS-SELECT rename trick).
- `_drop_table_raw(db_path: str, table: str)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L91) — Drop ``table`` via a raw connection (no ASTCache open).
- `_make_proj(tmp_path: Path)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L101) — Return (proj_root, db_path) with the .ast-cache dir pre-created.
- `_open_db(cache: ASTCache)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L29) — Fresh SQLite handle separate from the WAL-mode cache connection.
- `_seed_healthy_db(db_path: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L40) — Build a complete, healthy cache DB at ``db_path`` and close it.
- `_seed_legacy_db_without_version_table(db_path: str)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_schema_integrity.py#L50) — Healthy DB then DELETE every ast_schema_version row — simulates a

