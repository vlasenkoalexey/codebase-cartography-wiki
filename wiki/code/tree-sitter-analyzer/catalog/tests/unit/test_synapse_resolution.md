---
title: 'Module: tests/unit/test_synapse_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_synapse_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_synapse_resolution`/
symbols:
  TestResolverModuleSurface.test_resolve_callee_returns_expected_tuple_shape: TestResolverModuleSurface#test_resolve_callee_returns_expected_tuple_shape().
  TestRFC0002BuiltinClassifier.test_stdlib_import_wins_over_builtin_name_collision: TestRFC0002BuiltinClassifier#test_stdlib_import_wins_over_builtin_name_collision().
  _open_db: _open_db().
  TestResolveLocal.test_resolve_local_function_call_persists_symbol_id: TestResolveLocal#test_resolve_local_function_call_persists_symbol_id().
  TestResolveLocal.test_method_resolution_via_self: TestResolveLocal#test_method_resolution_via_self().
  TestResolveCrossFile.test_resolve_cross_file_via_from_import: TestResolveCrossFile#test_resolve_cross_file_via_from_import().
  TestResolveCrossFile.test_qualified_call_module_alias: TestResolveCrossFile#test_qualified_call_module_alias().
  TestResolveStdlib.test_resolve_stdlib_path_tagged_not_entered: TestResolveStdlib#test_resolve_stdlib_path_tagged_not_entered().
  TestResolveUnknown.test_unknown_callee_fallback: TestResolveUnknown#test_unknown_callee_fallback().
  TestResolverModuleSurface.test_resolve_callee_uses_shared_resolver_for_local_and_import: TestResolverModuleSurface#test_resolve_callee_uses_shared_resolver_for_local_and_import().
  TestSchemaMigration.test_schema_migration_adds_columns: TestSchemaMigration#test_schema_migration_adds_columns().
  TestResolveCrossFile.test_cross_file_edge_count_nonzero_after_index: TestResolveCrossFile#test_cross_file_edge_count_nonzero_after_index().
  TestStarImportBookkeeping.test_star_import_recorded: TestStarImportBookkeeping#test_star_import_recorded().
  _make_pkg: _make_pkg().
  TestRFC0002BuiltinClassifier.test_builtin_name_resolves_to_builtin: TestRFC0002BuiltinClassifier#test_builtin_name_resolves_to_builtin().
  TestRFC0002Monotonicity.test_reindex_does_not_regress_resolved_edges: TestRFC0002Monotonicity#test_reindex_does_not_regress_resolved_edges().
  TestRFC0002DistinctSymbolIds.test_same_named_functions_in_different_files_get_distinct_ids: TestRFC0002DistinctSymbolIds#test_same_named_functions_in_different_files_get_distinct_ids().
  TestRFC0002HyphaeCalleeFalsePositive.test_resolution_rate_above_zero_for_simple_project: TestRFC0002HyphaeCalleeFalsePositive#test_resolution_rate_above_zero_for_simple_project().
  TestSchemaMigration.test_callee_resolution_default_is_unknown: TestSchemaMigration#test_callee_resolution_default_is_unknown().
  TestResolverModuleSurface.test_convenience_context_loads_lazily_and_reuses_lru_cache: TestResolverModuleSurface#test_convenience_context_loads_lazily_and_reuses_lru_cache().
  TestRFC0002BuiltinClassifier.test_project_binding_shadows_builtin: TestRFC0002BuiltinClassifier#test_project_binding_shadows_builtin().
  TestRFC0002BuiltinClassifier._make_ctx: TestRFC0002BuiltinClassifier#_make_ctx().
  _edges_for_caller: _edges_for_caller().
  _copy_fixture: _copy_fixture().
  _column_names: _column_names().
  _FIXTURE_DIR: _FIXTURE_DIR.
  _table_exists: _table_exists().
  TestSchemaMigration: TestSchemaMigration#
  TestResolveLocal: TestResolveLocal#
  TestResolveCrossFile: TestResolveCrossFile#
  TestResolveStdlib: TestResolveStdlib#
  TestResolveUnknown: TestResolveUnknown#
  TestResolverModuleSurface: TestResolverModuleSurface#
  TestResolverModuleSurface.test_public_api_present: TestResolverModuleSurface#test_public_api_present().
  TestStarImportBookkeeping: TestStarImportBookkeeping#
  TestRFC0002BuiltinClassifier: TestRFC0002BuiltinClassifier#
  TestRFC0002Monotonicity: TestRFC0002Monotonicity#
  TestRFC0002DistinctSymbolIds: TestRFC0002DistinctSymbolIds#
  TestRFC0002HyphaeCalleeFalsePositive: TestRFC0002HyphaeCalleeFalsePositive#
