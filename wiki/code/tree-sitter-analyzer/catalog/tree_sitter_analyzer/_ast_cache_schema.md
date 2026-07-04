---
title: 'Module: tree_sitter_analyzer/_ast_cache_schema.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_cache_schema.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_cache_schema`/
symbols:
  init_db: init_db().
  RecordFn: RecordFn.
  apply_migration_v10: apply_migration_v10().
  apply_migration_v8: apply_migration_v8().
  apply_migration_v12: apply_migration_v12().
  apply_large_repo_indexes: apply_large_repo_indexes().
  apply_migration_v3: apply_migration_v3().
  apply_migration_v4: apply_migration_v4().
  apply_migration_v5: apply_migration_v5().
  apply_migration_v6: apply_migration_v6().
  apply_migration_v9: apply_migration_v9().
  apply_migration_v11: apply_migration_v11().
  SCHEMA_V2_FTS: SCHEMA_V2_FTS.
  EXPECTED_SCHEMA_VERSIONS.EXPECTED_SCHEMA_VERSIONS: EXPECTED_SCHEMA_VERSIONS.EXPECTED_SCHEMA_VERSIONS.
  apply_migration_v7: apply_migration_v7().
  check_schema_expectations: check_schema_expectations().
  SCHEMA_V1: SCHEMA_V1.
  SCHEMA_VERSIONS_DDL: SCHEMA_VERSIONS_DDL.
  SQL_GET_SCHEMA_VERSION: SQL_GET_SCHEMA_VERSION.
  get_table_columns: get_table_columns().
  backfill_schema_version_row: backfill_schema_version_row().
  clear_activation_for_file: clear_activation_for_file().
  SCHEMA_V3_CALL_EDGES: SCHEMA_V3_CALL_EDGES.
  SCHEMA_V4_IMPORTS: SCHEMA_V4_IMPORTS.
  SCHEMA_V5_ACTIVATION: SCHEMA_V5_ACTIVATION.
  SCHEMA_V6_VIOLATIONS: SCHEMA_V6_VIOLATIONS.
  SCHEMA_V9_UNRESOLVED_REFS: SCHEMA_V9_UNRESOLVED_REFS.
  SQL_TABLE_EXISTS: SQL_TABLE_EXISTS.
  already_applied_versions: already_applied_versions().
  record_schema_version: record_schema_version().
  LARGE_REPO_INDEXES.LARGE_REPO_INDEXES: LARGE_REPO_INDEXES.LARGE_REPO_INDEXES.
  SQL_COUNT_SYMBOL_ROWS: SQL_COUNT_SYMBOL_ROWS.
---
# Module: [`tree_sitter_analyzer/_ast_cache_schema.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py)

## Functions
- `already_applied_versions(conn: sqlite3.Connection)` — [`L620`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L620) — Return the set of schema versions already recorded in ast_schema_version.
- `apply_large_repo_indexes(conn: sqlite3.Connection)` — [`L606`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L606) — Create non-shape-changing indexes for large-repo query hot paths.
- `apply_migration_v10(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L312`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L312) — Promote caller/callee/file scalars to real ``edges`` columns (v10 — B1.1).
- `apply_migration_v11(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L340`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L340) — Consolidate to a single edge table — drop ast_call_edges + unresolved_refs.
- `apply_migration_v12(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L369`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L369) — Rebuild ``ast_symbols_fts`` with porter stemming (v12 — #604).
- `apply_migration_v3(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L162`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L162) — Create ``ast_call_edges`` table and its indexes (v3).
- `apply_migration_v4(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L175) — Add Synapse resolution columns + ``ast_imports`` table (v4).
- `apply_migration_v5(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L223`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L223) — Create ``ast_symbol_activation`` table (v5 — Temporal Activation).
- `apply_migration_v6(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L236`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L236) — Create ``ast_constraint_violations`` table (v6 — Constraint DSL).
- `apply_migration_v7(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L250`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L250) — Add ``extractor_version`` column to ``ast_index`` (v7).
- `apply_migration_v8(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L269`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L269) — Create unified ``edges`` table (v8 — EdgeStore).
- `apply_migration_v9(conn: sqlite3.Connection, record_fn: RecordFn)` — [`L302`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L302) — Create ``unresolved_refs`` table (v9 — cross-file second pass).
- `backfill_schema_version_row(conn: sqlite3.Connection, version: int, description: str, missing: list[str])` — [`L646`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L646) — INSERT OR IGNORE a version row for a legacy DB that predates the registry.
- `check_schema_expectations(conn: sqlite3.Connection, expectations: dict[str, list[str]], missing: list[str])` — [`L575`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L575) — Confirm every expected table + column from one version block exists.
- `clear_activation_for_file(conn: sqlite3.Connection, rel_path: str)` — [`L669`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L669) — Drop stale activation rows when project indexing runs in fast mode.
- `get_table_columns(conn: sqlite3.Connection, table: str)` — [`L566`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L566) — Return the column names of ``table``, or empty set when absent.
- `init_db(conn: sqlite3.Connection, fts5_available: bool | None, has_fts5_fn: Any, migrations: list[tuple[int, Any]])` — [`L680`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L680) — Apply schema DDL and migrations. Returns updated fts5_available flag.
- `record_schema_version(conn: sqlite3.Connection, version: int, description: str)` — [`L629`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L629) — Stamp a row in ast_schema_version after a migration block applies.

## Module values
- `EXPECTED_SCHEMA_VERSIONS` — [`L474`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L474)
- `LARGE_REPO_INDEXES` — [`L450`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L450)
- `RecordFn` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L155)
- `SCHEMA_V1` — [`L403`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L403)
- `SCHEMA_V2_FTS` — [`L425`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L425)
- `SCHEMA_V3_CALL_EDGES` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L24)
- `SCHEMA_V4_IMPORTS` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L68)
- `SCHEMA_V5_ACTIVATION` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L99)
- `SCHEMA_V6_VIOLATIONS` — [`L131`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L131)
- `SCHEMA_V9_UNRESOLVED_REFS` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L281)
- `SCHEMA_VERSIONS_DDL` — [`L466`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L466)
- `SQL_COUNT_SYMBOL_ROWS` — [`L557`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L557)
- `SQL_GET_SCHEMA_VERSION` — [`L556`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L556)
- `SQL_TABLE_EXISTS` — [`L555`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_cache_schema.py#L555)