---
# Module: [`tests/unit/test_synapse_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py)

## Classes
### `TestRFC0002BuiltinClassifier`
- def: [`tests/unit/test_synapse_resolution.py:555`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L555)
- doc: RFC-0002 criterion 1+2: builtins get `"builtin"` (not `"stdlib"`),
- signature: `class TestRFC0002BuiltinClassifier:`
- members:
  - `test_builtin_name_resolves_to_builtin(self)` — [`L580`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L580) — ``len()`` with no local shadow → resolution="builtin" (RFC-0002 criterion 1).
  - `test_project_binding_shadows_builtin(self)` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L592) — A project function named ``len`` shadows the builtin (RFC-0002 criterion 2).
  - `test_stdlib_import_wins_over_builtin_name_collision(self)` — [`L610`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L610) — When a name is both a known builtin and stdlib-imported, stdlib wins (runs earlier).
- protocol/private: `_make_ctx`[`L559`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L559)
- uses (calls/refs, reference-scoped): [`ResolverContext`](../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`resolve_callee`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#resolve_callee), [`resolution`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolution), [`local_name`](../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.local_name), [`CalleeResolver`](../../tree_sitter_analyzer/callee_resolution.md#CalleeResolver), [`ImportEntry`](../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry), [`module_path`](../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.module_path), [`callee_symbol_id`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.callee_symbol_id), [`file_path`](../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.file_path), [`language`](../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.language)

### `TestRFC0002DistinctSymbolIds`
- def: [`tests/unit/test_synapse_resolution.py:705`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L705)
- doc: RFC-0002 criterion 4: similarly-named functions in different files must
- signature: `class TestRFC0002DistinctSymbolIds:`
- members:
  - `test_same_named_functions_in_different_files_get_distinct_ids(self, tmp_path: Path)` — [`L709`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L709) — Two local ``helper()`` functions each called from their own file
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn)

### `TestRFC0002HyphaeCalleeFalsePositive`
- def: [`tests/unit/test_synapse_resolution.py:754`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L754)
- doc: RFC-0002 criterion 6: resolution rate on a small project must be
- signature: `class TestRFC0002HyphaeCalleeFalsePositive:`
- members:
  - `test_resolution_rate_above_zero_for_simple_project(self, tmp_path: Path)` — [`L758`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L758) — After indexing, at least one call edge must be resolved (not bare-name).
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn)

### `TestRFC0002Monotonicity`
- def: [`tests/unit/test_synapse_resolution.py:645`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L645)
- doc: RFC-0002 criterion 7: a re-index must not regress resolved edges back to unknown.
- signature: `class TestRFC0002Monotonicity:`
- members:
  - `test_reindex_does_not_regress_resolved_edges(self, tmp_path: Path)` — [`L653`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L653)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn)

### `TestResolveCrossFile`
- def: [`tests/unit/test_synapse_resolution.py:245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L245)
- doc: Resolution priority 3: imported name → 'project' with target file.
- signature: `class TestResolveCrossFile:`
- members:
  - `test_cross_file_edge_count_nonzero_after_index(self, tmp_path: Path)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L307) — After indexing a multi-file fixture, at least one 'project'
  - `test_qualified_call_module_alias(self, tmp_path: Path)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L275) — `bb.baz()` after `from . import b as bb` resolves to b.py.
  - `test_resolve_cross_file_via_from_import(self, tmp_path: Path)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L248) — `from .b import baz` makes baz() resolve to b.py.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project)  (3 test-only)

### `TestResolveLocal`
- def: [`tests/unit/test_synapse_resolution.py:183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L183)
- doc: Resolution priority 1: file-local symbol → 'local'.
- signature: `class TestResolveLocal:`
- members:
  - `test_method_resolution_via_self(self, tmp_path: Path)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L218) — `self.m2()` inside m1 resolves to the m2 method on the same class.
  - `test_resolve_local_function_call_persists_symbol_id(self, tmp_path: Path)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L186) — `foo` calling `bar` in the same file resolves to bar's row id.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project)  (3 test-only)

### `TestResolveStdlib`
- def: [`tests/unit/test_synapse_resolution.py:334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L334)
- doc: Resolution priority 4: stdlib allowlist → 'stdlib', not entered.
- signature: `class TestResolveStdlib:`
- members:
  - `test_resolve_stdlib_path_tagged_not_entered(self, tmp_path: Path)` — [`L337`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L337) — `Path('x')` after `from pathlib import Path` is tagged stdlib;
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project)  (3 test-only)

### `TestResolveUnknown`
- def: [`tests/unit/test_synapse_resolution.py:370`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L370)
- doc: Resolution priority 6: nothing matched → 'unknown'.
- signature: `class TestResolveUnknown:`
- members:
  - `test_unknown_callee_fallback(self, tmp_path: Path)` — [`L373`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L373) — A call to an undefined/non-imported name resolves to 'unknown'.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project)  (3 test-only)

### `TestResolverModuleSurface`
- def: [`tests/unit/test_synapse_resolution.py:399`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L399)
- doc: The new `tree_sitter_analyzer.synapse_resolver` module must export
- signature: `class TestResolverModuleSurface:`
- members:
  - `test_convenience_context_loads_lazily_and_reuses_lru_cache(self, monkeypatch: pytest.MonkeyPatch)` — [`L474`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L474) — Constructing ResolverContext should be cheap; first use loads maps.
  - `test_public_api_present(self, attr: str)` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L409)
  - `test_resolve_callee_returns_expected_tuple_shape(self, tmp_path: Path)` — [`L414`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L414) — `resolve_callee` returns a value with the documented attributes.
  - `test_resolve_callee_uses_shared_resolver_for_local_and_import(self)` — [`L437`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L437) — Synapse keeps its cascade while sharing local/import resolution.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`ResolverContext`](../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`resolve_callee`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#resolve_callee), [`resolution`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolution), [`CalleeResolver`](../../tree_sitter_analyzer/callee_resolution.md#CalleeResolver), [`resolved_file`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolved_file), [`callee_symbol_id`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.callee_symbol_id), [`file_symbols`](../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext.file_symbols), [`clear_resolver_context_cache`](../../tree_sitter_analyzer/synapse_resolver/_context.md#clear_resolver_context_cache)  (1 test-only)

### `TestSchemaMigration`
- def: [`tests/unit/test_synapse_resolution.py:103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L103)
- doc: The cache DB must surface the new columns / table on first init.
- signature: `class TestSchemaMigration:`
- members:
  - `test_callee_resolution_default_is_unknown(self, tmp_path: Path)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L147) — Pre-resolution rows default to callee_resolution='unknown'.
  - `test_schema_migration_adds_columns(self, tmp_path: Path)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L106) — The unified ``edges`` table carries callee_symbol_id /
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close)  (3 test-only)

### `TestStarImportBookkeeping`
- def: [`tests/unit/test_synapse_resolution.py:516`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L516)
- doc: Star imports MUST be recorded in ast_imports with is_star=1.
- signature: `class TestStarImportBookkeeping:`
- members:
  - `test_star_import_recorded(self, tmp_path: Path)` — [`L523`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L523)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project)  (2 test-only)

## Functions
- `_column_names(conn: sqlite3.Connection, table: str)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L70)
- `_copy_fixture(name: str, dest_dir: Path)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L34) — Copy a single fixture file into ``dest_dir``.
- `_edges_for_caller(conn: sqlite3.Connection, caller_name: str, pkg_name: str = "synapse_pkg")` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L82) — CALLS edges for ``caller_name`` (unified ``edges`` table), scoped to pkg.
- `_make_pkg(tmp_path: Path, files: list[str], pkg_name: str = "synapse_pkg")` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L48) — Build a fixture project at ``tmp_path/pkg_name`` with the given files.
- `_open_db(cache: ASTCache)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L63) — Fresh SQLite connection (separate from ASTCache's WAL handle).
- `_table_exists(conn: sqlite3.Connection, name: str)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L74)

## Module values
- `_FIXTURE_DIR` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_synapse_resolution.py#L26)

